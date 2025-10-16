---
title: "Dynamo: Predictive Modeling of Single-Cell Dynamics"
excerpt: "Contributing to an open-source framework for RNA velocity vector field analysis and predictive modeling of cell fate transitions (472★ on GitHub).<br/><img src='/images/dynamo-preview.png' style='max-width: 500px;'>"
collection: portfolio
---

## Project Overview

**Dynamo** is a comprehensive computational framework for modeling single-cell transcriptomic dynamics through RNA velocity vector field analysis. As an open-source contributor to this project, I helped enhance the framework's compatibility, performance, and usability for the broader single-cell genomics community.

🔗 **GitHub Repository**: [aristoteleo/dynamo-release](https://github.com/aristoteleo/dynamo-release) (472★)

## Scientific Background

### The Challenge
Understanding how cells transition between states during development, differentiation, and disease requires modeling the continuous dynamics underlying discrete single-cell measurements. Traditional trajectory inference methods provide static snapshots, but cannot predict future cell states or the effects of perturbations.

### The Solution
Dynamo learns continuous **vector fields** from RNA velocity data, enabling:
- Prediction of cell fate trajectories
- Identification of critical transition points (attractors, saddle points)
- In silico genetic perturbation experiments
- Optimal reprogramming path discovery

## Technical Framework

### Core Capabilities

1. **RNA Velocity Estimation**
   - Moment-based velocity calculation
   - Metabolic labeling integration (scSLAM-seq, scNT-seq)
   - Uncertainty quantification

2. **Vector Field Learning**
   - Continuous velocity field reconstruction from sparse measurements
   - Differential geometry analysis of cell state space
   - Identification of fixed points and bifurcations

3. **Predictive Modeling**
   - Cell fate prediction along learned trajectories
   - Optimal reprogramming path computation
   - In silico genetic perturbation simulation

4. **Visualization & Analysis**
   - Phase portrait generation
   - Streamline plots for trajectory visualization
   - Heatmaps for spatiotemporal gene expression

## My Contributions

### Software Engineering
- **Compatibility Enhancement**: Resolved critical import and dependency issues for AnnData ≥0.10, enabling broader user adoption
- **Performance Optimization**: Improved data preprocessing pipelines for large-scale datasets
- **Code Quality**: Enhanced documentation, testing, and error handling

### Scientific Development
- **Visualization Modules**: Optimized trajectory inference and phase portrait generation
- **Data Integration**: Improved methods for integrating multi-modal single-cell data
- **User Experience**: Streamlined workflows for common analysis tasks

## Applications

### Developmental Biology
- Modeling cell fate decisions during embryogenesis
- Understanding lineage commitment and specification
- Identifying critical developmental checkpoints

### Disease Modeling
- Investigating aberrant cell state transitions in cancer
- Modeling disease progression at single-cell resolution
- Identifying therapeutic intervention points

### Cellular Engineering
- Predicting optimal reprogramming strategies (iPSC generation)
- Designing directed differentiation protocols
- Screening genetic perturbations in silico

## Technical Stack

- **Language**: Python 3.8+
- **Core Dependencies**: NumPy, SciPy, Pandas, AnnData, Scanpy
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Performance**: Numba JIT compilation, GPU acceleration (optional)
- **Integration**: Compatible with Scanpy ecosystem

## Key Publications

- **Zeng, Z., et al. (including Cao, N.)** (2025). "Predictive Modeling of Single Cell Transcriptomic Dynamics with Dynamo." *Nature Protocols*, under review.

## Impact & Community

- **472 GitHub Stars**: Widely adopted in single-cell genomics community
- **Active Development**: Regular updates and feature additions
- **Collaborative**: Open to community contributions and feedback
- **Educational**: Comprehensive tutorials and documentation

## Example Use Cases

1. **Hematopoiesis Modeling**: Reconstructing blood cell differentiation trajectories
2. **Neural Development**: Predicting neuronal fate decisions
3. **Cardiac Development**: Modeling heart progenitor cell transitions (my focus area)
4. **Cancer Evolution**: Understanding tumor cell state dynamics

## Future Directions

- Integration with spatial transcriptomics (Spateo framework)
- Multi-omic data integration (RNA + protein + chromatin)
- Causal inference for perturbation prediction
- Real-time analysis for live-cell imaging data

---

**Duration**: August 2025 - Present  
**Role**: Open-Source Contributor  
**Lab**: [Qiu Lab](https://www.devo-evo.com/), Department of Genetics & Computer Science, Stanford University  
**Project Lead**: [Professor Xiaojie Qiu](https://med.stanford.edu/profiles/xiaojie-qiu)  
**Repository**: [github.com/aristoteleo/dynamo-release](https://github.com/aristoteleo/dynamo-release)
