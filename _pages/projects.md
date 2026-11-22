---
title: "Projects"
permalink: /projects/
author_profile: true
---

Small open-source projects, mostly in Python, on electrochemical simulation, data analysis and modelling. All code is on [GitHub](https://github.com/deannguyen9xyz).

## Electrochemical simulation

* **[CV-simulation](https://github.com/deannguyen9xyz/CV-simulation)**: simulates cyclic voltammetry of a reversible redox couple at a planar electrode by solving Fick's second law with an explicit finite-difference scheme under Nernstian conditions.
* **[SWV-Simulator](https://github.com/deannguyen9xyz/SWV-Simulator)**: simulates square-wave voltammograms with a charging-current baseline, then extracts the faradaic peak height by sliding-window linear baseline fitting.
* **[PINN-diffusion-study](https://github.com/deannguyen9xyz/PINN-diffusion-study)**: a physics-informed neural network (PyTorch) that solves the diffusion equation for concentration depletion near an electrode, trained on the governing equation and boundary conditions instead of data.

## Electrochemical data analysis

* **[CV-anodic-peak-extraction](https://github.com/deannguyen9xyz/CV-anodic-peak-extraction)**: notebook that fits a linear baseline in a pre-peak window and extracts anodic peak currents from multi-cycle CV exports (PalmSens PSTrace), averaged over consecutive scans.
* **[originlab-voltammetry-peaks](https://github.com/deannguyen9xyz/originlab-voltammetry-peaks)**: Python script for OriginLab that finds voltammetric peaks in Gamry files, subtracts a user-defined baseline and reports mean ± SD peak heights over cycles.
* **[Electrochemical-Wavelet-Denoising](https://github.com/deannguyen9xyz/Electrochemical-Wavelet-Denoising)**: denoising of simulated sensor binding-kinetics data with Savitzky–Golay smoothing and wavelet thresholding, followed by an anchored kinetic fit to recover the binding rate constant.
* **[EIS_Randles_Fitting](https://github.com/deannguyen9xyz/EIS_Randles_Fitting)**: fits impedance spectra to a Randles circuit with eight methods (local least squares, global optimizers and Bayesian MCMC) and compares the results.
* **[EIS-Fitting-Models](https://github.com/deannguyen9xyz/EIS-Fitting-Models)**: fits impedance spectra with three equivalent circuits: Randles (sensors), modified Randles and a two-RC Thevenin model (Li-ion batteries).

## Machine learning for electrochemical sensing

* **[SWV-Concentration-Prediction-ML](https://github.com/deannguyen9xyz/SWV-Concentration-Prediction-ML)**: compares 1D-CNN, LSTM/GRU and hybrid CNN–Transformer models that predict analyte concentration directly from augmented SWV curves of MIP sensors.
* **[cv-data-augmentation](https://github.com/deannguyen9xyz/cv-data-augmentation)**: augmentation methods for cyclic voltammetry data (potential shift, current scaling, baseline drift, peak broadening, warping and noise) to build machine-learning training sets.

## MIPs, materials and molecular modelling

* **[SEM-BSE-image-analysis-MIP-RuO2](https://github.com/deannguyen9xyz/SEM-BSE-image-analysis-MIP-RuO2)**: corrects backscattered-electron SEM images for emission-current differences between sessions and compares bare and MIP-modified RuO₂ screen-printed electrodes.
* **[Python-Molecular-Docking](https://github.com/deannguyen9xyz/Python-Molecular-Docking)**: docking workflow following the RCSB PDB-101 Python training: ligand preparation with Meeko, docking with AutoDock Vina and interaction fingerprints with ProLIF.

## Batteries and fuel cells

* **[battery-ekf-soc-estimator](https://github.com/deannguyen9xyz/battery-ekf-soc-estimator)**: extended Kalman filter for Li-ion state-of-charge estimation with a 1RC equivalent-circuit model under a dynamic current profile.
* **[battery-hybrid-digital-twin](https://github.com/deannguyen9xyz/battery-hybrid-digital-twin)**: hybrid Li-ion battery model combining a physics-based voltage model with a machine-learning residual corrector for aging-induced drift.
* **[Li-ion-RUL-Prediction](https://github.com/deannguyen9xyz/Li-ion-RUL-Prediction)**: remaining-useful-life prediction on NASA battery degradation data, with correlation analysis and random-forest regression validated on an unseen cell.
* **[pem-fuel-cell-model](https://github.com/deannguyen9xyz/pem-fuel-cell-model)**: physics-based PEM fuel cell simulator (Nernst voltage with activation, ohmic and concentration losses) giving polarization and power curves.
