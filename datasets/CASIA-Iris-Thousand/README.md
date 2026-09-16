# CASIA-Iris-Thousand

## Overview

CASIA-Iris-Thousand is one of the ocular datasets used in this project for image analysis, preprocessing, quality assessment, and subsequent experiments involving diffusion models and ocular recognition.

## Dataset Structure

The dataset contains ocular/iris images organized by subject identity, with separate directories for left (`L`) and right (`R`) eyes.

The dataset also includes a CSV file containing dataset-related information.

Example structure:

```text
CASIA-Iris-Thousand/
├── CASIA-Iris-Thousand/
│   ├── 000/
│   │   ├── L/
│   │   └── R/
│   ├── 001/
│   │   ├── L/
│   │   └── R/
│   ├── 002/
│   │   ├── L/
│   │   └── R/
│   └── ...
│
└── iris_thousands.csv
