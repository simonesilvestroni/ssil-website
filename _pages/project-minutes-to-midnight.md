---
layout: page
title: 'Minutes to Midnight - Official website'
date: '2022-02-12'
last_modified_at: '2023-04-25 18:37:08'
skillset:
  - Jekyll
  - Liquid
  - Markdown
  - HTML
  - CSS
  - Netlify
  - Git
  - Bash
  - Microformats
  - Webmentions
  - Indieweb
description: 'Why Minutes to Midnight’s new website eclipses the previous on IA, performance, sustainability and maintenance.'
permalink: '/project-minutes-to-midnight/'
---
<div class="notice">
  <h3>Skills</h3>
  {% for skill in page.skillset %}
  <kbd>{{ skill }}</kbd>
  {% endfor %}
</div>

### Controlling the source

Starting out in the Nineties, I could write HTML code with a simple text editor. Anything that could go wrong was under my hands: 

- easy to find
- easy to fix
- fast to serve
- quick to download

Then, the idea of a CMS seduced me. **I'd been using WordPress since version `1.5`**. I can honestly say I know my way around it. Either on my own or with my former [UI Farm team](https://web.archive.org/web/20220424052100/https://uifarm.co.uk/), I designed and coded custom themes and plug-ins for a large number of clients.

There won't be criticism directed at WordPress in this case study. It's a personal account of a change of direction that was beneficial to me. I will note similarities and a way to maintain a sort of continuity between then and now. The rationale behind the choice of leaving the CMS is quite simple in the end&nbsp;—&nbsp;to gain unconditional control over the workflow:

