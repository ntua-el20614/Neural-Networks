# WideResNet CIFAR Training

This repository contains a Jupyter notebook for training various configurations of Wide Residual Networks (WideResNet) on the CIFAR-10 dataset. The models are evaluated to understand the impact of dropout and mixup techniques on performance.

## Description

The notebook details experiments with several configurations of WideResNet models:
- Model 1: WRN-40-4, with and without dropout
- Model 2: WRN-28-10, with and without dropout
- Model 3: WRN-16-8, with and without dropout
- Additional experiments for WRN-28-10 with mixup and without mixup, including dropout in both cases

These models aim to classify images from the CIFAR-10 dataset, comparing the performance impacts of layer depth, dropout, and mixup regularization techniques.

## Getting Started

### Dependencies

- Get the .zip from the README.txt to start
- Python 3.8 or later
- PyTorch
- torchvision
- CUDA-compatible GPU environment (google colab!)

Ensure that you have the required libraries:
pip install torch torchvision

### Executing the Program

To run the notebook:
- Open `final_version.ipynb` in JupyterLab or Jupyter Notebook.
- Execute the cells sequentially to train the models and observe their performance.

## Models and Training

Each model was trained using SGD with momentum. Due to resource limitations on the free tier of Google Colab, the models were trained for up to 10 epochs. Even though the accuracy was notably low, this was expected as extended training sessions required a paid subscription which was not feasible for this project. Training for just 5 epochs was found to be suboptimal but was sufficient for educational purposes as per the course requirements.

## Results

The performance varied across different configurations, with dropout and mixup affecting the accuracy. Detailed results are documented in the notebook, showcasing how each modification influences model behavior under limited training epochs.

