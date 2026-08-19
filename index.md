---
layout: default
title: Home
description: Practical notes on building better digital systems.
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">MiFix LLC / Field notes</p>
    <h1>Make the complex <em>clear.</em></h1>
    <p class="hero-lede">A working journal about thoughtful technology, useful systems, and the details that make digital products feel human.</p>
    <a class="text-link" href="#latest">Read the latest <span aria-hidden="true">↓</span></a>
  </div>
  <div class="hero-art" aria-hidden="true">
    <div class="art-orbit orbit-one"></div>
    <div class="art-orbit orbit-two"></div>
    <div class="art-core">M<span>+</span></div>
    <div class="art-label label-top">EST. 2024</div>
    <div class="art-label label-bottom">SYSTEMS / PEOPLE / PROGRESS</div>
  </div>
</section>

<section class="latest-section" id="latest">
  <div class="section-heading">
    <p class="eyebrow">The archive</p>
    <h2>Latest notes</h2>
  </div>
  <div class="post-list">
    {% for post in site.posts %}
      <a class="post-card" href="{{ post.url | relative_url }}">
        <div class="post-meta"><span>{{ post.category | default: "Field notes" }}</span><span>{{ post.date | date: "%b %-d, %Y" }}</span></div>
        <h3>{{ post.title }}</h3>
        <p>{{ post.description }}</p>
        <span class="post-arrow" aria-hidden="true">↗</span>
      </a>
    {% else %}
      <p class="empty-state">New notes are on the way.</p>
    {% endfor %}
  </div>
</section>

<section class="about-section" id="about">
  <div class="about-number">01</div>
  <div>
    <p class="eyebrow">A little context</p>
    <h2>Technology should earn its place.</h2>
    <p>MiFix LLC helps turn fuzzy ideas into dependable, maintainable software. This is where we share the principles, patterns, and lessons we pick up along the way.</p>
  </div>
</section>