---
layout: page
title: 'No Slack Day'
date: '2021-08-26'
last_modified_at: '2023-04-25 18:37:08'
skillset:
  - Jekyll
  - SASS
  - purgeCSS
  - Git
  - GitHub Pages
  - Node
  - Bootstrap 5
description: 'A yearly reminder of how Slack can also be distracting and counter-productive.'
permalink: '/project-no-slack-day/'
---
<div class="notice">
  <h3>Skills</h3>
  {% for skill in page.skillset %}
  <kbd>{{ skill }}</kbd>
  {% endfor %}
</div>

A cool initiative by an elusive client of mine, No Slack Day is a yearly reminder of how a communication tool can also be distracting and counter-productive. Built using Jekyll and light imagery, I achieved a blazing fast performance for a modern-looking landing page.

<table>
  <thead>
    <tr>
      <th scope="col">Pagespeed score</th>
      <th scope="col">Speed index</th>
      <th scope="col">Page weight</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><kbd>100</kbd></td>
      <td><kbd>0.5 seconds</kbd></td>
      <td><kbd>95 KB</kbd></td>
    </tr>
  </tbody>
</table>

<a class="button big" href="https://web.archive.org/web/20230402145306/https://www.noslackday.org/"><strong>Visit the live site</strong></a>