# Amazon-531 Hierarchical Multi-Label Classification (BDA Final Project)

This repository contains the code and notebooks for a hierarchical multi-label text classification project on **Amazon-531**.
The pipeline focuses on **silver label generation**, **graph-aware class embeddings (GAT)**, and **self-training**.

---

## Project Structure

### Notebooks

#### 1) Pseudo label / document generation
- **`pseudo_label_doc.ipynb`**  
  Generates **class description documents** by calling GPT (documents that explain each label).

- **`pseudo_doc_generate.ipynb`**  
  Generates **review-like documents for each label** by calling GPT (data augmentation).

> Generated outputs from the notebooks above are stored in **`Amazon_products/`**.

#### 2) Training / Self-training
- **`selftraining.ipynb`**  
  Runs the **best model** (final pipeline).

- **`selftraining_2mlp.ipynb`**  
  Ablation: **best model without GAT** (replaces GAT with a 2-layer MLP).

- **`selftraining_2gat.ipynb`**  
  Ablation: **best model with deeper GAT** (2-layer GAT).

- **`wout_selftraining.ipynb`**  
  Ablation: **best model without self-training**.

---
