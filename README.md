
# Crop and Weed Classification using CNN

A multi-class image classification project using a basic Convolutional Neural Network (CNN) implemented from scratch with PyTorch.

## Project Overview

This project classifies 14 crop and weed species using a greenhouse image dataset containing 28,000 images.

Two CNN experiments were conducted to evaluate the effects of data augmentation and dropout on classification performance.

## Dataset

- Source: Mendeley Data
- Total Images: 28,000
- Total Classes: 14
- Crop Classes: 8
- Weed Classes: 6
- Dataset Size: 1.42 GB

Dataset DOI: https://doi.org/10.17632/hs7d7kpd3z.3

## Model Architecture

- 3 Convolutional Layers
- ReLU Activation
- Max Pooling
- Flatten Layer
- 2 Fully Connected Layers
- Dropout (Round 2)
- 14 Output Classes

## Dataset Split

| Dataset | Images | Percentage |
|---|---:|---:|
| Training | 19,600 | 70% |
| Validation | 4,200 | 15% |
| Testing | 4,200 | 15% |

## Experimental Results

| Metric | Round 1 | Round 2 |
|---|---:|---:|
| Epochs | 15 | 30 |
| Data Augmentation | No | Yes |
| Dropout | 0.0 | 0.5 |
| Best Validation Accuracy | 82.14% | 87.12% |
| Test Accuracy | 80.69% | 86.76% |

**Test Accuracy Improvement: +6.07 percentage points**

## Final Model Performance

- Test Accuracy: 86.76%
- Test Loss: 0.4063
- Macro Precision: 87.04%
- Macro Recall: 86.76%
- Macro F1-Score: 86.70%

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebook

## Conclusion

The CNN model achieved 86.76% test accuracy across 14 crop and weed classes. Data augmentation and dropout improved generalization compared to the baseline CNN model.

## Dataset Reference

A Novel Automated Cloud-Based Image Datasets for High Throughput Phenotyping in Weed Identification.

Mendeley Data:
https://doi.org/10.17632/hs7d7kpd3z.3
