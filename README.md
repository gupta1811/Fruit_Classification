# Fruit Classification using Custom CNN

This repository contains a Deep Learning project for classifying fruits using a Custom Convolutional Neural Network (CNN) trained on the Fruits-360 dataset. The goal is to design a lightweight, accurate model suitable for real-world applications such as automated sorting, smart farming, and quality inspection.

---

## 📌 Project Overview
Fruit classification is an important task in modern agriculture and retail automation. Manual classification is slow and inconsistent, whereas deep learning models provide high accuracy and speed.

This project builds a custom CNN architecture from scratch (no transfer learning models like VGG/ResNet). The model is trained on 100×100 RGB images and achieves high accuracy while maintaining low computational cost.

---

## 🎯 Objectives
- Build a CNN architecture optimized for fruit image classification.
- Train and evaluate the model on the Fruits-360 dataset.
- Achieve high accuracy with minimal model size.
- Compare performance with standard deep learning architectures.
- Create a fully reproducible pipeline using Jupyter Notebook.

---

## 📂 Dataset
**Dataset:** Fruits-360  
**Total Classes:** 228  
**Training Images:** ~108,000  
**Test Images:** ~40,000  
**Image Size:** 100×100  
**Augmentation:** rotation, horizontal flip, zoom, normalization

The dataset contains multiple fruit and vegetable categories with consistent backgrounds, enabling effective model training.

---

## 🧠 Custom CNN Architecture
The model consists of 4 convolutional blocks followed by dense layers:

- Conv2D layers with 32, 64, 128, 256 filters
- Batch Normalization
- MaxPooling layers
- Dropout for regularization
- Dense layer with 256 units
- Final Dense softmax layer for classification

This architecture is lightweight (~1.2M parameters) compared to VGG19 (~143M) or ResNet50 (~25M).

---

## 🚀 Methodology
1. Load and preprocess dataset  
2. Apply augmentation (rotation, zoom, flips)  
3. Train the custom CNN  
4. Track training and validation metrics  
5. Evaluate model on test dataset  
6. Compare performance with SOTA models  

---

## 📊 Results

### Training Performance
- Training Accuracy: 99.12%  
- Validation Accuracy: 98.88%  
- Training Loss: decreased from 1.45 to 0.04  
- Validation Loss: ~0.05  

### Test Performance
- Test Accuracy: 98.75%  
- Macro F1-Score: 0.98  

The model performs exceptionally well, even on visually similar fruits (e.g., multiple apple varieties).

---

## 🆚 Model Comparison

| Model              | Accuracy | Parameters | Notes |
|-------------------|----------|------------|-------|
| Custom CNN (ours) | 98.88%   | ~1.2M      | Fast, efficient |
| VGG19             | 98.20%   | 143M       | Very heavy |
| ResNet50          | 98.50%   | 25M        | Slower |
| MobileNetV2       | 97.90%   | 3.5M       | Lightweight |

### Why our model is better:
- Higher accuracy than VGG19 and MobileNet  
- Much smaller model size  
- Faster training time  
- Specifically optimized for Fruits-360  

---

## 👨‍🎓 Team Members
- Mridul Gupta  
- Rishabh Dhawan  
- Govinda  
- Devarshi Singh  

Submitted under the course:  
**Deep Learning and Applications (UEC642)**  
Thapar Institute of Engineering & Technology

---

## ⭐ If you found this project helpful, please consider giving the repository a star!
