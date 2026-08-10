# Neural Networks and Deep Learning — AAI-511-IN2

## Final Project: Music Genre and Composer Classification Using Deep Learning

MS Applied AI
University of San Diego — July 2026**  
Authors: Chandra Mouli Mudumba, Rajneesh Kumar and Rahul S Pawar 

---

## Overview

This repository contains the final team project for the course **AAI-511-IN2: Neural Networks and Deep Learning** as part of the MS Applied Artificial Intelligence program. The project develops and benchmarks deep learning models for classifying musical composers (Bach, Beethoven, Chopin, and Mozart) from symbolic MIDI data.

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
├── Chandra_Mouli_Mudumba_Final_Team_Project.ipynb   # Main Colab Notebook
├── Final_Project_Report_APA.md                       # APA-style Academic Report
├── README.md                                         # This file
└── data/                                             # Dataset (MIDI files)
```

## How to Run

1. Open `Chandra_Mouli_Mudumba_Final_Team_Project.ipynb` in Google Colab.
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
