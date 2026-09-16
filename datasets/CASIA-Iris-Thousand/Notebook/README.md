# Notebooks

This folder contains the Jupyter notebooks used for processing and analyzing the CASIA-Iris-Thousand dataset.

## Notebook Workflow

The notebooks are organized according to the processing workflow:

### 1. Dataset Collection and Analysis

This notebook is used to:

- Load and inspect the CASIA-Iris-Thousand dataset
- Analyze the dataset structure
- Examine image and identity information
- Perform initial dataset exploration

### 2. Image Preprocessing

This notebook handles the preprocessing of the ocular images, including:

- Loading the images
- Creating dataset splits
- Image resizing and cropping
- Grayscale conversion
- Pixel normalization
- Saving preprocessing configuration and related information

### 3. Ocular Image Quality Assessment

This notebook evaluates the quality of the images using metrics such as:

- Brightness
- Contrast
- Sharpness
- Noise

The quality assessment is used to understand the characteristics and quality of the dataset before further processing and experimentation.

## Execution Order

Run the notebooks in the following order:

1. Dataset Collection and Analysis
2. Image Preprocessing
3. Ocular Image Quality Assessment

## Environment

The notebooks are designed to run in a Python/Jupyter environment with the required dependencies installed.
