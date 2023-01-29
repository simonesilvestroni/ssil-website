---
layout: page
title: 'About'
date: '2022-11-22 21:47:23'
last_modified_at: '2022-11-22 21:47:26'
description: 'A web designer for two decades between Italy and the UK.'
excerpt: 'In the early 1990s, I started a side job in the publishing industry while graduating as a professional musician. A decade later I learned web design, fascinated by code as a digital evolution of my past experience with the printed page.'
permalink: '/about/'
---
As a web designer, in line with my origins, I still <em>strive for minimalism</em>. With a vast experience in front-end development and some back-end, UI design and custom WordPress systems, my main focus is on accessibility and sustainability through a relentless stack optimization.

I also have a parallel career in audio as a professional musician, producer and game sound designer that I carry out under the moniker _Minutes to Midnight_.

{: .d-inline-block .border .border-3 .rounded .mt-3 .px-3 .py-3 }
Check out my [**audio work**](https://minutestomidnight.co.uk) →

## Other interests

An avid reader, I follow recent tech trends through online media, Mastodon, workshops and newsletters. Trivia: I have a longstanding ~~obsession~~ fascination for typography.

Constantly looking for a way to complete a task in less and more efficient steps, I ended up writing an ebook about [project management](https://minutestomidnight.co.uk/projects/project-management/).

{: .d-inline-block .border .border-3 .rounded .mt-3 .px-3 .py-3 }
Read more in my [**resume**](/resume/) →

## Endorsements

<ul class="list-unstyled ps-0">
{% for item in site.endorsements -%}
  <li>
    <blockquote>
      <p>{{ item.quote }}</p>
      <cite><a href="{{ item.url }}">{{ item.name }}</a> — {{ item.role }}</cite>
    </blockquote>
  </li>
{% endfor -%}
</ul>

{: .d-inline-block .border .border-3 .rounded .my-3 .px-3 .py-3 }
[<svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" fill="currentColor" viewBox="0 0 16 16" role="img" aria-label="LinkedIn logo"><path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/></svg> Resume and endorsements on LinkedIn](https://www.linkedin.com/in/simonesilvestroni/) →

## Certifications

<ul>
{% for item in site.certifications -%}
  <li>
    {{ item.name }}
  </li>
{% endfor -%}
</ul>

## About the website

I've been managing all my activies under the moniker _Minutes to Midnight_ — the name I'd trademarked in the UK in 2017. As a consequence of the decision to split audio and web work, I bought my personal domain and moved the web design related content in here.

The website has been developed from scratch using:

- [Jekyll 4.2.1](https://jekyllrb.com/)
- [Markdown (extended)](https://www.markdownguide.org/getting-started/)
- Vanilla javascript for [search module](https://github.com/daviddarnes/jekyll-search-js) and [webmentions](http://beesbuzz.biz)
- Table of contents Liquid code by [Vladimir "allejo" Jimenez](https://github.com/allejo/jekyll-toc)
- Bash for building purposes
- [Github](https://github.com/simonesilvestroni/ssil-website)
- [Mona Sans font](https://github.com/github/mona-sans)
- [Netlify](https://netlify.com)

### Accessibility and sustainability

No errors for <abbr title="Web Content Accessibility Guidelines">WCAG</abbr> detected on [WAVE](https://wave.webaim.org/report#/https://simonesilvestroni.com/) and 100 scored on Google Lighthouse.

Only 0.04g of CO2 is produced every time someone visits the homepage, which is cleaner than 96% of web pages tested. The website is running on sustainable energy.

I [do not request third-party resources](https://aremythirdpartiesgreen.com/test/76e7ac7370d84f1fabd254608e118ff4), except for the blog posts, which are calling `webmention.io` to render web mentions.

Member of the [512kb club](https://512kb.club "Member of the 512kb Orange Team") and the [1Mb club](https://1mb.club/). The markup is valid, the homepage loads in 0.4 seconds and weighs 250KB (uncompressed). 

{: .d-inline-block .border .border-3 .rounded .mt-3 .px-3 .py-3 }
More about my [**ethical choices**](/ethics/) →

## Copyright

The _text content_ of this website is [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/) (CC BY-SA 4.0). It means you are free to share — copy and redistribute the material in any medium or format, adapt — remix, transform, and build upon the material for any purpose, even commercially. You must give appropriate credit, provide a link to the license, and indicate if changes were made.