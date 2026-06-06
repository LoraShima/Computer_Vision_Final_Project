# Urban Scene Classification Using CNN and Transformer Architectures

## Project Overview

This project focuses on the multiclass classification of urban scene images using several state-of-the-art Deep Learning architectures. The objective is to classify images into one of ten urban categories:

* Bridge
* Commercial
* Industrial
* Intersection
* Landmark
* Park
* Parking
* Playground
* Residential
* Stadium

The study compares both Convolutional Neural Network (CNN) architectures and Transformer-based architectures to evaluate their effectiveness for urban scene recognition. In addition, the impact of Transfer Learning is investigated by training each model both with and without pretrained weights.

## Dataset
https://www.kaggle.com/datasets/yessicatuteja/skycity-the-city-landscape-dataset/data 
The dataset contains approximately 8,000 images distributed across ten urban scene classes. Images were divided into training, validation, and test sets to ensure a fair evaluation process.

Before training, the images were preprocessed through:

* Image resizing
* Normalization
* Data augmentation

  * Random horizontal flips
  * Rotations
  * Other transformations to improve generalization

## Models Evaluated

### CNN Architectures

* VGG19
* ResNet101
* EfficientNet-B0

### Transformer Architectures

* Vision Transformer (ViT)
* Swin Transformer

Each architecture was evaluated in two configurations:

1. Training from scratch (pretrained=False)
2. Transfer Learning (pretrained=True)
