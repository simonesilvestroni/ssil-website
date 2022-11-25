---
layout: page
title: 'Projects'
date: '2022-11-22 21:06:03'
last_modified_at: '2022-11-22 21:06:06'
description: 'I’ve worked on many projects since the 1990s. A few highlights of the more representative.'
excerpt: 'I’ve worked on many projects since the 1990s. The following are a selection of highlights.'
permalink: '/projects/'
---
{%- assign webdesign = site.webdesign | reverse -%}

{%- for project in webdesign %}
{% include pattern-projectblock.html %}
{% endfor %}

<article class="h-entry m2m-entry my-5 py-3">

<h2 class="fs-3 p-name my-3">A modern workflow for the multi-device web</h2>

<p class="p-summary text-start mt-2">A process analysis that has led UI Farm Ltd to their workflow for delivering modern web solutions.</p>

<a href="https://medium.com/ui-farm/how-we-work-a-modern-workflow-for-the-multi-device-web-4e0dcb081b5b" title="Read the article">Read the article ↗</a>

</article>