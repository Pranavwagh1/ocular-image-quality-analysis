# CASIA-Iris-Thousand

## Overview

CASIA-Iris-Thousand is one of the datasets used in this project for ocular image analysis, preprocessing, and subsequent diffusion model training and ocular recognition experiments.

## Dataset Processing

The dataset is processed through the following stages:

### 1. Dataset Collection and Analysis

Initial analysis is performed to:

- Inspect the dataset structure
- Count images and identities
- Analyze image properties
- Examine left/right eye distribution
- Visualize sample images

### 2. Image Preprocessing

The preprocessing pipeline includes:

- Loading the images
- Creating identity-wise train/validation/test splits
- Converting images to grayscale
- Center cropping to a square
- Resizing images to `256 × 256`
- Normalizing pixel values to the range `[0, 1]`
- Converting processed images to `float32`

The preprocessing configuration is saved as:

`CASIA_Thousand_preprocessing_config.json`

### 3. Ocular Image Quality Assessment

Image quality is evaluated before using the dataset for further experiments.

The following quality metrics are analyzed:

- Brightness
- Contrast
- Sharpness
- Noise

For the current quality assessment, a random sample of **100 images** is analyzed.

#### Quality Metrics

- **Brightness:** Mean pixel intensity
- **Contrast:** Standard deviation of pixel intensities
- **Sharpness:** Variance of the Laplacian
- **Noise:** Standard deviation of the difference between the original image and a Gaussian-blurred image

Potential quality issues are identified using statistical thresholds based on the sample distribution.

## Notebooks

The analysis for this dataset is divided into three notebooks:

1. `01 — Dataset Collection and Analysis`
2. `02 — Image Preprocessing`
3. `03 — Ocular Image Quality Assessment`

## Results

The following result files are generated during processing:

- `CASIA_Thousand_data_split.csv`
- `CASIA_Thousand_preprocessing_config.json`
- `CASIA_Thousand_quality_assessment.csv`
- `CASIA_Thousand_quality_summary.csv`

## Purpose

The processed dataset and quality statistics will be used as a reference for subsequent synthetic ocular image generation and ocular recognition experiments.

