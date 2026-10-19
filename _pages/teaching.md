---
title: "Teaching & Mentoring"
permalink: /teaching/
author_profile: true
---

{% include base_path %}

<div class="entry-list">
  {% assign teaching_items = site.teaching | sort: 'date' | reverse %}
  {% for item in teaching_items %}
    {% capture meta %}{{ item.period }} · {{ item.venue }}{% endcapture %}
    {% include entry-item.html item=item meta=meta collapse=true id_prefix="teaching" index=forloop.index %}
  {% endfor %}
</div>
