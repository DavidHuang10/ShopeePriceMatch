# Shopee Product Matching - Kaggle Competition

## Project Overview
This repository contains the code and models for the Shopee Price Match Guarantee competition on Kaggle. The goal is to develop algorithms that can identify and match similar products in the e-commerce platform's marketplace using images and textual descriptions.

## Dataset
The dataset includes product images and descriptions provided by Shopee. It is divided into a training set and a test set, each containing unique product postings with associated image files, text descriptions, and labels.

### Files Structure
- `train_images/`: Folder containing the training images.
- `test_images/`: Folder containing the test images.
- `train.csv`: Training set metadata including titles and image paths.
- `test.csv`: Test set metadata for model evaluation.

## Models and Techniques
We utilize machine learning techniques involving contrastive loss and triplet networks to improve the feature embedding process for both images and text descriptions.

### Image Model
- **Triplet Network**: Optimizes a standard convolutional neural network by training in triplets - an anchor, a positive example, and a negative example.

### Text Model
- **Contrastive Loss**: Used to fine-tune embeddings such that similar items have closer embeddings, and dissimilar items are farther apart in the embedding space.

## Requirements
To install necessary libraries:
```bash
pip install -r requirements.txt
