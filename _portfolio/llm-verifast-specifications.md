---
title: "LLMs for Verifiable Specification Generation"
excerpt: "Evaluating how well GPT-4o generates fully accurate separation logic specifications for the VeriFast static verifier."
collection: portfolio
date: 2026-06-01
period: "May 2024 – Aug 2024"
affiliation: "Purdue · Summer Undergraduate Research Fellowship"
image: /images/research/verifast-listing.png
image_alt: "Listing 1 from the FORGE 2025 paper: a C increment function given to GPT-4o as input, and the output with VeriFast requires/ensures and open/close annotations."
summary: "Can LLMs write formal specifications that a static verifier (VeriFast) actually accepts?"
outputs:
  - title: "Evaluating the Ability of GPT-4o to Generate Verifiable Specifications in VeriFast"
    tag:
      label: "FORGE ’25"
      kind: conferences
    links:
      - label: Paper
        url: https://doi.org/10.1109/Forge66646.2025.00035
  - title: "An Empirical Study of LLM-Generated Specifications for VeriFast"
    tag:
      label: "ISSRE ’26"
      kind: conferences
    links:
      - label: Details
        url: /publications/#2026-06-01-issre-verifast-empirical-study
---

- Evaluated LLMs on generating separation logic specifications for VeriFast, from baseline prompting to chain-of-thought, prompt chaining, and few-shot prompting.
- Categorized the VeriFast benchmarks and built tailored input datasets for systematic evaluation.
- Designed a qualitative analysis framework for output correctness, syntactic validity, and model failure modes.
