---
title: "Neural Field: 3D Embryo Reconstruction from Spatial Transcriptomics"
excerpt: "Developing a differentiable framework for reconstructing 3D embryonic structures from 2D spatial transcriptomic slices using neural fields and Transformer-based encodings.<br/><img src='/images/neural-field-preview.png' style='max-width: 500px;'>"
collection: portfolio
---

## Project Overview

**Neural Field** is an open-source framework for reconstructing three-dimensional embryonic structures from sequential two-dimensional spatial transcriptomic slices. This project addresses a fundamental challenge in developmental biology: how to computationally integrate discrete 2D tissue sections into continuous 3D representations that preserve both spatial relationships and gene expression patterns.

## Research Context

Understanding embryonic development requires analyzing how cells organize in three-dimensional space and how gene expression varies across tissues. Modern spatial transcriptomics technologies like Stereo-seq can capture gene expression at subcellular resolution, but typically only in 2D slices. Our framework bridges this gap by learning continuous 3D representations from these discrete measurements.

## Technical Approach

### Neural Field Architecture
- **Continuous Representation**: Neural networks that map 3D coordinates to gene expression values, enabling smooth interpolation between slices
- **Transformer-Based Positional Encodings**: Advanced spatial encodings that capture nonlinear relationships across tissue sections
- **Variational Autoencoder (VAE) Integration**: Latent space learning for dimensionality reduction and noise robustness

### Key Innovations
1. **Enhanced Algorithmic Stability**: Improved optimization techniques that ensure smooth convergence during training
2. **Improved Slice Alignment**: Transformer encodings that better capture spatial correspondences between adjacent slices
3. **Scalability**: Efficient implementation enabling reconstruction of large-scale embryo datasets

## Datasets & Validation

- **Human Embryo Data**: Stereo-seq datasets capturing early organogenesis
- **Mouse Embryo Data**: High-resolution developmental time series
- **Validation Metrics**: Alignment accuracy, reconstruction fidelity, biological plausibility

## Biological Insights

Through 3D reconstruction, we can:
- Reveal spatiotemporal gene regulation patterns during organogenesis
- Identify signaling gradients and morphogen dynamics
- Understand cell-cell communication in 3D tissue context
- Investigate mechanisms underlying congenital diseases

## My Contributions

- Integrated Transformer-based positional encodings into the neural field architecture
- Enhanced training stability through advanced optimization techniques
- Conducted large-scale experiments on human and mouse embryo datasets
- Improved model robustness and alignment accuracy
- Contributed to manuscript preparation for Nature Biotechnology

## Tools & Technologies

- **Framework**: PyTorch
- **Visualization**: Biorender, Matplotlib, Plotly
- **Data Processing**: AnnData, Scanpy
- **Computational Resources**: Stanford GPU clusters

## Status

- **Code**: Private GitHub repository (`aristoteleo/neural_field`)
- **Manuscript**: In preparation for Nature Biotechnology
- **Collaborators**: Yifan Lu, Professor Xiaojie Qiu (Qiu Lab, Stanford)

## Future Directions

- Integration with imaging modalities (microscopy, histology)
- Temporal modeling across developmental stages
- Multi-species comparative analysis
- Application to disease modeling and drug screening

---

**Duration**: September 2025 - Present  
**Lab**: [Qiu Lab](https://www.devo-evo.com/), Department of Genetics & Computer Science, Stanford University  
**Advisor**: [Professor Xiaojie Qiu](https://med.stanford.edu/profiles/xiaojie-qiu)
