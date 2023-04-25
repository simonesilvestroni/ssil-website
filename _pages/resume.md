---
layout: page
title: 'Resume'
date: 2023-04-24
last_modified_at: 2023-04-24 22:58:30
description: 'I’ve been a web designer for over twenty years. Here a list of skills, work experience and projects, along with a few endorsements.'
permalink: '/resume/'
---
<div class="notice">
  <h3>Content</h3>
  <ul>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#work-experience">Work Experience</a></li>
    <li><a href="#languages">Languages</a></li>
    <li><a href="#endorsements">Endorsements</a></li>
  </ul>
</div>

### Skills

{: .list-hr }
- I've been crafting websites from scratch with <kbd>HTML</kbd> and <kbd>CSS</kbd> since 1998, later adopting dynamic languages such as <kbd>PHP</kbd> and Shopify's <kbd>Liquid</kbd> to handle the logic and generate the markup, and <kbd>SASS</kbd> for stylesheets.
- Been using <kbd>WordPress</kbd> as my <abbr title="Content Management System">CMS</abbr> of choice since version 1.5, building custom themes and plug-ins. I recently switched to <kbd>Jamstack</kbd> and the static site generator <kbd>Jekyll</kbd> for my recent projects. I use it with or without an headless CMS.
- I can set up, run and maintain local and remote web servers running <kbd>Apache</kbd> and <kbd>MySQL</kbd> either through a GUI or <kbd><abbr title="Secure Shell">SSH</abbr></kbd>.
- Well versed in graphic tools such as <kbd>Sketch</kbd>, <kbd>Figma</kbd> and more, as well as <abbr title="Desktop Publishing">DTP</abbr> software like <kbd>Adobe InDesign</kbd>.
- My code editor of choice is the cross-platform <kbd>Sublime Text</kbd>, using <kbd>git</kbd> as the preferred versioning system.
- I make a point of putting <kbd>performance</kbd>, <kbd>usability</kbd> and <kbd>sustainability</kbd> at the forefront. I strongly dislike the overuse of technology such as <kbd>Javascript</kbd> in modern web development.

### Work Experience

<div class="notice resume-experience">
  <h4>Web designer at <a href="https://minutestomidnight.co.uk">Minutes to Midnight</a></h4>
  <span class="small">2017-present (Cambridge/Milan)</span>
  <p>Design, front-end development, deployment and maintenance.</p>
  <h4>Recent projects</h4>
  <ul>
    <li><a href="{{ site.url }}/project-responsive-photogallery-carousel/">Pure HTML and CSS responsive carousel in Jekyll</a></li>
    <li><a href="{{ site.url }}/project-minutes-to-midnight/">Minutes to Midnight</a></li>
    <li><a href="{{ site.url }}/project-silvia-maggi-design/">Silvia Maggi Design</a></li>
    <li><a href="{{ site.url }}/project-no-slack-day/">No Slack Day</a></li>
  </ul>
  <h4>Publications</h4>
  <ul>
    <li><a href="https://minutestomidnight.co.uk/work/project-management/">Efficient Productivity for Music Professionals</a> (e-Book)</li>
  </ul>
</div>

<div class="notice resume-experience">
  <h4>Front-end web developer at <a href="https://web.archive.org/web/20220424052100/https://uifarm.co.uk/">UI Farm Ltd</a></h4>
  <span class="small">2012-2017 (London)</span>
  <p>Co-founder, web designer and UI developer, I worked for many clients, such as Reevoo, Not On The High Street, UniCredit, Elite, APM, Women Management.</p>
  <p>At UI Farm, we pioneered responsive web design, and I contributed to building a bespoke responsive framework  on top of WordPress (theme, child theme and custom plug-ins), featuring a performance-first approach.</p>
  <h4>Relevant projects</h4>
  <ul>
    <li><a href="{{ site.url }}/project-reevoo/">Reevoo</a></li>
    <li><a href="{{ site.url }}/project-unicredit/">UniCredit</a></li>
  </ul>
  <h4>Publications</h4>
  <ul>
  <li><a href="{{ site.url }}/a-modern-workflow-for-the-multi-device-web/">How we work: a modern workflow for a multi-device web</a></li>
  </ul>
</div>

<div class="notice resume-experience">
  <h4>Senior UI developer at <a href="http://web.archive.org/web/20120302142629/http://www.bodog.eu/">Bodog</a></h4>
  <span class="small">2011-2012 (London)</span>
  <p>Within an Agile environment, I developed gaming and e-sport applications with the accompanying websites — including the then flagship slots.com — using SASS, Drupal (PHP), Javascript, <abbr title="Linux, Apache, MySQL, PHP">LAMP</abbr>, <abbr title="Subversion">SVN</abbr>.</p>
</div>

<div class="notice resume-experience">
  <h4>UI developer at New Energy / Part of Accenture</h4>
  <span class="small">2005-2011 (Milan)</span>
  <p>Initially working for a subsidiary company, I fully joined New Energy as a UI developer, ending up leading a multi-disciplinary UX team. Within the role, I contributed to <strong>UniCredit</strong>’s corporate websites, their online banking system, the online acquisition landing pages and forms.</p>
  <p>I also produced mockups and working prototypes for the in-house usability tests; helped setting up the internal usability lab and led the A/B testing workflow, including <abbr title="Research and development">R&amp;D</abbr> for eye-tracking.</p>
</div>

<div class="notice resume-experience">
  <h4>Web designer at Playstos Entertainment</h4>
  <span class="small">2000-2005 (Milan)</span>
  <p>While I was the team leader and sound designer for the for PlayStation 2 video game <em>Ruff Trigger: The Vanocore Conspiracy</em>, published by Natsume, I was also in charge of the design and development of the company website, its subsidiaries and all the games websites.</p>
  <h4>Projects</h4>
  <ul>
    <li><a href="https://minutestomidnight.co.uk/work/sound-design/ruff-trigger-playstation2-game/">Ruff Trigger console game</a></li>
  </ul>
</div>

### Languages

- **Italian**: native
- **English**: bilingual proficiency
- **German**: elementary

### Endorsements

Check out the [full list on **LinkedIn**](https://www.linkedin.com/in/simonesilvestroni/).

{%- for endorsement in site.endorsements %}
<blockquote>
  <p>{{ endorsement.quote }}</p>
  <cite>&mdash; {{ endorsement.name }}, <a href="{{ endorsement.url }}">{{ endorsement.role }}</a></cite>
</blockquote>
{%- endfor %}