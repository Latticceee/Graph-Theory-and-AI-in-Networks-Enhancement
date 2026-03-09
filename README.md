# Graph Neural Network for Spanning Tree Approximation in Electric Networks

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/#fileId=https%3A//storage.googleapis.com/kaggle-colab-exported-notebooks/omarsaidlatticceee/graph-theory-ai-in-networks-enhancement-code.09401d0d-c093-4482-87d2-1cb895b6fd7c.ipynb%3FX-Goog-Algorithm%3DGOOG4-RSA-SHA256%26X-Goog-Credential%3Dgcp-kaggle-com%2540kaggle-161607.iam.gserviceaccount.com/20260303/auto/storage/goog4_request%26X-Goog-Date%3D20260303T144307Z%26X-Goog-Expires%3D259200%26X-Goog-SignedHeaders%3Dhost%26X-Goog-Signature%3D6527b13bee90dd34845edbc71ceb8d025738096cf990453ef2ceb9c934c0a820da8cad0665a2b8f6aef26f65c215b59654fe799db237b9847e3cfc440ab5212940430e7b78ed0889808ce11e90efdb5c37ef68abb346b1e453d5955ff0ef39ca3bb7aad65e429c6cedeaa951d56747cbdc4bac472a599a37bc4fed559891519a27420d457728e2a622895c3dc89b4276270e8fafc597136bb1acd92c4ac67ff074ce5f6d6fb48d0cfa6e47e790098d8f658035cce9229363063b444532b11dd9ead422804de20815f814308e20c67d9bb72ed67aa8afc928acdbfd9f26b359a72da6f0e8bc4112c15f09414f900d4c2ac00de1382acfbfb9acd1be773575482c)

You can access the project's poster through the following link: (https://drive.google.com/file/d/1Zm3Q954yRdaspiHClpllby9uh1Wu9IaW/view?usp=sharing)

## Abstract
This repository implements a Graph Neural Network (GNN) architecture designed to approximate the number of spanning trees (network complexity) within large-scale graphs. Exact analytical computation of spanning trees via Kirchhoff's Matrix-Tree Theorem requires evaluating the cofactor of the graph's Laplacian matrix, an operation strictly bounded by $\mathcal{O}(n^3)$ time complexity. This project introduces a machine learning approximation that mitigates this computational bottleneck, achieving high predictive accuracy while shifting the computational load from cubic time evaluation to highly parallelizable, low-latency forward passes.

## Application: Power Grid Topology Optimization
The model's utility is demonstrated through case studies on real-world electric power grid topologies. Because the number of spanning trees serves as a robust proxy for network reliability and redundancy, rapid estimation allows for real-time topological analysis. This framework enables infrastructure engineers to dynamically simulate edge additions/deletions and identify optimal network configurations, facilitating resilience enhancements against cascading failures without the prohibitive latency of algebraic graph methods.

## 🏆 Academic Recognition
* **1st Place, Mathematics Category** - 2026 Bibliotheca Alexandrina Science & Engineering Fair (BASEF)

## Repository Contents
* `Graph_Theory_&_AI_in_Networks_Enhancement_Code.ipynb`: The core implementation, including graph data preprocessing, GNN model architecture, training loops, and empirical validation against exact Laplacian determinant calculations.

## Key Contributions
* **Algorithmic Efficiency:** Bypasses the $\mathcal{O}(n^3)$ limits of exact mathematical calculation, enabling scalable analysis of massive network structures.
* **High-Fidelity Approximation:** Maintains rigorous empirical consistency with theoretical spanning tree counts, demonstrating minimal divergence from exact analytical solutions across tested topologies.
