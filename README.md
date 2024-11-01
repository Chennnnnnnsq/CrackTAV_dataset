# Tunnel Crack Detection Thermal And Visible Dataset (CrackTAV)
A multimodal dataset for tunnel crack detection, containing various channel configurations including RGB, IR, fused RGB-IR, RGB-T, and RGB-IR modalities.


**A multimodal dataset for tunnel crack detection, containing various channel configurations including RGB, IR, fused RGB-IR, RGB-T, and RGB-IR modalities.**

## Overview

The Tunnel Crack Detection Dataset (CrackTAV) is a comprehensive dataset developed to support research in tunnel crack detection using multimodal imagery. The dataset includes visible light (RGB), infrared (IR), RGB_IR_Fused, RGBT, and RGBIR images, enabling researchers to explore the performance of detection models across different channel configurations and modalities. The dataset is designed to address challenges in complex lighting conditions and varying environmental factors.

## Table of Contents
- [Overview](#overview)
- [Dataset Structure](#dataset-structure)
- [Data Format](#data-format)
- [Sample Images](#sample-images)
- [How to Use](#how-to-use)
- [Citation](#citation)
- [License](#license)

## Dataset Structure

The dataset is organized into the following structure:

```plaintext
CrackTAV/
├── README.md               # Dataset description
├── images/                 # Contains all images in the dataset
│   ├── RGB/                # 3-channel RGB images (visible light)
│   ├── IR/                 # 3-channel IR images (thermal)
│   ├── RGB_IR_Fused/       # 3-channel fused RGB and IR images
│   ├── RGBT/               # 4-channel RGB and temperature images
│   └── RGBIR/              # 6-channel RGB and IR images
├── labels/                 # Ground truth labels for cracks
│   ├── RGB/                # Labels for RGB images
│   ├── IR/                 # Labels for IR images
│   ├── RGB_IR_Fused/       # Labels for fused RGB_IR images
│   ├── RGBT/               # Labels for RGBT images
│   └── RGBIR/              # Labels for RGBIR images
└── metadata.csv            # Metadata file containing additional information about each image
```

## Data Format

### Image Specifications

- **RGB Images**: 3-channel images representing the visible light spectrum.
- **IR Images**: 3-channel thermal images.
- **RGB_IR_Fused Images**: 3-channel images combining RGB and IR data.
- **RGBT Images**: 4-channel images, including RGB and a temperature channel.
- **RGBIR Images**: 6-channel images with both RGB and IR data combined.

- **Resolution**: All images are of size 256x256 pixels.
- **File Format**: Images are saved in JPEG format.

### Annotation Specifications

- **Format**: Annotations are provided as binary masks in PNG format.
- **Values**: Each pixel in the mask has a value of:
  - `0` for background (non-crack regions)
  - `1` for crack regions


