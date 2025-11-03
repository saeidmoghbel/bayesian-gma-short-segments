# Bayesian Modeling of Grammar in Short Segments

## Overview
This project implements a hierarchical Bayesian GLM to analyze grammatical features in English text. It extends Geometric Multivariate Analysis (GMA) to short text segments using probabilistic models and propagates feature uncertainty into PCA-derived dimensions [file:4].

## Features
- Fully self-contained workflow
- Extracts 6 POS features from Universal Dependencies corpus
- Bayesian GLM via PyMC
- Posterior predictive checking
- PCA with uncertainty intervals

## Requirements
- Python (>=3.11)
- pandas, numpy, matplotlib, scikit-learn, pyconll, tqdm, pymc, arviz, jupyter

## Usage
1. Clone this repo and create a Python virtual environment:
2. Place Universal Dependencies `.conllu` files in `./data/UD_English-EWT/`  
3. Open and run `gma_surrogate_bayesGLM_selfcontained_v5.ipynb` in Jupyter

## Outputs
- Model diagnostics and credible intervals for PCA loadings
- Plots comparing observed and synthetic data distributions

## Thesis Connection
This workflow directly addresses the challenges in extending GMA to short text segments with high variability and sparse features, as described in the QuanTOR project thesis proposal [file:4].

## Author
Saeid Moghbel — saeid.moghbel@fau.de
