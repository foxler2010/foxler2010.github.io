---
title: "Home"
layout: splash
permalink: /
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/main-splash.jpg
  actions:
    - label: "Check it out"
      url: "https://foxler2010.github.io/blog"
  caption: "[Photo credit: Mary Ray/Unsplash](https://unsplash.com/@mary_ray)"
excerpt: "Hey. I'm Drew, and this is my blog"
intro: 
  - excerpt: '# **Hardware & Projects**'
feature_row:
  - image_path: assets/images/raspberrypis-cropped.jpg
    alt: "My Raspberry Pis"
    title: "Raspberry Pis"
    excerpt: "I have three Raspberry Pi 4s, and one Raspberry Pi 3B+"
    url: "/projects/pis"
    btn_label: "Check it out"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "The server"
    title: "Server"
    excerpt: "I own a Dell PowerEdge R710 that I use for a lot of things,"
    url: "/projects/server"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-gallery-image-3-th.jpg
    alt: "The Minecraft title screen with Forge installed"
    title: "Coding"
    excerpt: "I know how to code in Java, and am currently working on coding my text-adventure game, Jump The Volcano."
feature_row2:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: ""
    title: ""
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Stupidity"
    excerpt: "I admit,  I am very dumb. Go learn more by reading these posts!"
    url: "/categories/#stupidity"
    btn_label: "Read more"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

{% include paginator.html %}
