# Computer Vision - Deep Learning

## Overview
This repository contains the code and report for the Deep Learning course. The assignment focuses on Transfer Learning using Convolutional Neural Networks (CNNs) applied to the Food101 dataset. The task is divided into two main parts:

- **Part A: Transfer Learning and Model Comparison**
- **Part B: Fine-Tuning the Best Model**

## Dataset
- **Name:** Food101
- **Description:** The dataset contains 101,000 images across 101 food categories. For each class, there are 750 training images and 250 test images, all resized to a maximum side length of 512 pixels.
- **Download Link:** [Food101 Dataset](http://data.vision.ee.ethz.ch/cvl/food-101.tar.gz)

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
- **Part A Notebook:** `googlenet-model.ipynb`, `mobilenet-model.ipynb`,`nasnet-model.ipynb`
- **Part B Notebook(Fine tunning model):** `mobilenet-model-finetunning.ipynb`
- **Report:** `Report.docx`

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

## Acknowledgments

The task content is from the **Master of Data Science and Innovation** course of University of Technology Sydney, and it is the asset of TD School)

## License Agreements of the Dataset:
 - The Food-101 data set consists of images from Foodspotting [1] which are not
   property of the Federal Institute of Technology Zurich (ETHZ). Any use beyond
   scientific fair use must be negociated with the respective picture owners
   according to the Foodspotting terms of use [2].

[1] http://www.foodspotting.com/
[2] http://www.foodspotting.com/terms/

