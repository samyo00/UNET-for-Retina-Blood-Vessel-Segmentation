# UNET-for-Retina-Blood-Vessel-Segmentation

This repository contains a Python notebook for semantic segmentation of retinal blood vessels using the U-Net architecture. The project utilizes the DRIVE dataset to perform image segmentation tasks.

<p align="center">
  <img src="https://github.com/user-attachments/assets/78e1bb02-0630-42f1-8197-191d33382693" alt="U-net"/>
</p>


## Project Overview

The goal of this project is to train a U-Net model to segment blood vessels from retinal images in the DRIVE dataset. The project notebook includes data loading, preprocessing, augmentation, model building, and training.

The notebook contains:
- **Data Preprocessing**: Loading images and ground truth masks, resizing them, and applying data augmentation.
- **U-Net Model Architecture**: Implementation of the U-Net model using PyTorch.
- **Training and Evaluation**: Includes training the model with a combined Dice and BCE loss, and evaluating it on the validation set.

## Dataset

<p align="center">
  <img src="https://github.com/user-attachments/assets/78e1bb02-0630-42f1-8197-191d33382693" alt="DRIVE dataset"/>
</p>

The [DRIVE dataset](https://drive.grand-challenge.org/) is used for training and testing. It includes:
- **Training images**: Retinal images with corresponding segmented vessel maps.
- **Test images**: Retinal images with ground truth vessel segmentations.

## Features

- **Data Augmentation**: Flipping and rotating the images to increase the dataset size.
- **U-Net Architecture**: Fully convolutional network for precise segmentation.
- **Custom Loss**: Combines Dice Loss and Binary Cross-Entropy (BCE) Loss.
- **Learning Rate Scheduling**: Uses ReduceLROnPlateau to adapt learning rate based on model performance.

## Requirements

To run the notebook, you'll need the following Python libraries:
- Python 3.8+
- PyTorch
- OpenCV
- imageio
- Albumentations
- tqdm

You can install the dependencies by running:

```bash
pip install torch opencv-python imageio albumentations tqdm
