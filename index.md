---
layout: default
title: "Daily Health Picks — Honest Supplement Reviews"
description: "Research-backed reviews of the best health supplements for immunity, energy, and overall wellbeing."
---

<div class="hero">
  <h1>Honest Health Supplement Reviews</h1>
  <p>We research the science, read the reviews, and cut through the marketing — so you know exactly what's worth buying.</p>
</div>

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    {% if post.description %}<p class="excerpt">{{ post.description }}</p>{% endif %}
    <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
  </li>
  {% endfor %}
</ul>
