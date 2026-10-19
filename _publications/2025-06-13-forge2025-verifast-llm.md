---
title: "Evaluating the Ability of GPT-4o to Generate Verifiable Specifications in VeriFast"
collection: publications
category: conferences
permalink: /publication/2025-06-13-forge2025-verifast-llm
excerpt: 'We evaluate how well GPT-4o generates fully accurate, verifiable specifications for the VeriFast static verifier, using prompt engineering, chain-of-thought, prompt chaining, and few-shot prompting.'
date: 2025-04-27
venue: 'IEEE/ACM FORGE 2025, co-located with ICSE 2025'
venue_short: "FORGE ’25"
authors: '**Marilyn Rego**\*, Wen Fan\*, Xin Hu, Sanya Dod, Zhaorui Ni, Danning Xie, Jenna DiVincenzo, Lin Tan (\*equal contribution)'
links:
  - label: Paper
    url: https://doi.org/10.1109/Forge66646.2025.00035
  - label: arXiv
    url: https://arxiv.org/abs/2411.02318
  - label: BibTeX
    url: /files/bibtex/rego2025forge.bib
paperurl: 'https://ieeexplore.ieee.org/document/11052787'
bibtexurl: '/files/bibtex/rego2025forge.bib'
citation: '<b>Marilyn Rego</b>*, Wen Fan*, Xin Hu, Sanya Dod, Zhaorui Ni, Danning Xie, Jenna DiVincenzo, Lin Tan. (2025). &quot;Evaluating the Ability of GPT-4o to Generate Verifiable Specifications in VeriFast.&quot; <i>2025 IEEE/ACM Second International Conference on AI Foundation Models and Software Engineering (FORGE)</i>.'
---

Static verification tools like VeriFast require developers to hand-write formal specifications, which is a major barrier to adoption. This paper evaluates whether GPT-4o can generate fully accurate specifications that VeriFast can verify, progressing from baseline prompt engineering to chain-of-thought (CoT) reasoning, prompt chaining, and few-shot prompting. We categorized the VeriFast benchmark suite, built tailored input datasets for testing, and designed a qualitative analysis methodology to assess output correctness, syntactic validity, and model failure modes — offering an early look at how far off-the-shelf LLMs are from generating machine-checkable proofs.
