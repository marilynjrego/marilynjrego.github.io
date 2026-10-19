---
title: "SpliDT: Partitioned Decision Trees for Line-Rate ML Inference"
excerpt: "ML models (One-class SVMs, Random Forest, Isolation Forest) for payload-level anomaly detection and malicious traffic classification on programmable PISA switches."
collection: portfolio
date: 2025-09-01
---

At Purdue's NextGArch Lab, I worked on machine learning models for network classification on PISA (Protocol Independent Switch Architecture) switches. I implemented and benchmarked classification models — One-class SVMs, Random Forest, and Isolation Forest — for anomaly detection at the application payload level, establishing baseline metrics for accuracy, computational cost, and scalability. I analyzed how packet-level, flow-level, and connection-level payload features affect malicious traffic classification, weighing prediction accuracy against computational overhead, and explored transformer-based models to automate feature selection for application payloads, comparing them against traditional methods integrated with SNORT.

This work, SpliDT, partitions decision trees to enable scalable, stateful ML inference at line rate, and was presented as a talk and poster at SRC TECHCON 2025.
