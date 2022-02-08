---
layout: homepage
title: Isomer Site
description: Brief site description here
image: /images/isomer-logo.svg
permalink: /
notification: Here's a notification bar you can use!
sections:
  - hero:
      title: Hero titlZZZZ
      subtitle: Hero subtitle
      background: /images/hero-banner.png
      heroType: dropdown
      dropdown:
        title: ""
        options:
          - &a1
            title: Hero Dropdown Element Title
            url: ""
          - *a1
          - *a1
  - infobar:
      title: Infobar title
      subtitle: Subtitle
      description: About a sentence worth of description here
      button: Button text
      url: /faq/
---
