---
title: "Teaching & Mentoring"
permalink: /teaching/
author_profile: true
---

{% include base_path %}

<div class="entry-list">
  {% assign teaching_items = site.teaching | sort: 'date' | reverse %}
  {% for item in teaching_items %}
    <article class="entry-item">
      <h2 class="entry-item__title">{{ item.title }}</h2>
      <p class="entry-item__date">{{ item.date | date: "%B %Y" }} &middot; {{ item.type }}, {{ item.venue }}, {{ item.location }}</p>
      <input type="checkbox" id="teaching-toggle-{{ forloop.index }}" class="entry-item__toggle-checkbox">
      <div class="entry-item__body">
        {{ item.content }}
      </div>
      <label for="teaching-toggle-{{ forloop.index }}" class="entry-item__toggle-label">
        <span class="entry-item__label-more">Show more</span>
        <span class="entry-item__label-less">Show less</span>
      </label>
    </article>
  {% endfor %}
</div>
