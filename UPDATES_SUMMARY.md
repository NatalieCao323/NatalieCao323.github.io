# Website Update Summary - CS+Bio PhD Application Focus

## Overview
Transformed the website from a business/MS&E focus to a computational biology research focus tailored for CS+Bio PhD applications, highlighting work in predictive modeling of embryonic development, spatial transcriptomics, and single-cell genomics.

## Major Changes

### 1. Site Configuration (`_config.yml`)
**Updated:**
- Site description: Now emphasizes computational biology and developmental genomics
- Author bio: "Computational Biology Researcher | Machine Learning + Developmental Genomics | Building Predictive Models of Embryonic Development"

### 2. About Page (`_pages/about.md`)
**Completely rewritten with:**
- Introduction highlighting work with Professor Xiaojie Qiu in computational developmental biology
- Research interests focused on:
  - Computational Developmental Biology (neural fields, graph neural networks, flow matching)
  - Spatial Transcriptomics & Single-Cell Genomics
  - Machine Learning Theory & Applications for biological systems
- Current research projects:
  - Virtual Embryo Framework (Nature Comment)
  - Neural Field for 3D Embryo Reconstruction
  - Dynamo: RNA Velocity & Vector Field Analysis
- Updated publications section with computational biology papers
- Research experience, professional experience, teaching, and technical skills

### 3. Navigation (`_data/navigation.yml`)
**Updated menu structure:**
- About
- Publications (new)
- Research (portfolio)
- Teaching
- CV

Removed: Entrepreneurship section

### 4. Publications (`_publications/`)
**Created new publication pages:**
1. `2025-virtual-embryo.md` - "Towards a Predictive Virtual Embryo with Genomics and AI" (Nature Methods, under review)
2. `2025-neural-field-3d.md` - "3D Reconstruction of the Spatial Transcriptomics with Neural Field" (Nature Biotechnology, in preparation)
3. `2025-dynamo-protocols.md` - "Predictive Modeling of Single Cell Transcriptomic Dynamics with Dynamo" (Nature Protocols, under review)
4. Updated `2009-10-01-paper-title-number-1.md` → IEEE EEBDA 2024 paper

**Removed:**
- Placeholder publications (2010, 2015)

### 5. Research Projects (`_portfolio/`)
**Created comprehensive project pages:**
1. `neural-field-embryo.md` - Neural Field: 3D Embryo Reconstruction from Spatial Transcriptomics
2. `dynamo-release.md` - Dynamo: Predictive Modeling of Single-Cell Dynamics (472★ GitHub)
3. `sentinel-nlp.md` - SENTINEL: AI-Generated Text Detection (CS 224N project)
4. `vrvo-reinforcement-learning.md` - VRVO: Variance-Regularized Value Optimization for RL

**Removed:**
- Placeholder portfolio items

### 6. CV Page (`_pages/cv.html`)
**Completely restructured:**
- Education section with Stanford MS&E and Duke/DKU degrees
- Research experience highlighting Qiu Lab work
- Professional experience (Sahara AI, Ping An, Sequoia)
- Teaching experience (MS&E 152, 252, 180)
- Technical skills emphasizing computational biology tools
- Languages section

## Content Highlights

### Research Narrative
The updated website now tells a cohesive story:
1. **Mathematical Foundation**: Applied Mathematics background with dynamical systems and stochastic modeling
2. **Machine Learning Expertise**: RL, NLP, transformers, neural networks
3. **Computational Biology Focus**: Spatial transcriptomics, single-cell genomics, developmental modeling
4. **Vision**: Building a Virtual Embryo to predict and prevent congenital diseases

### Key Achievements Highlighted
- Co-developing neural_field framework for 3D embryo reconstruction
- Leading manuscript on Virtual Embryo framework (Nature Methods)
- Contributing to Dynamo open-source project (472★ on GitHub)
- 94.98% accuracy on AI text detection (CS 224N)
- VRVO algorithm improving RL generalization

### Technical Depth
Each research project page includes:
- Scientific background and motivation
- Technical approach and innovations
- Methods and tools used
- Results and impact
- Connections to broader research goals
- Future directions

## Professional Presentation

### Academic Tone
- Formal, scholarly language appropriate for PhD applications
- Emphasis on research contributions and scientific impact
- Clear articulation of research vision and goals

### Structure
- Clean, organized sections
- Consistent formatting across pages
- Professional timeline layouts
- Clear hierarchies of information

## Next Steps

### Required Actions
1. **Update CV PDF**: Create and upload updated CV PDF to `/files/natalie_cv.pdf`
2. **Add Images**: Consider adding research figures/diagrams:
   - `images/neural-field-preview.png`
   - `images/dynamo-preview.png`
   - `images/sentinel-preview.png`
   - `images/vrvo-preview.png`
3. **Review and Edit**: Proofread all content for accuracy
4. **Test Locally**: Run `bundle exec jekyll serve` to preview changes
5. **Push to GitHub**: Commit and push changes to deploy

### Optional Enhancements
1. Add research highlights/news section
2. Include visualization of research workflow
3. Add links to code repositories (when public)
4. Create a research statement page
5. Add Google Scholar profile link when available

## File Changes Summary

### Modified Files
- `_config.yml`
- `_pages/about.md`
- `_pages/cv.html`
- `_data/navigation.yml`
- `_publications/2009-10-01-paper-title-number-1.md` (renamed content)

### New Files
- `_publications/2025-virtual-embryo.md`
- `_publications/2025-neural-field-3d.md`
- `_publications/2025-dynamo-protocols.md`
- `_portfolio/neural-field-embryo.md`
- `_portfolio/dynamo-release.md`
- `_portfolio/sentinel-nlp.md`
- `_portfolio/vrvo-reinforcement-learning.md`

### Deleted Files
- `_publications/2010-10-01-paper-title-number-2.md`
- `_publications/2015-10-01-paper-title-number-3.md`
- `_portfolio/portfolio-1.md`
- `_portfolio/portfolio-2.html`

## Deployment Instructions

```bash
# Navigate to repository
cd /Users/caoqt1/CascadeProjects/windsurf-project/NatalieCao323.github.io

# Check status
git status

# Add all changes
git add .

# Commit with descriptive message
git commit -m "Transform website for CS+Bio PhD applications

- Update focus to computational biology and developmental genomics
- Add publications on virtual embryo, neural fields, and Dynamo
- Create detailed research project pages
- Restructure CV to highlight computational biology work
- Update navigation and site configuration"

# Push to GitHub
git push origin main
```

The website will automatically rebuild and deploy via GitHub Pages (typically takes 1-2 minutes).

## Contact Information
All contact information remains current:
- Email: nc323@stanford.edu
- Location: 735 Campus Drive, Stanford, CA 94305
- GitHub: nataliecao323
- LinkedIn: natalie-c-568a28176
- ResearchGate: https://www.researchgate.net/profile/Natalie-Cao-2

---

**Last Updated**: October 16, 2025
**Purpose**: CS+Bio PhD Application Portfolio
**Focus**: Computational Biology, Machine Learning, Developmental Genomics
