# Image Matching Challenge 2024

The goal of this project is constructing 3D model from 2D images(called Structure from Motion (SfM)). There are 7 objects and 6 categories in the data.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Process](#process)

## Installation

### Input
#### Datasets
- Image Matching Challenge 2024
- colmap-db-import
- imc2024-packages-lightglue-rerun-kornia
- dust3r-package
- einops
- module roma
- trimesh for kaggle
- Kornia Local Feature model weights
- SuperGluePretrainedNetwork
- pytorch_lightglue_models
- dkm_dependencies
- dependencies_imc
- matchformer_dependencies
- MatchFormer
- pkg_check_orientation
#### Models
- Dino v2
- Aliked
- LightGlue
- DUSt3R

## Usage
All the work was done in Kaggle. You can simply run the code by running it in Kaggle.

## Process
1. EDA & study about SfM
2. Search for related papers and select suitable models
3. Attempts to develop an algorithm
  1) Using train_labels to construct 3D models by clustering feature points (creating-a-3d-model-using-train-labels.ipynb)
    - preprocessing
    - Extracting feature points
    - Clustering & RANSAC
    - Construct 3D model by mapping points
    - Calculating projection matrices
  2) Using train_labels to construct 3D models by feature points matching (creating-a-3d-model-using-train-labels.ipynb)
    - preprocessing
    - Extracting feature points
    - Feature points matching
    - Graph-based clustering
