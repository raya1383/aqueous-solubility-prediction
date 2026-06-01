# Aqueous Solubility Prediction

This project implements a machine learning pipeline to predict the aqueous solubility (LogS) of small drug-like molecules using the ESOL dataset. The pipeline combines physicochemical descriptors and Morgan fingerprints as input features and trains a Random Forest regressor to estimate LogS.

## Features

- Computes 7 physicochemical descriptors (MolWt, LogP, TPSA, RotatableBonds, HDonors, HAcceptors, RingCount)
- Generates 2048-bit Morgan fingerprints for structural encoding
- Data preprocessing: handling invalid SMILES, feature scaling
- Dimensionality reduction and visualization via PCA
- Model evaluation: RMSE, MAE, R², cross-validation
- Feature importance analysis

## Dataset

The project uses the ESOL dataset (Delaney, 2004), which contains experimentally measured aqueous solubility values (LogS) for 1,128 drug-like molecules.

## Results
Random Forest regression achieved R² ≈ 0.87 on a held-out test set
Feature importance shows LogP as the most influential descriptor
Residuals and PCA plots indicate the model captures continuous trends in solubility
