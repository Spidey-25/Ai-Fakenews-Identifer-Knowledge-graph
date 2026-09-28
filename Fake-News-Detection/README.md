# Fake News Detection using Emotion Amplification and Knowledge Graphs

This repository contains the experimental notebooks for a research project focused on **fake news detection** using a hybrid approach that combines **textual features, emotional cues, and knowledge graph analysis**.  
The work explores how **emotion amplification** and **entity-level relationships** can improve both detection accuracy and interpretability.

---

## 🧠 Project Overview

Fake news often exploits emotional triggers and loosely connected facts to mislead readers.  
This project investigates a hybrid detection pipeline that integrates:

- **TF-IDF based text representation**
- **Emotion extraction and amplification**
- **Traditional machine learning classifiers**
- **Knowledge graph construction for explainability**

The goal is not only to classify news as *fake* or *real*, but also to **understand semantic and entity-level patterns** behind misinformation.

---

## 📊 Datasets Used

The experiments were conducted on a mix of benchmark, domain-specific, and synthetic datasets:

### 1. ISOT Fake News Dataset
- Source: Kaggle (University of Victoria)
- Size: ~44,000 news articles
- Domain: Political and world news
- Purpose: Benchmark evaluation on a large-scale dataset

### 2. Health & Well Being (HWB) Fake News Dataset
- Domain-specific research dataset
- Focus: Health-related misinformation
- Purpose: Evaluating model robustness on nuanced, sensitive content

### 3. Smoke & Mirrors News Collection (Synthetic Dataset)
- **Custom synthetic dataset created using DeepSeek**
- Size: ~2,000 samples
- Purpose:
  - Simulate controlled misinformation patterns  
  - Test generalisation and overfitting behaviour  
  - Support robustness analysis beyond real-world datasets

---

## 🧪 Methodology Highlights

- Text preprocessing: tokenization, stop-word removal, stemming
- Feature extraction using **TF-IDF**
- Emotion detection using **NRC Emotion Lexicon / pretrained models**
- **Emotion amplification** by scaling emotional scores and merging with textual vectors
- Model training using:
  - Logistic Regression
  - Support Vector Machines (SVM)
  - Random Forest
  - XGBoost
- Knowledge graph construction using:
  - Named Entity Recognition (SpaCy)
  - Graph modelling with NetworkX / Neo4j
- Visual analysis of entity coherence between real and fake news

---

## 📁 Repository Structure
```bash
notebooks/
├── Dataset_Generation.ipynb
├── Fake News Detection with Knowledge Graph on ISOT Dataset.ipynb
├── Fake News Detection with Knowledge Graph on Health & Well Being (HWB) Dataset.ipynb
└── Fake News Detection with Knowledge Graph on Smoke & Mirrors Dataset.ipynb
```

Each notebook is self-contained and documents the workflow for the corresponding dataset.

---

## 🛠️ Tools & Technologies

- Python
- Jupyter Notebooks
- pandas, scikit-learn, xgboost
- nltk, SpaCy
- NetworkX, Neo4j
- matplotlib
- DeepSeek (for synthetic dataset generation)

---

## ✨ Key Takeaway

Emotion-enriched features combined with **knowledge graph analysis** provide deeper insight into how fake news differs from real news — not just linguistically, but **semantically and structurally**.

---

## 👩‍💻 Author

**Namita S**  
Research Summer Internship Project

---

> This repository is intended for academic and research reference.
