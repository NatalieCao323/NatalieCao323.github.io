---
title: "Predictive Modeling of Single Cell Transcriptomic Dynamics with Dynamo"
collection: publications
permalink: /publication/2025-dynamo-protocols
excerpt: 'A comprehensive protocol for RNA velocity vector field learning, differential geometry analyses, and predictive modeling of cell fate transitions including optimal reprogramming and in silico genetic perturbation predictions.'
date: 2099-02-01
venue: 'Nature Protocols (under review)'
citation: 'Zeng, Z., Yu, S., Ni, K., Zhang, Y., Shin, U., Huang, C., Cao, N., Weissman, J., Xing, J., & Qiu, X. (under review). &quot;Predictive Modeling of Single Cell Transcriptomic Dynamics with Dynamo.&quot; <i>Nature Protocols</i>.'
---

## Abstract

This protocol presents **Dynamo**, a comprehensive computational framework for modeling single-cell transcriptomic dynamics through RNA velocity vector field analysis. We provide detailed methods for reconstructing continuous vector fields from discrete single-cell measurements, performing differential geometry analyses to identify critical cell state transitions, and making non-trivial predictions including optimal reprogramming paths and in silico genetic perturbation outcomes.

## Key Features

- **RNA Velocity Vector Fields**: General framework for learning continuous velocity fields from sparse single-cell RNA-seq data
- **Differential Geometry Analysis**: Mathematical tools for identifying attractors, saddle points, and bifurcations in cell state space
- **Predictive Modeling**: Algorithms for predicting optimal reprogramming strategies and genetic perturbation effects
- **Trajectory Inference**: Advanced methods for reconstructing developmental and differentiation trajectories
- **Visualization Tools**: Comprehensive suite for phase portrait generation and trajectory visualization

## Applications

- Cell fate decision analysis during development
- Optimal reprogramming path prediction for cellular engineering
- In silico genetic perturbation screening
- Disease mechanism investigation through trajectory perturbation
- Drug response prediction in single-cell contexts

## Computational Tools

- Python package: `dynamo-release` (472★ on GitHub)
- Compatible with AnnData ≥0.10
- Integration with Scanpy ecosystem
- GPU-accelerated computation for large-scale datasets

## My Contributions

- Enhanced model compatibility with modern single-cell data formats
- Improved data preprocessing and visualization modules
- Optimized trajectory inference algorithms for large-scale datasets
- Documentation and testing for broader user adoption

## Status

Manuscript under review at *Nature Protocols*.

**Authors**: Zehua Zeng, Sichao Yu, Ke Ni, Yan Zhang, Ukyeon Shin, Cinlong Huang, Natalie Cao, Jonathan Weissman, Jianhua Xing, Xiaojie Qiu

**Corresponding Author**: Xiaojie Qiu, Department of Genetics & Computer Science, Stanford University
