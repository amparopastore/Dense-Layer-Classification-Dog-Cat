# Dog vs Cat Image Classification Using Dense Layers

## Author: Amparo Godoy Pastore
## Date: June 2nd, 2024
## Course: CAP 6619 - Deep Learning
## Professor: Xingquan Zhu

## Overview
This repository contains the code and data for Homework 2, Question 7 of the CAP 6619 - Deep Learning course at Florida Atlantic University. The task involves building and evaluating dense layer neural networks to classify images from the Dogs vs Cats dataset.

## Dataset
The Dogs vs Cats Dataset consists of 1000 color images of dogs and cats. Each image is 32x32 pixels, with 500 images of dogs and 500 images of cats.

## Repository Contents
- `dogs_vs_cats_photos.npy`: Numpy array containing the images.
- `dogs_vs_cats_labels.npy`: Numpy array containing the target labels.
- `Dog vs Cat Image Classification Using Dense Layers.ipynb`: Jupyter Notebook containing the code for loading data, visualizing it, training, and evaluating different neural network architectures.

## Notable Functions
- `show_a_random_face_per_class(images, unique_ids)`: Displays one random face for each of the 40 classes in the dataset.
- `create_model(layers)`: Creates a neural network model with the specified number of layers.
- `evaluate_model(layers, data, target, kf)`: Evaluates a model using k-fold cross-validation.

## Results
The notebook compares the performance of two different neural network architectures:
1. Model 1: Feedforward neural network with one hidden layer.
2. Model 2: Feedforward neural network with one hidden layer, batch normalization, and dropout.

### Accuracy Results
- **Model 1:** Mean Accuracy: 0.5010, Std Dev: 0.0563
- **Model 2:** Mean Accuracy: 0.5030, Std Dev: 0.0593

### Conclusion
Model 2, which includes batch normalization and dropout, exhibits slightly better performance in terms of mean accuracy compared to Model 1. Both batch normalization and dropout contribute positively to the model's performance by stabilizing training and preventing overfitting.
