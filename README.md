# Lightweight-Chinese-Sentiment-NLP
Lightweight Aspect-Based Sentiment Analysis (ABSA) for Chinese restaurant reviews using knowledge distillation.
This project implements a teacher–student architecture where a large Chinese RoBERTa model is distilled into a compact DistilBERT-based model enhanced with aspect-specific attention pooling.
The resulting model achieves ~82% accuracy and ~0.76 macro-F1, while being over 2× faster and significantly smaller than the teacher — making it suitable for real-time and resource-constrained deployments.

The repository includes:

Preprocessing pipeline for the ASAP Chinese restaurant review dataset

Teacher model (RoBERTa + Aspect Attention)

Student model (DistilBERT + Knowledge Distillation)

Baseline models (TF-IDF + Logistic Regression, BiLSTM, TextCNN)

Evaluation scripts: per-aspect analysis, confusion matrices, error analysis

Complete training code and model checkpoints

This work accompanies the research paper:
**“Lightweight Aspect-Based Sentiment Analysis for Chinese Reviews


Dataset: https://github.com/Meituan-Dianping/asap/tree/master/data
