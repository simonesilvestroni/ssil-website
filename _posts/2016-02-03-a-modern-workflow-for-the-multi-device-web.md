---
title: 'A modern workflow for the multi-device web'
date: '2016-02-03'
last_modified_at: '2023-03-10 10:12:09'
categories:
  - 'Web design'
tags:
  - 'responsive web design'
  - 'design'
  - 'development'
  - 'html'
  - 'css'
  - 'javascript'
  - 'framework'
  - 'accessibility'
  - 'sustainability'
  - 'web performance'
  - 'multi-device'
  - 'a-b tests'
  - 'workflow'
  - 'agile'
  - 'popular'
description: 'UI Farm analyses the process that has led to their new workflow for delivering modern web solutions, by applying a sustainable and future-proof use of Responsive Web Design.'
excerpt: 'In this article, <a href="https://web.archive.org/web/20201105212259/http://uifarm.co.uk/">UI Farm</a>, the London-based UI & UX agency, analyses the process that has led to their new workflow for delivering modern web solutions. By applying a sustainable and future-proof use of Responsive Web Design, UI Farm achieve performant, multi-device websites within an agile environment.'
---
**Technical review**: [Kara McCain](https://www.linkedin.com/in/karamccain/)

## About UI Farm

UI Farm are a modern agency committed to creating beautiful, user-centric responsive websites and mobile applications for the multi-device web. UI Farm are passionate about the web and its future — in particular, how responsive design can help businesses grow sustainably online. At UI Farm, their approach is to provide user-centric design and development solutions that are device and platform agnostic.

## Introduction

An always [increasing percentage of global internet traffic is coming from mobile devices](http://www.cisco.com/c/en/us/solutions/collateral/service-provider/visual-networking-index-vni/white_paper_c11-520862.html). UI Farm uses [Responsive Design](http://alistapart.com/article/responsive-web-design) to design and develop powerful and efficient web solutions for the [multi-device world](http://www.lukew.com/ff/entry.asp?1436).

{% include pattern-figure.html image="/assets/images/uif-article/02_mobile-traffic-cisco.jpg" alt="Mobile data traffic looks set to explode, a map by Cisco" caption="Mobile data traffic looks set to explode" width="960" height="684" %}

<small>Source: <a href="http://www.cisco.com/c/en/us/solutions/collateral/service-provider/visual-networking-index-vni/white_paper_c11-520862.html">Cisco</a></small>

## A Traditional Workflow

### **Before the Multi-Device Web**

{% include pattern-figure.html image="/assets/images/uif-article/03_before-phase1.png" alt="Phase 1" caption="Phase 1" width="982" height="330" %}

{% include pattern-figure.html image="/assets/images/uif-article/04_before-phase2.png" alt="Phase 2" caption="Phase 2" width="980" height="334" %}

## What Could Be Improved

### Separate Roles

Web agencies used to keep the roles of the designer and the developer strictly *separate*. Sometimes, none or little knowledge was shared among these roles. This dynamic produced **static design files** from the designers, with developers fighting over the feasibility of every detail.

### Negative Loops

#### Static images

{% include pattern-figure.html image="/assets/images/uif-article/05_negative-loops1.png" alt="Negative loop 1: static images" caption="Negative loop 1: static images" width="406" height="428" %}

Static image files generates negative loops:

- The client must review every design change.
- The designer must apply the change, and re-submit the files for approval.

If the project is a responsive website, the process is going to be repeated for each content view:

- Small Screens
- Tablet
- Desktop
- Large Screens

The whole process of handling this negative loop is:

- Time consuming
- Expensive
- Producing assets that are not ideal in a multi-device web
- Forcing the developers to *adapt a static design to a different media* (the browser)

#### Not the real media

{% include pattern-figure.html image="/assets/images/uif-article/06_negative-loops2.png" alt="Negative Loop 2: Not The Real Media" caption="Negative Loop 2: Not The Real Media" width="405" height="428" %}

The developers’ implementation of static image files creates web pages that have a *different look & feel* from the static designs. This is a fatal flaw, due to the different nature of the media.

In fact, the natural media for a web page is the browser.

## Multi-device web

{% include pattern-figure.html image="/assets/images/uif-article/07_multi-device-web.jpg" alt="A multitude of different devices aligned on a table" width="520" height="286" %}

Welcome to a world where you have neither “standard” devices nor resolutions. Read more about the [multi-device web](/assets/files/uifarm-multi-device-websites.pdf).

### Responsive Web Design

In a multi-device web, Responsive design focuses on running a website on every device.

{% include pattern-figure.html image="/assets/images/uif-article/08_responsive-design.jpg" alt="A models website shown on multiple devices" width="800" height="304" %}

The designer now needs to think about:

1. Device specific behaviour
2. Look & feel on different devices
3. User interaction
4. Performance

UI Farm think it is too hard to achieve this within an old-fashioned workflow, where:

- Roles are separate
- Designers produce static image files
- Efficient Agile methodologies are hard to implement

## An Agile New Workflow

### Agile Project Management

UI Farm uses Atlassian’s JIRA for project management of website projects, to facilitate delivering projects on-time. Throughout the duration of the project UI Farm will divide the design and development tasks into 2 week segments.

The client gets access to view the progress of a task’s timeline and interact with UI Farm, for an open and quicker collaboration on the designs and website development. This is achieved through Atlassian’s Confluence tool. This can be used to collaborate on documents such as specifications and requirements within projects and tasks.

### Version Control

[Git](https://en.wikipedia.org/wiki/Git_(software)) is used for the code repository and version control. Every commit includes a detailed comment, and it’s linked to a specific project task on JIRA: this ensures *full traceability and easy rollback* in case something needs to be changed. This also allows the developers to review each others’ code, and suggest improvements.

### Hybrid Roles

At UI Farm the role of UX designer and UI developer are:

- Hybrid
- With less separation between roles

The designer and developer work together to create a fully responsive HTML/CSS prototype that provides multiple benefits.

### Agile iterations

{% include pattern-figure.html image="/assets/images/uif-article/09_no-loops.png" alt="No bottlenecks, no negative loops" width="330" height="330" %}

Evolve and remove time-consuming bottlenecks, by turning indefinite loops into time-defined agile iterations.

### Design Sustainably

Avoid expensive, non-interactive mockups by designing sustainable reusable prototypes.

## The New Sprint-Based Workflow

{% include pattern-figure.html image="/assets/images/uif-article/10_new-sprint-based-method.png" alt="A new sprint-based methodology" width="1182" height="457" %}

### Sprint 1: UX Analysis

After agreeing the functional requirements and specifications for the site, the UX designers will undertake sketching of the page templates.

### Sprint 2 & 3: Wireframe

Based on the UX analysis and sketches, designers and developers start creating the wireframes, *directly in the browser*.

Major benefits:

- The client can see the wireframes via a live URL
- The wireframe is a real HTML/CSS responsive prototype
- The prototype runs on any device, on any browser
- By keeping a separate URL for each version, the client can see the progress

Even at this early stage, the client can see **how the site will interact with the user** and how the flow of the product works.

{% include pattern-figure.html image="/assets/images/uif-article/11_positive-loop.png" alt="A positive loop" caption="A positive loop" width="340" height="348" %}

### Sprint 4 & 5: Skin

Traditionally, the next step would be for the visual designer to create static designs for each page, in applications like Adobe Photoshop.

At UI Farm we don’t use such tools to design responsive websites as they can’t reflect the fluid, non-static nature of the multi-device web.

With visual designers and developers working together, UI Farm take the interactive responsive wireframe and apply the design patterns on top, through **the web’s natural language tools**: HTML5, SASS (CSS3) and Javascript.

We then engage the visual designers when we need graphical elements for a design pattern, using tools like Sketch or Adobe Illustrator.

### User Testings

One huge advantage with UI Farm’s agile new workflow is the possibility to add user testing sessions into each Agile sprint.

Clients can do usability tests starting from the wireframe version, as it is a real web product already, responsive and running on all devices. It doesn’t take a long time to reach this phase, and this is why UI Farm’s new workflow is making the usability tests doable even for low budgeted projects.

{% include pattern-figure.html image="/assets/images/uif-article/12_positive-loop-user-testing.png" alt="Positive loops: user testing" caption="Positive loops: user testing" width="258" height="298" %}

It is also very easy to apply changes for subsequent rounds of tests, and even possible to apply changes *between* a usability test and the next one. Finally, A/B tests can be easily arranged, before or after the project is live. Clients can test the usability of *the very same HTML product*, and watch it evolve through subsequent tests and improvements from the feedback. The tested product throughout all of the different phases, is the one that eventually makes it to production.

### Even More Advantages

- Client changes are a lot quicker than changing static image files
- Having the designers and developers working closely, it’s easy for them to identify potential design pitfalls up-front

This stage is a *true collaborative effort* until the client is happy with the end result.

### Sprint 6: Quality Assurance

UI Farm adheres strictly to industry web coding standards.

- Valid HTML and CSS, verified by W3C
- Conform to ARIA Accessibility rules
- Complying with all priority 1, 2, and 3 guidelines of the W3C Web Content Accessibility Guidelines (WCAG)
- Ensuring that a contrast ratio of 4.5:1 and higher (ideally 7:1) exists between background and foreground items

### Performance

As stated by Brad Frost in his post [Prioritizing Performance In Responsive Design](http://bradfrostweb.com/blog/post/prioritizing-performance-in-responsive-design/), citing a [research by Guy Podjarny](http://www.guypo.com/rwd-ratio-in-top-100000-websites-refined/): 

> **86% of responsive sites** send about the same hefty payload to small screens as they do to large screens. 

In other words, mobile users are downloading desktop-sized sites.

UI Farm look at **performance as a major feature implemented by default**, and not treated as an afterthought. During the Quality Assurance Agile sprint, UI Farm run several benchmarks, implementing all of the performance improvements, to serve the best experience to all the different devices.

Starting from the first design phase, UI Farm run a series of tools, like [sitespeed.io](http://sitespeed.io/), to make sure the pages are working at their best on all the devices.

All the results are documented on Confluence.

### DRY, or Don’t Repeat Yourself

UI Farm implemented a strong DRY strategy, essentially based on an object-oriented approach to both the Javascript and the [SASS](http://sass-lang.com/), loading the right asset for the right device, heavily reducing the number of scripts and the amount of code necessary to render all the single design objects. UI Farm’s implementation of responsive images is a great addendum to this approach.

### Testing

UI Farm perform functional, interface, usability, compatibility, accessibility and performance testing on all pages against our defined browser list.

- All functional tests will be tested against the requirements agreed by both parties at the start of the project
- All testing documentation will be made available on Confluence

### Deployment

As UI Farm are now designing directly into the browser, we already have the final HTML/CSS/JS responsive site. No further front-end development is needed.

UI Farm use the ultra-efficient Ruby’s [Capistrano](http://capistranorb.com/) to quickly deploy websites through [SSH](https://en.wikipedia.org/wiki/Secure_Shell) and Git, keeping any staging and production releases properly separate. Through Capistrano’s multi-releases feature, UI Farm can quickly roll-back to a previous version, in case something needs to be reverted.

## A Case Study: UniCredit Responsive Landing Pages

UniCredit, a leading European bank, hired UI Farm to re-design and develop their Online Acquisition landing pages, currently desktop-only. UniCredit required a strong eye on accessibility, usability, and a clean and modern design, optimised for great performance on all modern devices.

After the UX analysis, the client agreed with UI Farm to perform an optimisation of the content, prioritising it for a responsive re-design and the best performance.

### First Iteration: Responsive Wireframe In The Browser

{% include pattern-figure.html image="/assets/images/uif-article/13_responsive-wireframe-in-the-browser.jpg" alt="Responsive wireframe in the browser" width="1176" height="688" %}

UI Farm started designing in the browser, using a custom version of their [multi-device framework](https://web.archive.org/web/20161021070205/http://uifarm.co.uk/responsifarm-powerful-bespoke-solution-for-your-website/). The mobile-first approach outlined the results of the content strategy analysis, so the first step was adding the real content to the correct markup wrapped in a solid HTML5 structure. Although no images or complex functionality were added at this stage, the resultant wireframe was a fully working HTML5/CSS3/Javascript greyscale website, multi-device compliant and ready for a first round of usability tests. [ARIA](https://www.w3.org/WAI/intro/aria) accessibility features were added at this stage as well.

The wireframe kept its own staging URL throughout the development of the successive iterations, so the client could go back to check the progress of each phase.

### Second Iteration: Skin

{% include pattern-figure.html image="/assets/images/uif-article/14_second-iteration-skin.jpg" alt="Second iteration: skin" width="1176" height="688" %}

Once the client was happy with the content-structured wireframe, UI Farm applied the first skin. Since the codebase is the same as the wireframe’s, the designers and the developers just continued to work, improving and adding depth, colours and images and always following the company’s brand guidelines. At this stage, the larger screens viewports gained some more specific details, while during the first iteration it was still showing the “mobile-first” approach.

During this iteration, UI Farm discussed with the client all of the potential design and performance improvements to apply to the pages. The discussion kept going in parallel with the active development, so that it was possible to experiment with some of the ideas directly on the site, test the results, discard what wasn’t working, or keep the rest for the next iteration.

### Third Iteration: Improvements From The Feedback

{% include pattern-figure.html image="/assets/images/uif-article/15_third-iteration-improvements-feedback.jpg" alt="Third iteration: improvements from the feedback" width="1176" height="688" %}

The third iteration included:

- modern full-screen imagery
- custom typography
- functionality for touch enabled devices
- a sticky header that changes whether the main call to actions are visible or not
- social networks integration
- many more performance improvements, such as [conditional loading](https://adactio.com/journal/5414).

This is the final codebase iteration, meaning the same pages had undertaken several phases, going from a greyscale wireframe to a full-fledged web product while maintaining the same repository and a consistent look & feel. The client was free to perform *full-scaled usability tests over different stages of the same website*, without worrying about the non-real feel of static mockups and prototypes.

A final word for the **great efficiency and sustainability** of having a product that’s evolving without changing its nature: there are no static JPEGs to be churned into HTML/CSS pages by two different teams. Everyone can relate to the money-saving argument.

## A/B Tests

UniCredit performed A/B tests on the new landing pages, which proved successful for all mobile devices against the former desktop-only version.

> UI Farm’s innovative workflow and unique skills has given us a very clear insight into our customers’ behaviour and preferences, which has considerably boosted our account application conversions.<br>
> Thanks to UI Farm’s approach, we have been able to significantly improve the experience delivered to our customers and prospects, and make changes that may have seemed minor to us but have resulted in significant conversion lifts. UI Farm has truly changed our approach to Interaction Design.
> <cite>—Gabriele Rosati, Head of Interaction Design at UniCredit</cite>

# Conclusion

UI Farm strongly believes that the new era of multi-device web should massively gain from technologies like responsive web design, and a more **sustainable workflow** as outlined. To achieve this, new methods and a more focussed effort on features previously considered minor, need to be used. Or invented. Or both.

—

<small>This post was originally published on Medium.</small>