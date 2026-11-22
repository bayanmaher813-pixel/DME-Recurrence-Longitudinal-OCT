# Longitudinal Deep Learning for Predicting DME Recurrence from SD-OCT Scans

## 1. Project Overview
This repository houses the research codebase, preprocessing pipelines, and experimental evaluation framework for predicting anatomical recurrence of diabetic macular edema (DME) following the initial three-injection anti-VEGF loading phase using paired longitudinal spectral-domain optical coherence tomography (SD-OCT) B-scans.

## 2. Dataset Description
The pipeline processes paired longitudinal macular SD-OCT B-scans acquired at two clinical timepoints:
- **T0 (Baseline):** Pre-treatment fovea-centered SD-OCT B-scan prior to anti-VEGF initiation.
- **T1 (Post-Loading):** Post-stabilization SD-OCT B-scan acquired after completing three consecutive monthly anti-VEGF injections.
- **Target Label:** Binary anatomical recurrence (`Recurrent` vs. `Stable`) during pro re nata (PRN) follow-up, defined by central subfield thickness (CST) rebound or re-accumulation of intraretinal/subretinal fluid.

## 3. Software and Environment Requirements
- **Python:** 3.10+
- **Deep Learning Framework:** PyTorch 2.2.0, Torchvision 0.17.0
- **Medical Imaging & Scientific Stack:** `pydicom 2.4.4`, `SimpleITK 2.3.1`, `scikit-learn 1.4.2`, `numpy 1.26.4`, `pandas 2.2.1`
- **Hardware:** NVIDIA GPU with CUDA 12.1+ recommended for training

## 4. How to Run the Analysis
1. Clone the repository:
```bash
   git clone https://github.com/Bayanmaher/DME-Recurrence-Longitudinal-OCT.git
   cd DME-Recurrence-Longitudinal-OCT
