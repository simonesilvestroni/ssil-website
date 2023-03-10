---
layout: page
title: Resume
date: '2022-04-06 00:04:25'
last_modified_at: '2022-04-14 13:05:45'
description: 'Online cv of Simone Silvestroni, sound and web designer since 1995. Contains skills, tools, work experience, projects, certifications and endorsements.'
permalink: '/resume/'
---
## Skills and tools

I've been crafting websites from scratch with **`HTML`** and **`CSS`** since 1997, later adopting **`PHP`** to generate the markup and **`SASS`** for the stylesheets. I've been using **`WordPress`** as my CMS of choice since version 1.5, building custom themes and plug-ins. I make a point of putting performance, **`usability`** and **`sustainability`** at the forefront. I'm well versed in graphic tools such as **`Figma`**, **`Sketch`** and DTP software like **`Adobe InDesign`**.

I can set up, run and maintain local and remote web servers in **`Apache`**, **`PHP`**, **`MySQL`** either through a GUI or **`SSH`**. I recently moved to static site generators with or without an **`headless CMS`**, especially digging **`Jekyll`** with its **`Liquid`** template language and **`Netlify`** for deployment and production builds. I use **`git`** as a versioning system, with Github as my preferred service.

{: .d-inline-block .border .border-3 .rounded .mt-3 .px-3 .py-3 }
Check out all the [tools I use](https://minutestomidnight.co.uk/uses/) ↗

## Experience

{: .fw-bold .mb-2 }
### Web designer at [Minutes to Midnight](https://minutestomidnight.co.uk)

{: .initialism .fs-6 }
September 2017-present (Cambridge, UK / Milan, Italy)

{: .detached }
Design, front-end development, deployment and maintenance.

#### Projects

{: .list-unstyled .ps-0 }
- [Pure HTML and CSS responsive carousel in Jekyll]({{ site.url }}/projects/web-design/responsive-photogallery-carousel/)
- [Minutes to Midnight]({{ site.url }}/projects/web-design/minutes-to-midnight/)
- [Silvia Maggi Design]({{ site.url }}/projects/web-design/silvia-maggi-design/)
- [No Slack Day]({{ site.url }}/projects/web-design/no-slack-day/)

#### Publications

{: .list-unstyled .ps-0 }
- [Efficient Productivity for Music Professionals ↗︎](https://minutestomidnight.co.uk/projects/project-management/) (e-Book)

{: .fw-bold .mb-2 .pt-3 }
### Front-end web developer at [UI Farm Ltd](https://web.archive.org/web/20220424052100/https://uifarm.co.uk/)

{: .initialism .fs-6 }
May 2012-September 2017 (London, UK)

{: .detached }
Co-founder, web designer and UI developer, I worked for clients like Reevoo, Not On The High Street, UniCredit, Women Management and many others. At UI Farm I contributed to building a bespoke responsive framework on top of WordPress, featuring semantic patterns, a fluid grid and custom plugins. Handcrafted using PHP (HTML5), SASS (CSS3), JavaScript and SVG.

#### Projects

{: .list-unstyled .ps-0 }
- [Reevoo]({{ site.url }}/projects/web-design/reevoo/)
- [UniCredit]({{ site.url }}/projects/web-design/unicredit/)

#### Publications

{: .list-unstyled .ps-0 }
- [How we work: a modern workflow for the multi-device web ↗︎](/blog/a-modern-workflow-for-the-multi-device-web/) (article)

{: .fw-bold .mb-2 .pt-3 }
### Senior UI developer at Bodog

{: .initialism .fs-6 }
September 2011-May 2012 (London, UK)

{: .detached }
Developed gaming and sports applications and accompanying websites, using SASS, Compass, Drupal, jQuery, LAMP, SVN, Web Typography within an Agile environment.

{: .fw-bold .mb-2 .pt-3 }
### UI developer at New Energy / Part of Accenture

{: .initialism .fs-6 }
January 2005-September 2011 (Milan, Italy)

{: .detached }
Initially working for a subsidiary company, I then fully joined New Energy as a UI developer, ending up leading a multi-discipline UX team, composed by programmers, designers and online market specialists. Within that role, I contributed to the development of UniCredit's corporate websites, their online banking system, the online acquisition landing pages and forms. 

I also produced mockups and working prototypes for the usability tests; helped to set up the internal usability lab and led the A/B testing workflow, including R&D for eye-tracking.

{: .fw-bold .mb-2 .pt-3 }
### Web designer at Playstos Entertainment

{: .initialism .fs-6 }
January 2000-January 2005 (Milan, Italy)

{: .detached }
While I was the team leader and sound designer for the title _Ruff Trigger: The Vanocore Conspiracy_, published by Natsume for PlayStation 2, I was also in charge of the design and development of the company website, its subsidiaries and all the games websites.

#### Project

{: .list-unstyled .ps-0 }
- [Ruff Trigger console game](https://minutestomidnight.co.uk/projects/sound-design/console-game-ruff-trigger/)

## Languages

{: .list-unstyled .ps-0 }
- 🇮🇹 **Italian**: native
- 🇬🇧 **English**: bilingual proficiency
- 🇩🇪 **German**: elementary

## Certifications and courses

{: .list-unstyled .ps-0 }
{%- for cert in site.certifications.web %}
- 🏛 {{ cert.name }}.
{%- endfor %}

## Endorsements

{: .d-inline-block .border .border-3 .rounded .mt-3 .px-3 .py-3 }
Check out the [full list on **LinkedIn** ↗︎](https://www.linkedin.com/in/simonesilvestroni/)

{%- assign endorsementweb = site.endorsements.web %}

{%- for endorsement in endorsementweb %}

> {{ endorsement.quote }}
> <cite>&mdash; {{ endorsement.name }}, [{{ endorsement.role }}]({{ endorsement.url }})</cite>

{%- endfor %}