# Assignment 2: Computer Vision - Deep Learning

**Course:** 94691 Deep Learning - Autumn 2024  
**University of Technology Sydney**

## Overview
This repository contains the code and report for Assignment 2 of the Deep Learning course. The assignment focuses on Transfer Learning using Convolutional Neural Networks (CNNs) applied to the Food101 dataset. The task is divided into two main parts:

- **Part A: Transfer Learning and Model Comparison**
- **Part B: Fine-Tuning the Best Model**

## Dataset
- **Name:** Food101
- **Description:** The dataset contains 101,000 images across 101 food categories. For each class, there are 750 training images and 250 test images, all resized to a maximum side length of 512 pixels.
- **Download Link:** [Food101 Dataset](https://link-to-food101-dataset)

## Part A: Transfer Learning
### Objective
Analyze and compare the architectures and performance of three pre-trained CNN models:
- GoogLeNet
- MobileNet V3
- NasNet

### Methodology
- Each model's head is replaced with:
  - A Global Average Pooling layer
  - Three fully connected layers, with the final layer being the output layer for class prediction.
- The models are fine-tuned on the Food101 dataset using pre-trained weights from the ImageNet dataset.

### Output
- Comparison of the models' performance in terms of accuracy and other relevant metrics.

## Part B: Fine-Tuning
### Objective
Fine-tune the best performing model from Part A by unfreezing at least two different layers.

### Methodology
- Experiment with unfreezing different layers and further training the model on the Food101 dataset to improve performance.

### Output
- Analysis of the fine-tuning process and its impact on model performance.

## Files Included
- **Part A Notebook:** `Part_A_Transfer_Learning.ipynb`
- **Part B Notebook:** `Part_B_Fine_Tuning.ipynb`
- **Report:** `Assignment2_Report.pdf`

## Report Contents
- **Presentation of the Dataset**
- **Detailed Analysis of the CNN Architectures**
  - Historical context and advancements of GoogLeNet, MobileNet V3, and NasNet.
- **Walk-Through of Transfer Learning**
  - Description of the training process for each model.
- **Performance Analysis**
  - Evaluation of the models' performance and limitations.
- **Fine-Tuning Approach**
  - Detailed steps and strategies used for fine-tuning the selected model.
- **Recommendations**
  - Discussion on remaining issues, limitations, and potential future improvements.
