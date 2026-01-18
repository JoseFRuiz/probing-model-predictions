# Probing Model Predictions

This repository contains an example demonstrating how to compute saliency maps using **Grad-CAM** (Gradient-weighted Class Activation Mapping) for image classification models.

## Overview

This demo uses a **ResNet-18** model pretrained on ImageNet to generate Grad-CAM saliency maps. The example works with camera trap images, but note that since the model was trained on ImageNet classes, the predicted classes will not be accurate for wildlife/camera trap images. The purpose of this demo is to illustrate how Grad-CAM highlights the regions of an image that the model focuses on when making predictions.

## Setup

We recommend creating a Conda environment to run this notebook:

```bash
# Create a new Conda environment
conda create -n gradcam-demo python=3.10

# Activate the environment
conda activate gradcam-demo

# Install required packages
conda install pytorch torchvision -c pytorch
conda install pillow matplotlib numpy
```

Alternatively, you can install the dependencies using pip:

```bash
pip install torch torchvision Pillow matplotlib numpy
```

## Usage

1. Open the `gradcam_saliency_demo.ipynb` notebook
2. Run the cells sequentially
3. The notebook will automatically download demo camera trap images
4. The Grad-CAM visualization will show which regions of the image the model focuses on for its prediction

## Dependencies

- `torch` (PyTorch)
- `torchvision`
- `Pillow` (PIL)
- `matplotlib`
- `numpy`

## Author

**Jose F. Ruiz-Munoz**

*Note: This repository was prepared with AI assistance.*