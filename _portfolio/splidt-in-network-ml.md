---
title: "SpliDT: Partitioned Decision Trees for Line-Rate ML Inference"
excerpt: "ML models (One-class SVMs, Random Forest, Isolation Forest) for payload-level anomaly detection and malicious traffic classification on programmable PISA switches."
collection: portfolio
date: 2025-09-01
period: "Jan 2024 – Aug 2025"
affiliation: "Purdue · NextGArch Lab"
image: /images/research/splidt-tree.png
image_alt: "Diagram from the SpliDT poster: a decision tree partitioned into subtrees p1–p4, each using its own window of packets w1–w4."
summary: "Detecting malicious network traffic with ML models that run at line rate on programmable switches."
venue_tags:
  - label: "SRC TECHCON ’25"
    kind: talks
links:
  - label: Poster
    url: /files/SpliDT_MarilynRego_poster.pdf
---

- Implemented and benchmarked one-class SVMs, random forests, and isolation forests for payload-level anomaly detection, establishing baselines for accuracy, cost, and scalability.
- Analyzed how packet-, flow-, and connection-level payload features trade off prediction accuracy against computational overhead.
- Explored transformer-based models to automate payload feature selection, comparing them against traditional methods integrated with SNORT.
