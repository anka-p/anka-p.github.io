---
layout: default
title: Hijibiji
permalink: /hijibiji/
---

<div class="gallery-grid">
  {% for hijibiji in site.hijibiji %}
    <a href="{{ hijibiji.url | relative_url }}" class="gallery-item">
      <img src="{{ hijibiji.image | relative_url }}" alt="{{ hijibiji.title }}">
      <div class="gallery-overlay">
        <h3>{{ hijibiji.title }}</h3>
        <p>{{ hijibiji.description }} </p>
      </div>
    </a>
  {% endfor %}
</div>