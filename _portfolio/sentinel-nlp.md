---
title: "SENTINEL: AI-Generated Text Detection"
excerpt: "Heterogeneous ensemble framework for detecting AI-generated text, achieving 94.98% accuracy on Kaggle benchmark (CS 224N Final Project).<br/><img src='/images/sentinel-preview.png' style='max-width: 500px;'>"
collection: portfolio
---

## Project Overview

**SENTINEL** (Sophisticated Ensemble for Tracing and Identifying Non-Authentic Language) is a machine learning system designed to distinguish between human-written and AI-generated text. Developed as the final project for Stanford's CS 224N (Natural Language Processing with Deep Learning), SENTINEL combines state-of-the-art deep learning models with classical machine learning algorithms to achieve robust detection performance.

## Motivation

With the proliferation of large language models (GPT-3, GPT-4, Claude, etc.), the ability to reliably detect AI-generated content has become increasingly important for:
- Academic integrity and plagiarism detection
- Misinformation and disinformation prevention
- Content authenticity verification
- Understanding AI model behavior and limitations

## Technical Approach

### Heterogeneous Ensemble Architecture

SENTINEL integrates multiple complementary approaches:

#### Deep Learning Models
1. **BERT (Bidirectional Encoder Representations from Transformers)**
   - Fine-tuned for binary classification (human vs. AI)
   - Captures bidirectional context and semantic patterns
   
2. **RoBERTa (Robustly Optimized BERT)**
   - Enhanced pre-training and optimization
   - Better generalization across text styles

#### Classical Machine Learning
1. **Multinomial Naive Bayes (MNB)**
   - Fast, interpretable baseline
   - Effective for stylistic features
   
2. **Stochastic Gradient Descent (SGD) Classifier**
   - Linear model with online learning
   - Robust to high-dimensional features
   
3. **LightGBM & CatBoost**
   - Gradient boosting frameworks
   - Excellent performance on structured features

### Feature Engineering

#### Hybrid Feature Extraction
- **RoBERTa Embeddings**: Dense semantic representations (768-dim)
- **TF-IDF N-grams**: Sparse lexical features (1-3 grams)
- **Statistical Features**: Text length, vocabulary richness, punctuation patterns
- **Stylometric Features**: Sentence complexity, word frequency distributions

### Ensemble Strategy

- **Weighted Voting**: Learned weights based on validation performance
- **Stacking**: Meta-learner combines base model predictions
- **Diversity Optimization**: Selecting complementary models to reduce correlation

## Performance

### Kaggle Competition Results
- **Accuracy**: 94.98%
- **AUC-ROC**: 0.9685
- **F1-Score**: 0.9492
- **Precision**: 95.2%
- **Recall**: 94.7%

### Robustness Analysis
- **Cross-domain**: Tested on multiple text genres (essays, articles, social media)
- **Model Agnostic**: Detects text from various LLMs (GPT-3.5, GPT-4, Claude, etc.)
- **Adversarial Robustness**: Resistant to simple paraphrasing attacks

## Implementation Details

### Data Pipeline
1. **Preprocessing**: Custom tokenization, normalization, cleaning
2. **Augmentation**: Synthetic examples from multiple LLMs
3. **Balancing**: Stratified sampling to ensure class balance
4. **Validation**: 5-fold cross-validation for robust evaluation

### Model Training
- **Framework**: PyTorch, Transformers (Hugging Face), Scikit-learn
- **Optimization**: AdamW optimizer, learning rate scheduling
- **Regularization**: Dropout, weight decay, early stopping
- **Hardware**: NVIDIA V100 GPUs on Stanford clusters

### Inference
- **Latency**: <100ms per document (batch processing)
- **Scalability**: Handles documents up to 10,000 tokens
- **Deployment**: REST API for easy integration

## Key Insights

### What Makes Text "AI-like"?
1. **Consistency**: AI text tends to be more uniform in style
2. **Predictability**: Lower perplexity, more expected word choices
3. **Structure**: More regular sentence patterns
4. **Vocabulary**: Subtle differences in word usage distributions

### Model Interpretability
- **SHAP Values**: Identified key features for classification
- **Attention Visualization**: Highlighted discriminative text regions
- **Error Analysis**: Characterized failure modes and edge cases

## Connections to Computational Biology

While developed for NLP, SENTINEL's techniques are highly transferable to computational biology:

1. **Literature Mining**: Detecting AI-generated scientific abstracts
2. **Biomedical NLP**: Extracting information from PubMed articles
3. **Phenotype Tagging**: Classifying clinical descriptions
4. **Evidence Synthesis**: Aggregating findings from research papers
5. **Assay Classification**: Categorizing experimental protocols

## Code & Resources

- **Course**: [CS 224N: Natural Language Processing with Deep Learning](https://web.stanford.edu/class/cs224n/)
- **Instructor**: Professor Christopher Manning
- **Dataset**: Kaggle LLM Detection Challenge
- **Framework**: PyTorch, Transformers, Scikit-learn

## Future Enhancements

1. **Multilingual Detection**: Extend to non-English languages
2. **Fine-grained Attribution**: Identify specific AI models
3. **Temporal Robustness**: Adapt to evolving LLM capabilities
4. **Explainability**: Provide human-readable justifications
5. **Real-time Monitoring**: Continuous detection in production systems

## Lessons Learned

### Technical
- **Ensemble Diversity**: Combining different model families improves robustness
- **Feature Engineering**: Domain knowledge enhances deep learning
- **Hyperparameter Tuning**: Critical for optimal performance

### Practical
- **Data Quality**: Clean, diverse training data is essential
- **Evaluation**: Multiple metrics needed for comprehensive assessment
- **Deployment**: Production systems require latency/accuracy tradeoffs

---

**Duration**: April 2024 - June 2024  
**Course**: CS 224N: Natural Language Processing with Deep Learning  
**Institution**: Stanford University  
**Instructor**: Professor Christopher Manning  
**Achievement**: 94.98% accuracy on Kaggle benchmark