- Handling the code from top to bottom.
- Owning the visual design to its fullest.
- Writing in HTML and [Markdown](https://en.wikipedia.org/wiki/Markdown) using whichever editor.
- Knowing _what_ every single bit of the building process is doing, _why_ and _how_.

### Sustainability

WordPress can serve websites with optimal performance; however, as a database-driven system it needs time to communicate with a remote server in order to return the page requested by the browser. I don't need that. Even if this is solved with an aggressive cache policy, the way it works inevitably leads to files and database swelling over time, requiring constant maintenance and several chores that I wanted to rid of.

When my simple WordPress site ballooned to an unreasonable **740 MB** over a a couple of years — despite my relentless maintenance — I wanted a change. Following the principle of pre-rendering and decoupling,[^1] I dropped both WordPress and my hosting service SiteGround, switching to [Jekyll](https://jekyllrb.com/) and [Netlify](https://netlify.com).

Jekyll takes content written either in Markdown or HTML, organized in [Liquid](https://shopify.github.io/liquid/) templates, and builds a static website ready to be uploaded to any web server. I wasn't interested in pre-built themes, so I built the whole system from scratch.

### Moving the content

The change carried the possibility of rethinking the information architecture. Before importing anything from my old site, [Silvia](https://silviamaggidesign.com) helped me reorganizing and refocusing the content, putting my multi-disciplinary skills back together. I realized the importance of this stage later in the project, when I saw how convoluted was my previous navigation and how much material I decided to remove.

I then [imported posts and pages](https://import.jekyllrb.com/docs/wordpress/).

To avoid too many SEO issues, I used a redirection feature provided by Netlify in the form of a simple plain text `_redirects` file. It also supports wildcards:

```
https://blog.minutestomidnight.co.uk/* https://minutestomidnight.co.uk/blog/:splat 301!
```

### Liquid template language

[Liquid](https://github.com/Shopify/liquid/) is an open source template language written in Ruby. It was created by Shopify and is now used in Jekyll, Salesforce, Zendesk, 500px and more.[^2] Coming from PHP, I've found Liquid incredibly intuitive: a simpler programming language, yet powerful enough to let me build complex component that fuels the static site.

### Layouts

I built specific layouts for pages, projects, posts, archives and landing pages. The functionality is vaguely similar to templates in WordPress. I love how layouts in Jekyll *can be nested*, thus the possibility to build powerful and complex structures. Key to this are:

- The special Liquid variable `{% raw %}{{ content }}{% endraw %}`, whose value is the rendered content of the post or page being wrapped.
- The `layout` declaration at the top of each page and post.

For example, after creating the `default.html` layout containing a general structure and all the basic inclusions like header, main and footer, a second layout called `page.html` can inherit. It’s just a matter of adding a declaration in the second layout:

```yml
---
layout: default
---
```

The above instruction allows the **page layout** to be entirely included in the `{% raw %}{{ content }}{% endraw %}` variable of `default.html`.

### Modularity

An array of components are collected in an `_includes/` folder. They can be site-wide, such as footer and header, or embeddable modules. The latter type (i.e. images, videos etc.) is recurringly added to posts and pages. 

Embeddable modules works in a similar fashion as shortcodes[^3] in WordPress.

#### Module example: YouTube

This is a simple module to embed YouTube videos, through the [open source front-end Invidious](https://invidious.io/), called `pattern-video.html`:

```liquid
{% raw %}<div class="video iframe-container">
  <iframe loading="lazy" src="https://yewtu.be/embed/{{ include.id }}" frameborder="0" allowfullscreen title="{{ include.title | default: "Video" }}"></iframe>
</div>{% endraw %}
```

Whenever I need to embed a video, I just call a snippet, passing a video ID parameter and an optional title:

```liquid
{% raw %}{% include pattern-video.html id="N0Sa-1Vqn6g" title="Berlin 91 official music video" %}{% endraw %}
```

#### Automating the embed

I've been using [Alfred](https://www.alfredapp.com/) on macOS for many years. Among other things, it offers access to clipboard history and **creation of custom text snippets**. A keyword for each snippet can be set. For example, to embed my include code for adding a `<figure>` tag, I type <kbd>/figure</kbd> and then complete the missing data where `000` is present:

{% include pattern-figure.html image="/assets/img/embed-figure.gif" alt="Short animation of how I embed a figure tag" caption="Embedding a figure tag using Alfred" width="1050" height="470" %}

Like the block editor in WordPress, I associated keywords such as <kbd>/image</kbd>, <kbd>/video</kbd> and so on. All modules, whether simple or complex, work the same way. I can also recall Alfred's snippets window with my shortcut <kbd>⌥ ⌘ C</kbd>, select the one I need and hit enter.

{% include pattern-figure.html image="/assets/img/embed-alfred.jpg" alt="Alfred's snippets recall window" caption="Alfred's snippets recall window" width="960" height="562" %}

### Markdown

Posts, notes, pages and projects are written in Markdown. Jekyll's [Kramdown](https://jekyllrb.com/docs/configuration/markdown/) implementation includes footnotes, code highlighting and more. Projects are particular content types outside the posts loop, created using [collections](https://jekyllrb.com/docs/step-by-step/09-collections/). Not too different from custom post types in WordPress.

### Design

The theme is handcrafted by applying styles to the layouts. I'm using [Simple CSS](https://simplecss.org) as a base, with my custom components built in plain CSS on top of it. I only load a minified stylesheet on production:

```html
{% raw %}{% if jekyll.environment == "production" -%}
<link rel="stylesheet" href="/assets/css/m2m.min.css">
{% else -%}
<link rel="stylesheet" href="/assets/css/m2m.css">
{%- endif -%}{% endraw %}
```

### Meta content

First, I check upon the existence of a variable called `robots`, used to exclude the page from search crawling.

```html
{% raw %}{%- if page.robots %}
<meta name="robots" content="{{ page.robots }}" />
{% endif %}{% endraw %}
```

The page title is rendered based on a few checks:

```liquid
{% raw %}{%- if page.url == "/" -%}
{{ site.title | append: ' – ' }}{{ site.tagline }}
{%- elsif page.type == 'tag' -%}
{{ page.type | capitalize }}: {{ page.title | capitalize | append: ' – ' }}{{ site.title }}
{%- else -%}
{{ page.title | append: ' – ' }}{{ site.title }}
{%- endif -%}{% endraw %}
```

Things I added next:

{: .list-hr }
- Canonical link,[^4] where I check against a page variable to see if the post has already been published elsewhere earlier:
  ```html
  {% raw %}<link rel="canonical" href="{% if page.canonical %}{{ page.canonical }}{% else %}{{ page.url |  replace:'index.html','' | absolute_url }}{% endif %}">{% endraw %}
  ```
- Meta description,[^5] where I check for the presence of a `description` variable. Its fallback value is found in the `config.yml` file:
  
  ```html
  {% raw %}<meta name="description" content="{% if page.description %}{{ page.description }}{% else %}{{ site.description }}{% endif %}">{% endraw %}
  ```
- [Open Graph](https://ogp.me/). This is the content appearing in the 'card' which unfurls when links from my website are shared to social media sites and instant messengers like Telegram. I check for `description` and the presence of a featured image, again with fallbacks.
  ```html
  {% raw %}<meta property="og:title" content="{%- include site-meta-title.html -%}">
  <meta property="og:url" content="{{ page.url | prepend: site.url }}">
  <meta property="og:type" content="website">
  <meta property="og:site_name" content="{{ site.title }}">
  <meta property="og:description" content="{% if page.description %}{{ page.description }}{% elsif note.description %}{{ note.description }}{% else %}{{ site.description }}{% endif %}">
  <meta property="og:image" content="{% if page.featimage %}{{ site.url }}{{ page.featimage-url }}{% else -%}{{ site.logo | prepend: site.url }}{% endif %}">{% endraw %}
  ```
- [Schema](https://schema.org/docs/documents.html) is "a collaborative, community activity with a mission to create, maintain, and promote schemas for structured data on the Internet, on web pages, in email messages, and beyond."
  ```html
  {% raw %}<script type="application/ld+json">
  {
    "@context": "http://schema.org",
    {% if page.is_post -%}
    "@type": "BlogPosting",{% else %}"@type": "WebSite",
    {%- endif %}
    "name": "{%- include site-meta-title.html -%}",
    "headline": "{%- include site-meta-title.html %} {{ site.tagline }}",
    "url": "{{ site.url }}{{ page.url }}",
    "description": "{% if page.description %}{{ page.description }}{% elsif note.description %}{{ note.description }}{% else %}{{ site.description }}{% endif %}",
    "keywords": "{% if page.tags %}{{ page.tags | join: ',' }}{% else %}{{ site.keywords }}{% endif %}",
    {%- assign tagArchive = page.type | where: 'post.type', 'tag' -%}
    {% unless tagArchive %}
    "datePublished": "{{ page.date }}",
    "dateModified": "{{ page.last_modified_at }}",
    {% endunless -%}
    "author": {
      "@type": "Person",
      "name": "Simone Silvestroni",
      "givenName": "Simone",
      "familyName": "Silvestroni"
    },
    "mainEntityOfPage": {
      "@type": "WebPage",
      "@id": "{{ site.url }}{{ page.url }}"
    },
    "sameAs": [
      "https://sonomu.club/@m2m",
      "https://uk.linkedin.com/in/simonesilvestroni/",
      "https://github.com/simonesilvestroni/",
    ],
    {%- if page.featimage %}
    "image": {
      "@type": "ImageObject",
      "width": "1024",
      "height": "765",
      "url": "{{ site.url }}{{ page.featimage-url }}"
    }
    {%- else %}
    "image": {
      "@type": "ImageObject",
      "width": "1200",
      "height": "628",
      "url": "{{ site.url }}{{ site.logo }}"
    }
    {%- endif %}
  }
  </script>{% endraw %}
  ```

Without the need of external plug-ins, all benchmarks gives optimal results with all audits fully passed.

### File management

Since I don't need any setup for Apache, PHP or MySQL, file management is extremely easy. Using GitHub as a versioning system, my local website directory is a perfect mirror of the remote repository. Again, all my images, CSS or other assets are kept together with the source code. No external database to be backed up, no extra maintenance.

### Build process
I use [Bash](https://www.gnu.org/software/bash/) to run Jekyll's internal build tasks, using appropriate aliases in my `bash_profile` for regular localhost preview, serving drafts and future posts.

### Javascript

I don't compile nor minify Javascript because I only use it for the search engine and webmentions, which I never need to edit.

### Performance, accessibility and sustainability

I've been treating [performance as a design feature](https://web.archive.org/web/20130717022229/http://uifarm.co.uk/responsive-design-framework-performance/) for more than ten years. The complete size of the website source code is currently `1.1 MB`, reaching a root total of `23 MB` including images and a `13 MB` PDF file. It's a sensible reduction from the previous `800 MB`.

What contributes to my Pagespeed and Lighthouse score of `100` on performance, accessibility and SEO?

- Semantic and valid structured code.
- Attention to <abbr title="Web Content Accessibility Guidelines">WCAG</abbr> accessibility requirements.
- Use of images only when strictly needed.
- Responsive images (small devices are served with specific smaller versions).
- Avoid Javascript when valid alternatives can be employed.
- Multi-platform font stacks.
- Optimization of static assets.
- A fast and green server.

I also took care of removing files that are not needed on the live server, by adding a second `config-production.yml` which is called in my build command on Netlify. After validating the markup with the [W3C](https://validator.w3.org/nu/?doc=https://minutestomidnight.co.uk/), the final benchmarks shows a <kbd>100</kbd> on all grades for Google Pagespeed and also 100 on Gtmetrix.

The homepage weighs `56 KB` uncompressed and loads in <kbd>0.4 seconds</kbd>. Only `0.01g of CO2` is produced every time someone visits the homepage. Cleaner than `99%` of [web pages tested](https://www.websitecarbon.com/website/minutestomidnight-co-uk/ "Visit Website carbon").

About accessibility:

- Compliant with <abbr title="Web Content Accessibility Guidelines">WCAG</abbr> guidelines
- Current [WAVE accessibility rank](https://webaim.org/projects/million/lookup?domain=minutestomidnight.co.uk): `#7,280` of 1,000,000
- The page content is fully accessible with Javascript turned off
- The dynamic [search functionality](https://minutestomidnight.co.uk/search/) has a plain HTML alternative

### Search

As a static site generator, Jekyll lacks two features: a search functionality and a comment system. I solved the first by including a clever vanilla [Javascript solution](https://github.com/daviddarnes/jekyll-search-js) supported by Liquid syntax to indicize the content. A [script-free solution](https://minutestomidnight.co.uk/search/) using DuckDuckGo is provided.

### Integrations: Webmentions, Indieweb

After deciding to avoid third-party commenting systems, I turned to [webmentions](https://minutestomidnight.co.uk/blog/indieweb-and-webmentions-for-my-static-site/), a decentralized way to interact with other websites' posts, notes, likes and reposts.[^6]

I've been out of mainstream social networks since 2020, so putting my website at the center of my online presence seemed perfect.

<a class="button big" href="https://minutestomidnight.co.uk/"><strong>Visit the live site</strong></a>

---

#### Footnotes

[^1]: Decoupling is the process of creating a clean separation between systems or services. By decoupling the services needed to operate a site, each component part can become easier to reason about, can be independently swapped out or upgraded, and can be designated the purview of dedicated specialists either within an organization, or as a third party.
[^2]: [https://github.com/Shopify/liquid/wiki#who-uses-liquid](https://github.com/Shopify/liquid/wiki#who-uses-liquid)
[^3]: A shortcode is akin to a shortcut to add features to your website that would typically require lots of complicated computer code and technical ability. [Read more](https://wordpress.com/support/shortcodes/).
[^4]: [https://developers.google.com/search/docs/advanced/crawling/consolidate-duplicate-urls](https://developers.google.com/search/docs/advanced/crawling/consolidate-duplicate-urls)
[^5]: [https://developers.google.com/search/docs/advanced/appearance/snippet?hl=en](https://developers.google.com/search/docs/advanced/appearance/snippet?hl=en)
[^6]: A Webmention is a notification that one URL links to another. For example, Alice writes an interesting post on her blog. Bob then writes a response to her post on his own site, linking back to Alice's original post. Bob's publishing software sends a Webmention to Alice notifying that her article was replied to, and Alice's software can show that reply as a comment on the original post.