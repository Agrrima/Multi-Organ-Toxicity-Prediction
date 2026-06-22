
# Multi-Organ Toxicity Prediction

This repository contains machine learning and graph neural network approaches for predicting drug-induced toxicities from molecular structure and biological interaction data.

The projects explore two complementary paradigms in computational toxicology:

* **Graph neural networks operating on drug-protein interaction networks**
* **Classical machine learning on molecular descriptors and fingerprints**


---

## Project 1: Ototoxicity Prediction using Graph Neural Networks

A heterogeneous drug-protein graph was constructed using molecular fingerprints, protein features, and drug-target interaction data obtained from ChEMBL.


### Objective

Predict compounds associated with ototoxicity while leveraging both molecular structure and biological interaction information.


### Methodology

* Heterogeneous drug-protein graph construction
* Drug-protein interaction edges from ChEMBL
* Drug-drug similarity edges using molecular fingerprints
* GraphSAGE architecture
* Batch normalization and residual connections
* Focal loss for class imbalance handling
* Random Forest baseline and ensemble comparison

---

## Project 2: Cardiotoxicity Prediction using Molecular Fingerprints

A scaffold-aware machine learning pipeline was developed to predict cardiotoxic compounds from molecular structure.

### Objective

Assess the ability of machine learning models to generalize structurally novel compounds using chemically informed validation strategies.

### Methodology

* PubChem BioAssay AID 588834 dataset
* Canonical SMILES standardization and deduplication
* Morgan fingerprints (ECFP4)
* MACCS structural keys
* Physicochemical descriptors
* Bemis-Murcko scaffold-based train/test split
* Leakage-free threshold optimization using out-of-fold predictions
* Random Forest and XGBoost benchmarking



## Technical Stack

* Python
* RDKit
* PyTorch Geometric
* Scikit-learn
* XGBoost
* Pandas
* NumPy






