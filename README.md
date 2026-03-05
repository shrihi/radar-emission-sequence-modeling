# Prediction and Classification of Dynamic Radar Emissions using NLP and Deep Learning

## Overview

This project explores the use of **machine learning and deep learning techniques for analyzing radar emission sequences in Electronic Intelligence (ELINT) systems**.

Traditional radar signal analysis methods rely on rule-based processing and static feature matching. However, modern radar systems dynamically change parameters such as frequency, pulse repetition intervals, and transmission patterns. These adaptive behaviors make conventional techniques less effective.

To address this, the project models **radar pulse streams as symbolic sequences**, similar to language modeling in Natural Language Processing (NLP), and applies **deep sequence learning techniques** to understand radar behavior.

---

## Key Objectives

- Model radar pulse streams as structured temporal sequences  
- Convert radar pulse parameters into symbolic tokens for sequence modeling  
- Learn contextual relationships between pulse patterns using embeddings  
- Apply deep learning to perform:
  - **Radar emitter classification**
  - **Radar emission prediction**

---

## System Pipeline

The overall framework follows a structured data processing and modeling pipeline:

```
Radar Pulse Data
       ↓
Data Cleaning & Preprocessing
       ↓
Pulse Deinterleaving
       ↓
Radar Pulse Symbolization
       ↓
Sequence Window Generation
       ↓
Word2Vec Embedding Learning
       ↓
LSTM-based Temporal Modeling
       ↓
Emitter Classification / Emission Prediction
```

---

## Core Techniques Used

- Radar Pulse Deinterleaving
- Symbolic Sequence Representation
- Word2Vec Skip-Gram Embeddings
- Long Short-Term Memory (LSTM) Networks
- Sliding Window Sequence Generation
- Multi-class Sequence Classification
- Next-Symbol Prediction

---

## Model Architecture

The classification model combines **embedding-based representation learning** with **temporal sequence modeling**.

```
Embedding Layer (Word2Vec initialized)
        ↓
Layer Normalization
        ↓
LSTM Layer (256 units)
        ↓
LSTM Layer (64 units)
        ↓
Dropout Regularization
        ↓
Dense Softmax Output Layer
```

This architecture allows the model to learn **temporal emission patterns and behavioral signatures of radar emitters**.

---

## Dataset Representation

Radar pulses are represented using parameters such as:

- Pulse Repetition Interval (PRI)
- Radio Frequency (RF)
- Pulse Width (PW)
- Time of Arrival (TOA)
- Signal amplitude

These parameters are transformed into **symbolic tokens**, enabling the pulse stream to be treated as a structured sequence suitable for machine learning.

---

## Results

The proposed framework demonstrates that radar emission sequences contain **structured temporal dependencies** that can be learned using deep sequence models.

The prediction framework achieved approximately **52% Top-5 accuracy**, indicating meaningful pattern learning in radar emission behavior.

---

## Repository Structure

```
assets/
   architecture.png
   embedding_diagram.png
   confusion_matrix.png
   training_curve.png
```

These diagrams illustrate the **system architecture, embedding representation, and experimental results**.

---

## Applications

This work contributes to research in:

- Electronic Intelligence (ELINT)
- Radar emitter identification
- Adaptive radar behavior analysis
- Data-driven signal intelligence systems

---
