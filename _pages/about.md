---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
Hi, this is Marilyn! I'm a Ph.D. student in Computer Science and Engineering at the [University of Michigan](https://cse.engin.umich.edu/), advised by [Muhammad Shahbaz](https://gitlab.com/mshahbaz/mshahbaz.gitlab.io/-/wikis/home).

My research sits at the intersection of machine learning and computer systems. I'm interested in building the infrastructure behind large-scale AI, with a focus on distributed AI systems, heterogeneous computing, LLM inference systems, and hardware–software co-design. As an SRC Research Scholar, I'm currently working on communication-efficient systems for cross-region LLM inference across geographically distributed data centers.

Before Michigan, I completed my undergrad in Computer Science at Purdue. In Summer 2026, I was a Research Scientist/Engineer Intern at Adobe, where I built CPU–GPU profiling infrastructure for multi-process and multi-node LLM inference workloads.

Outside of research, I enjoy traveling, trying new food, and painting.

Feel free to browse my [publications](/publications/), [talks](/talks/), or [CV](/files/CV.pdf) or feel free to reach out if you'd like to [connect](/contact/)!

## News

<ol class="news-timeline">
{% for item in site.data.news %}
  <li class="news-timeline__item">
    <span class="news-timeline__date">{{ item.date }}</span>
    <div class="news-timeline__text">{{ item.text | markdownify }}</div>
  </li>
{% endfor %}
</ol>

## Honors & Awards

- Adobe Research Code Quality Jam – Robustness Category Winner, 2026
- Elected Member, [Tau Beta Pi](https://www.tbp.org/home.cfm) Engineering Honor Society (University of Michigan chapter), 2026
- USENIX NSDI Student Grant Awards, 2025 and 2026
- First-Year CSE PhD Rackham Fellowship, 2025
- Purdue College of Science Dean's List and Semester Honors, 2021–2025

## Service

- Judge, University of Michigan Undergraduate Research Symposium, 2026
