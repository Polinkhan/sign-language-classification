# Sign Language Detection and Classification

This repository contains the implementation of a Sign Language Detection and Classification system. The project is divided into two main components: a hand detection model using YOLOv8 and a classification model using PyTorch's Fastai library. The goal is to detect and classify sign language gestures from images.

## Introduction

Sign language is an essential mode of communication for individuals with hearing or speech impairments. This project aims to automate the detection and classification of sign language gestures to facilitate better communication.

## Workflow

The system works in two stages:

1. **Hand Detection**: The YOLOv8 model is used to detect the hand region in an image.
2. **Gesture Classification**: Once the hand is detected, the cropped image is passed to a classification model trained using various architectures like ResNet, MobileNet, VGG, and DenseNet.

## Dataset

The dataset used in this project contains images of 49 different sign language gestures. The data is split into training, validation, and test sets with an 80:10:10 ratio.

### Dataset Structure

```plaintext
Dataset/
│
├── detection/         # Data for YOLOv8 model
│   ├── train/
│   ├── valid/
│   ├── test/
│   └── custom.yaml/
│
├── classification/    # Data for classification model
│   ├── train/
│   ├── valid/
│   └── test/
