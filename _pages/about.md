---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
Hi, I'm Marilyn! I'm a Ph.D. student in CSE at the [University of Michigan](https://cse.engin.umich.edu/), advised by [Muhammad Shahbaz](https://gitlab.com/mshahbaz/mshahbaz.gitlab.io/-/wikis/home). I build systems for large-scale AI — **distributed LLM inference**, **heterogeneous computing**, and **hardware–software co-design**.

Previously, I did my B.S. in Computer Science at Purdue and interned at Adobe as a Research Scientist/Engineer. Here's my [CV](/files/CV.pdf).

Outside of research, I enjoy traveling, trying new food, and painting.

## News

{% assign news_recent = 6 %}
<ol class="news-timeline">
{% for item in site.data.news limit: news_recent %}
  {% include news-item.html item=item %}
{% endfor %}
</ol>
{% if site.data.news.size > news_recent %}
<details class="news-older">
  <summary><span class="news-older__more">Show older news</span><span class="news-older__less">Hide older news</span></summary>
  <ol class="news-timeline">
  {% for item in site.data.news offset: news_recent %}
    {% include news-item.html item=item %}
  {% endfor %}
  </ol>
</details>
{% endif %}

## Honors & Awards

- Adobe Research Code Quality Jam – Robustness Category Winner, 2026
- Elected Member, [Tau Beta Pi](https://www.tbp.org/home.cfm) Engineering Honor Society (University of Michigan chapter), 2026
- USENIX NSDI Student Grant Awards, 2025 and 2026
- First-Year CSE PhD Rackham Fellowship, 2025
- Purdue College of Science Dean's List and Semester Honors, 2021–2025

## Service

- Judge, University of Michigan Undergraduate Research Symposium, 2026
