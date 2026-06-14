# Deep-Learning-Based-Rice-Leaf-Disease-Classification-Using-Image-Processing
Deep Learning-based Rice Leaf Disease Classification using Custom CNN, VGG16, and ResNet50. Utilized image preprocessing, augmentation, and transfer learning techniques for automated crop disease detection.
# Deep Learning-Based Rice Leaf Disease Classification Using Image Processing

## Project Overview

This project develops a deep learning-based image classification system for detecting and classifying major rice leaf diseases using computer vision techniques. The system identifies three common rice diseases from leaf images and compares the performance of multiple deep learning architectures to determine the most effective approach.

## Objectives

* Classify rice leaf diseases from image data
* Apply image preprocessing and data augmentation techniques
* Build and evaluate deep learning models
* Compare custom CNN and transfer learning approaches
* Identify the most suitable model for future agricultural disease detection systems

## Dataset

The dataset contains RGB images of rice leaves categorized into three disease classes:

* Bacterial Leaf Blight
* Brown Spot
* Leaf Smut

### Dataset Characteristics

* Image Format: JPG (.jpg)
* Color Space: RGB
* Image Size: Resized to 128 × 128 × 3
* Total Images: Approximately 120
* Images per Class: ~40
* Capture Method: Field-collected images under natural lighting conditions

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* OpenCV
* Scikit-learn

## Data Preprocessing

The following preprocessing and augmentation techniques were applied:

* Image Rescaling (1/255)
* Rotation Augmentation (25°)
* Zoom Augmentation (0.2)
* Horizontal Flipping
* Train-Test Split
* Image Resizing (128×128)

These techniques were used to improve model robustness and reduce overfitting.

## Deep Learning Models Implemented

### 1. Custom CNN

* Convolutional Layers with ReLU Activation
* MaxPooling Layers
* Flatten Layer
* Dense Layer (64 Units)
* Dropout Layer (0.5)
* Softmax Output Layer

### 2. VGG16 (Transfer Learning)

* Pre-trained VGG16 Base Model
* Frozen Feature Extraction Layers
* Global Average Pooling Layer
* Dense Layer (128 Units)
* Dropout Layer
* Softmax Output Layer

### 3. ResNet50 (Transfer Learning)

* Pre-trained ResNet50 Base Model
* Frozen Base Layers
* Global Average Pooling Layer
* Dense Layer (128 Units)
* Dropout Layer
* Softmax Output Layer

## Model Performance

| Model      | Training Accuracy | Validation Accuracy |
| ---------- | ----------------- | ------------------- |
| Custom CNN | ~66%              | ~30%                |
| VGG16      | ~63%              | ~30%                |
| ResNet50   | ~39%              | ~30%                |

## Best Model

### VGG16

Although all models achieved similar validation accuracy, VGG16 was identified as the most promising model because:

* More stable learning behavior
* Better generalization than Custom CNN
* Less bias compared to ResNet50
* Strong foundation for future fine-tuning and improvement

## Key Features

* Deep Learning Image Classification
* Transfer Learning
* Data Augmentation
* CNN Architecture Design
* Performance Evaluation
* Confusion Matrix Analysis
* Classification Reports
* Agricultural Disease Detection

## Challenges Encountered

* Small dataset size
* Overfitting in Custom CNN
* Limited generalization capability
* Difficulty in fine-tuning pre-trained models
* Class imbalance and model bias

## Future Improvements

* Increase dataset size
* Apply advanced augmentation techniques
* Fine-tune deeper layers of pre-trained models
* Experiment with EfficientNet and MobileNet architectures
* Deploy as a web or mobile application for real-time disease detection

## Business Impact

Early detection of rice diseases can help farmers take preventive measures, reduce crop losses, improve yield quality, and support precision agriculture through AI-powered disease monitoring systems.

## Author

Zunaid Akhtar
