# Machine Learning Based Firewall
## BSc Ethical Hacking Honours Dissertation - CMP403

**Author:** Alejandro Panigada  
**Institution:** Abertay University  
**Submission Date:** April 22, 2026  

---

## Project Overview

This repository contains the implementation and evaluation of machine learning and deep learning models for network intrusion detection, comparing XGBoost gradient boosting against Transformer-based architectures on the LyCoS-Unicas-IDS2018 dataset.

---

## Key Results

- **XGBoost:** 90.28% macro F1, 98.97% accuracy
- **Transformer:** 89.54% macro F1, 99.11% accuracy
- **Dataset:** 100,000 stratified sample, 77→56 features (permutation-based RFECV)
- **Production-ready:** 8/10 attack classes achieve F1 ≥ 0.95
- **Challenge:** Slowhttptest/FTP-Patator confusion accounts for 91.4% of errors

---

## Repository Contents

- `ml-deployed-Final.ipynb` - Main notebook containing all experiments
- 'loadset_dataset.zip' serialized dataset
- 'ids_artifacts' - serialized models 
- `README.md` - This file

---

## Requirements

- Python 3.10.13
- scikit-learn 1.3.2
- XGBoost 2.0.3
- PyTorch 2.1.2
- pandas 2.1.4
- NumPy 1.26.2


---

## Usage

1. Extract files from ids_artefacts.zip and loadset_dataset.zip in a folder named "Artefacts" (for inference)
2. Open notebook: `jupyter notebook ml-deployed-Final.ipynb`
3. Run cells in order to reproduce experiments
4. Random seed 42 used throughout for reproducibility
5. Can skip to chapter 7-8 for serialization loading and deployment without retraining

---

## Dataset

**LyCoS-Unicas-IDS2018** - Corrected version of CSE-CIC-IDS2018  
- 13,691,268 total records
- 100,000 stratified sample used (0.73%)
- 10 attack classes + Benign traffic
- Features extracted via LycoSTand

To be extracted and put inside a folder named "datset"

---

## Citation