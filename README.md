# CNN CIFAR-10 Image Classification System

### Web Interface

![Main Interface](/assets/website-screen.png)
*Main classification interface with drag-and-drop upload*

<!-- 
### Classification Results
![Results](/frontend/public/website-screen-result.png)
*Real-time classification results with confidence scores* -->

A comprehensive deep learning project that implements a Convolutional Neural Network (CNN) for image classification using the CIFAR-10 dataset. This project features both a Flask backend API and a modern Next.js frontend interface, providing a complete web application for image classification tasks.

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Live Demo](#live-demo)
- [Technical Details](#technical-details)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Project Overview

This project demonstrates the implementation of a deep learning-based image classification system using Convolutional Neural Networks (CNNs) on the CIFAR-10 dataset. The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck.

The system is designed as a full-stack web application with:
- **Backend**: Flask-based REST API for model inference
- **Frontend**: Modern Next.js interface for user interaction
- **Model**: Custom CNN architecture trained on CIFAR-10 dataset


## ✨ Features

- **Real-time Image Classification**: Upload images and get instant predictions
- **Modern Web Interface**: Responsive design with intuitive user experience
- **RESTful API**: Well-structured API endpoints for integration
- **Model Training**: Scripts for training custom CNN models
- **Academic Documentation**: Comprehensive technical documentation

## 🔧 Prerequisites

### System Requirements
- **Python**: 3.8+ (3.10+ recommended)
- **Node.js**: 16+ (18+ recommended)
- **Memory**: At least 4GB RAM (8GB+ recommended for training)
- **Storage**: 2GB+ free space

### Development Environment
- **OS**: Windows 10/11, macOS, or Linux
- **Package Managers**: pip, npm/yarn
- **IDE**: VS Code, PyCharm, or any preferred editor

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Barfoud-Fatima-Zohra/cnn-cifar10-classification.git
cd cnn-cifar10-classification
```

### 2. Backend Setup (Flask API)

#### Windows (PowerShell)
```powershell
# Navigate to backend directory
cd backend

# Create virtual environment
python -m venv .venv

# Activate virtual environment
.\.venv\Scripts\Activate.ps1

# Install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

#### macOS/Linux
```bash
cd backend
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### 3. Frontend Setup (Next.js)

```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install
```

## 🎮 Usage

### Starting the Backend Server
```bash
cd backend
# Activate virtual environment (if not already active)
.\.venv\Scripts\Activate.ps1  # Windows
# source .venv/bin/activate    # macOS/Linux

# Start Flask server
python app.py
```
The API will be available at `http://localhost:5000`

### Starting the Frontend Application
```bash
cd frontend
npm run dev
```
The web interface will be available at `http://localhost:3000`

### Training a New Model (Optional)
```bash
cd backend
python train_model.py
```
**Note**: Training requires significant computational resources and may take several hours without GPU acceleration.


## 🌐 Live Demo

- **Website**: [https://cnn-cifar10.vercel.app/](https://cnn-cifar10.vercel.app/)
- **GitHub Repository**: [link](https://github.com/Barfoud-Fatima-Zohra/cnn-cifar10-classification)

## 🔬 Technical Details

### Model Architecture
The CNN model consists of:
- **Input Layer**: 32x32x3 (RGB images)
- **Convolutional Layers**: Multiple Conv2D layers with ReLU activation
- **Pooling Layers**: MaxPooling2D for dimensionality reduction
- **Dense Layers**: Fully connected layers for classification
- **Output Layer**: 10 neurons (CIFAR-10 classes)

### Training Configuration
- **Dataset**: CIFAR-10 (60,000 images)
- **Epochs**: 10 (configurable)
- **Batch Size**: 32
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy

### Performance Metrics
- **Training Accuracy**: ~85%
- **Validation Accuracy**: ~80%

