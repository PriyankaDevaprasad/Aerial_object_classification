# 🐦 Aerial Object Classification Using Deep Learning

## 📌 Project Overview

Aerial Object Classification is a deep learning project that classifies aerial images into two categories: **Bird** and **Drone**. The project uses PyTorch and Convolutional Neural Networks (CNNs) to learn visual patterns from images and predict the class of an uploaded image.

The project explores both a custom CNN and transfer learning using a pretrained ResNet50 model. A Streamlit web application provides an interactive interface for image classification.

## 🎯 Objectives

- Develop a deep learning model to distinguish birds from drones.
- Implement image classification using PyTorch.
- Compare a custom CNN with a pretrained ResNet50 model.
- Evaluate model performance using classification metrics.
- Deploy the trained model through a Streamlit web application.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Deep Learning Framework:** PyTorch
- **Image Processing:** Torchvision
- **Data Analysis:** NumPy, Pandas
- **Visualization:** Matplotlib, Seaborn
- **Model Evaluation:** Scikit-learn
- **Web Application:** Streamlit
- **Development Environment:** Google Colab

## 🧠 Models Implemented

### 1. Custom CNN

A Convolutional Neural Network built from scratch to learn image features through convolution, activation, pooling, and fully connected layers.

### 2. ResNet50 Transfer Learning

A pretrained ResNet50 model is adapted for binary classification by replacing its final fully connected layer with a two-class output layer. The pretrained feature extractor is used to reduce the amount of training required.

## 📂 Dataset

The dataset contains aerial images organized into two classes:

- **Bird**
- **Drone**

The data is divided into training, validation, and testing sets to support model training, model selection, and final performance evaluation.

### Image Preprocessing

- Resizing images to 224 × 224 pixels.
- Normalizing images using ImageNet mean and standard deviation.
- Applying data augmentation to training images, including random rotation, horizontal flipping, and color jitter.
- Loading images in batches using PyTorch DataLoaders.

## ⚙️ Project Workflow

1. Load and explore the dataset.
2. Preprocess images and apply data augmentation.
3. Create training, validation, and testing DataLoaders.
4. Build and train the custom CNN.
5. Implement ResNet50 transfer learning.
6. Monitor validation performance and save the best model.
7. Evaluate the models on the test dataset.
8. Compare model performance and visualize results.
9. Deploy the selected model using Streamlit.

## 📊 Model Evaluation

The models are evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report
- Training time and generalization performance

The comparison helps identify a suitable model for distinguishing birds from drones.

## 🌐 Streamlit Web Application

The web application allows users to:

- Upload an aerial image.
- View the uploaded image.
- Generate a prediction: **Bird** or **Drone**.
- View the model's predicted class and confidence score.

- Integrated a trained deep learning model into an interactive Streamlit application.
