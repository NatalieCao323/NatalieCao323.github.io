---
title: "3D Reconstruction of the Spatial Transcriptomics with Neural Field"
collection: publications
permalink: /publication/2025-neural-field-3d
excerpt: 'A differentiable framework for reconstructing 3D embryonic structures from 2D spatial transcriptomic slices using neural field models with Transformer-based positional encodings and VAE modules.'
date: 2025-03-01
venue: 'Nature Biotechnology (in preparation)'
citation: 'Lu, Y., Cao, N., & Qiu, X. (2025). &quot;3D Reconstruction of the Spatial Transcriptomics with Neural Field.&quot; To be submitted to <i>Nature Biotechnology</i>.'
---

## Abstract

We present **neural_field**, a novel differentiable framework for reconstructing three-dimensional embryonic structures from sequential two-dimensional spatial transcriptomic slices. By leveraging neural field representations combined with Transformer-based positional encodings and variational autoencoder (VAE) modules, our method achieves superior alignment accuracy and training stability on large-scale Stereo-seq datasets from human and mouse embryos.

## Key Contributions

- **Novel Architecture**: Integration of neural fields with Transformer-based spatial encodings for capturing nonlinear spatial relationships across tissue slices
- **Enhanced Stability**: Improved algorithmic stability and loss smoothness through advanced optimization techniques
- **Biological Insights**: Analysis of spatiotemporal gene regulation and signaling dynamics underlying organogenesis
- **Disease Applications**: Revealed patterns relevant to understanding congenital diseases through 3D reconstruction of developmental processes

## Methods & Tools

- Neural field models for continuous 3D representation
- Transformer-based positional encodings for spatial alignment
- Variational autoencoders (VAE) for latent space learning
- PyTorch implementation with GPU acceleration
- Validation on Stereo-seq datasets (human and mouse embryos)

## Status

Manuscript in preparation for submission to *Nature Biotechnology*.

**Authors**: Yifan Lu, Natalie Cao, Xiaojie Qiu  
**Affiliation**: Department of Genetics & Computer Science, Stanford University
