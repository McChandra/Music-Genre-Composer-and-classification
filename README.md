# Music Genre and Composer Classification Using Deep Learning

## Final Team Project — Neural Networks and Deep Learning

**Authors:** Chandra Mouli Mudumba, Rajneesh Kumar, Rahul S Pawar  
**Date:** August 10, 2026  
**University of San Diego, MS Applied AI**

---

## Overview

This repository contains the Final Team Project for the course **Neural Networks and Deep Learning** as part of the MS Applied AI program at the University of San Diego. The project develops and benchmarks deep learning models for classifying musical composers (Bach, Beethoven, Chopin, and Mozart) from symbolic MIDI data.

## Models Implemented

| Model | Architecture | Key Feature |
|-------|-------------|-------------|
| CNN | Convolutional Neural Network | 2D Piano Roll spatial patterns |
| Bi-LSTM | Bidirectional LSTM | Sequential temporal dependencies |
| MusicBERT (Variant) | Transformer (BERT-based) | Self-attention with OctupleMIDI tokenization |

## SOTA Models Referenced

- **MusicBERT** — OctupleMIDI encoding with bar-level masking (Zeng et al., 2021)
- **MIDI-BERT** — Compound Word (CP) representation for piano (Chou et al., 2021)
- **MMT-BERT** — Chord-aware multitrack generation (Zhu et al., 2024)

## Frameworks & Tools

- **MusPy** — Symbolic music data handling
- **PyTorch Lightning** — Structured model training
- **Optuna** — Hyperparameter optimization
- **Transformers (HuggingFace)** — BERT architecture
- **Scikit-learn** — Evaluation metrics

## Repository Structure

```
├── Final Project.ipynb                                                        # Main Colab Notebook
├── Project Report - Music Genre and Composer Classification Using Deep Learning.md   # APA-style Academic Report
├── README.md                                                                  # This file
└── data/                                                                      # Dataset (MIDI files)
```

## How to Run

1. Open `Final Project.ipynb` in Google Colab.
2. The first cell installs all required dependencies.
3. Upload your MIDI dataset to the Colab runtime.
4. Run all cells sequentially.

## Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| CNN | 91% | 90% | 91% | 90% |
| Bi-LSTM | 85% | 84% | 85% | 84% |
| MusicBERT (Variant) | **95%** | **94%** | **95%** | **94%** |

## License

This project is for academic purposes as part of the MS Applied AI program.
