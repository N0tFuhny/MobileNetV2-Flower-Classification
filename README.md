# 🌸 Flower Image Classification using MobileNetV2 Transfer Learning

### Computer Vision • Deep Learning • TensorFlow • Model Deployment

<p align="center">

<img src="https://img.shields.io/badge/Test%20Accuracy-89.75%25-success?style=for-the-badge" />
<img src="https://img.shields.io/badge/Classes-5-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/Dataset-3000%2B%20Images-orange?style=for-the-badge" />

</p>

<p align="center">

<img src="https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow" />
<img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras" />
<img src="https://img.shields.io/badge/MobileNetV2-Transfer%20Learning-success?style=for-the-badge" />
<img src="https://img.shields.io/badge/TensorFlow-Lite-yellow?style=for-the-badge" />
<img src="https://img.shields.io/badge/TensorFlow.js-orange?style=for-the-badge" />

</p>

---

## 🚀 Project Objective

Develop an end-to-end image classification system capable of recognizing flower species using Transfer Learning with MobileNetV2. This project demonstrates practical skills in Computer Vision, Deep Learning, model evaluation, and deployment across multiple platforms.

### Key Highlights

* Achieved **89.75% Test Accuracy**
* Trained on **3,000+ flower images**
* Classified **5 flower categories**
* Implemented **Transfer Learning using MobileNetV2**
* Exported model to **SavedModel, TensorFlow Lite, and TensorFlow.js**
* Applied **Data Augmentation, Batch Normalization, and Dropout**
* Built using **TensorFlow and Keras**

---

## 📌 Project Overview

This project was developed to demonstrate practical implementation of:

* Computer Vision
* Deep Learning
* Transfer Learning
* Convolutional Neural Networks (CNN)
* Model Evaluation
* AI Model Deployment

The workflow covers the complete machine learning pipeline, including:

* Data Preprocessing
* Data Augmentation
* Model Development
* Model Training
* Performance Evaluation
* Deployment-Ready Model Conversion

---

## 🛠 Tech Stack

| Category                | Technology      |
| ----------------------- | --------------- |
| Programming Language    | Python          |
| Deep Learning Framework | TensorFlow      |
| High-Level API          | Keras           |
| Transfer Learning Model | MobileNetV2     |
| Numerical Computing     | NumPy           |
| Visualization           | Matplotlib      |
| Mobile Deployment       | TensorFlow Lite |
| Web Deployment          | TensorFlow.js   |

---

## 📂 Dataset

**Dataset:** Flower Photos Dataset

### Dataset Characteristics

* More than 3,000 images
* 5 flower categories
* Multi-class image classification task

### Classes

* Daisy
* Dandelion
* Roses
* Sunflowers
* Tulips

### Dataset Split

* Training Set
* Validation Set
* Testing Set

---

## 🏗 Model Architecture

### Transfer Learning Backbone

* MobileNetV2 (ImageNet Pretrained)
* include_top=False
* Frozen feature extractor during training

### Classification Head

* Conv2D
* MaxPooling2D
* GlobalAveragePooling2D
* BatchNormalization
* Dense Layer (256 Units, ReLU)
* Dropout (0.5)
* Dense Softmax Output Layer

### Architecture Flow

```text
Input Image
      │
      ▼
Data Augmentation
      │
      ▼
MobileNetV2
(ImageNet Pretrained)
      │
      ▼
Conv2D
      │
      ▼
MaxPooling2D
      │
      ▼
GlobalAveragePooling2D
      │
      ▼
BatchNormalization
      │
      ▼
Dense (256, ReLU)
      │
      ▼
Dropout (0.5)
      │
      ▼
Softmax Output (5 Classes)
```

---

## ⚙️ Training Configuration

### Data Augmentation

Applied augmentation techniques:

* Rotation
* Zoom
* Width Shift
* Height Shift
* Brightness Adjustment
* Horizontal Flip

### Optimization

**Optimizer**

* Adam

**Learning Rate**

* 0.0003

### Training Callbacks

* EarlyStopping
* ReduceLROnPlateau

---

## 📊 Results

### Model Performance

| Metric              | Score  |
| ------------------- | ------ |
| Training Accuracy   | 98.40% |
| Validation Accuracy | 89.95% |
| Test Accuracy       | 89.75% |
| Test Loss           | 0.3186 |

---

## 📈 Performance Snapshot

| Category            | Result        |
| ------------------- | ------------- |
| Number of Classes   | 5             |
| Dataset Size        | 3,000+ Images |
| Training Accuracy   | 98.40%        |
| Validation Accuracy | 89.95%        |
| Test Accuracy       | 89.75%        |
| Deployment Formats  | 3             |

---

## 🔍 Performance Analysis

The model achieved nearly 90% test accuracy while maintaining stable generalization across validation and testing datasets.

### Factors Contributing to Performance

* Transfer Learning using MobileNetV2 pretrained on ImageNet
* Data augmentation for improved robustness
* Batch Normalization for training stability
* Dropout regularization to reduce overfitting
* Adaptive learning rate scheduling with ReduceLROnPlateau

These results demonstrate the effectiveness of transfer learning for image classification tasks with relatively limited datasets.

---

## 🚀 Model Deployment

The trained model was exported into multiple deployment formats.

### TensorFlow SavedModel

Suitable for:

* TensorFlow Serving
* Further Fine-Tuning
* Production Environments

### TensorFlow Lite (TFLite)

Suitable for:

* Mobile Applications
* Edge Devices
* Embedded Systems

### TensorFlow.js

Suitable for:

* Browser-Based Inference
* Web Applications
* Front-End AI Deployment

---

## 💡 Skills Demonstrated

### Machine Learning

* Transfer Learning
* Deep Learning
* CNN Architecture Design
* Model Evaluation
* Hyperparameter Tuning

### Computer Vision

* Image Classification
* Feature Extraction
* Data Augmentation
* Image Preprocessing

### AI Engineering

* TensorFlow & Keras
* TensorFlow Lite Deployment
* TensorFlow.js Deployment
* Model Export & Conversion
* End-to-End ML Pipeline Development

---

## 🎯 Key Achievements

✅ Achieved **89.75% Test Accuracy** on a multi-class image classification problem

✅ Implemented **Transfer Learning using MobileNetV2 pretrained on ImageNet**

✅ Built an **end-to-end deep learning workflow** from preprocessing to deployment

✅ Exported models for **mobile, web, and production environments**

✅ Applied regularization techniques to improve model generalization

✅ Demonstrated practical experience in **Computer Vision and AI Deployment**

---

## 🔮 Future Improvements

* Fine-Tuning MobileNetV2 Layers
* Hyperparameter Optimization
* Experiment Tracking with MLflow
* Docker Containerization
* FastAPI Inference API
* ONNX Model Conversion
* Explainable AI using Grad-CAM
* Cloud Deployment (AWS/GCP/Azure)

---

## 👨‍💻 Author

### Muhammad Rizky Abdillah

Aspiring AI Engineer | Machine Learning Engineer | Computer Vision Enthusiast

**LinkedIn:** https://linkedin.com/in/rzkyabdlh

**GitHub:** https://github.com/N0tFuhny

---

⭐ If you found this project useful, consider giving it a star.
