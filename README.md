# Employing Knowledge Distillation to Create Light-Weight Lane Detection Machine Learning Models for Low-Cost Computing Environments

## Overview

This project, spearheaded by LeAnn Mendoza at Northeastern University San Jose, delves into the utilization of knowledge distillation for optimizing lane detection models in autonomous driving vehicles. [Knowledge distillation](https://arxiv.org/abs/1503.02531), a model compression technique developed by Hinton et. al, allows for the creation of compact yet accurate deep learning models. By distilling a large, cumbersome model into a smaller, student model, we aim to maintain high levels of accuracy while significantly reducing model size, computation memory, and energy costs.

The Jupyter notebook, `main.ipynb`, contains comprehensive experiments and analyses supporting this research. It outlines the methodology for applying knowledge distillation to lane detection models and presents the findings, demonstrating the feasibility and effectiveness of this approach for application in edge computing (Raspberry Pi)

## Objectives

- To demonstrate the application of knowledge distillation in reducing the size of lane detection models without significantly compromising accuracy.
- To design efficient and compact deep learning networks capable of operating on low-power edge devices.
- To present a comparative analysis of model performance pre and post-knowledge distillation, emphasizing model size reduction, mean squared error (MSE), and R2 metrics.

## Methodology

### Data Collection

The dataset was created using a SunFounder Smart Video Car Kit V2.0 for Raspberry Pi 4, capturing images and their respective driving angles through a driver-controlled run.

### Model Development and Training

A cumbersome model was developed using TensorFlow and Keras libraries, employing an NVIDIA CNN Model architecture. This model served as the baseline for distillation into various student models, differing primarily in their convolutional filter sizes.

### Experimental Design

The experiments aimed to develop student CNN models that reduce model size while minimizing accuracy loss, measured by the difference in MSE and R2 between the cumbersome model and the student models. Different temperatures (T) were used during knowledge distillation to optimize model performance.

## Installation and Usage

Ensure you have Jupyter Notebook or JupyterLab installed to interact with the notebook. It's recommended to create a virtual environment and install the necessary dependencies listed in the notebook, such as TensorFlow, Keras, and others relevant to the project. Personally, I utilized the Jupyter Notebook integration on Google Collab.

## Contributions and Contact

Contributions to this project are welcome. For questions, suggestions, or potential collaborations, please reach out to LeAnn Mendoza at mendoza.l@northeastern.edu.

## Acknowledgments

This work was presented at SIGCSE '23, Toronto, Ontario, Canada. Special thanks to all collaborators and participants in the study for their valuable input and feedback.
