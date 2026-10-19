---
title: "Communication-Efficient Cross-Region LLM Inference"
excerpt: "Communication-efficient systems for cross-region LLM inference through hardware–software co-design across geographically distributed data centers."
collection: portfolio
date: 2026-07-01
period: "Aug 2025 – Present"
affiliation: "University of Michigan · SRC Research Scholars Program"
image: /images/research/mrllm-wan.png
image_alt: "Diagram from the mrLLM poster: an LLM split across Region A and Region B, with large intermediate activations crossing a bandwidth-limited WAN link."
summary: "Building communication-efficient systems for LLM inference across geographically distributed data centers, through hardware–software co-design."
outputs:
  - title: "mrLLM: Fast Multi-Region LLM Inference Using Learned Adapters"
    tag:
      label: "NSDI ’26 poster"
      kind: talks
    links:
      - label: Poster
        url: /files/mrLLM_poster.pdf
  - title: "Towards Network-Efficient Cross-Regional Inference via Learned Activation Compression"
    tag:
      label: "NAIC @ SIGCOMM ’26"
      kind: workshops
    links:
      - label: Paper
        url: https://doi.org/10.1145/3789240.3828744
---

- Designing learned activation-compression techniques and adapter-based methods to reduce cross-region data movement while preserving model quality.
- Evaluating partitioning strategies for prefill, decode, and agentic inference workloads across latency, throughput, data movement, and model quality under heterogeneous compute and network constraints.
