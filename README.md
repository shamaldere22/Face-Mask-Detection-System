# Face Mask Detection System using Deep Learning 😷

## 📌 Project Overview
This project is an AI-based solution designed to detect whether a person is wearing a face mask in real-time. It uses **Computer Vision (OpenCV)** and **Deep Learning (TensorFlow/Keras)** to classify faces into two categories: **'MASK'** and **'NO MASK'**. This can be used for automated safety monitoring in public places.

## 📊 Dataset Information
The model was trained using the **Face Mask Detection dataset from Kaggle**.
- **Source:** [Kaggle - Face Mask Detection](https://www.kaggle.com)

- **Content:** Images of people with and without masks.
- **Preprocessing:** Images were resized to **100x100 pixels** and normalized (scaled by 1/255) to ensure faster and more accurate model training.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** 
  - **Deep Learning:** TensorFlow, Keras
  - **Computer Vision:** OpenCV
  - **Data Manipulation:** NumPy
  - **OS:** Python OS module for file handling

## 🏗️ Model Architecture
The project utilizes a **Convolutional Neural Network (CNN)** with the following layers:
1. **Conv2D Layer:** 32 filters, 3x3 kernel, ReLU activation.
2. **MaxPooling2D:** 2x2 pool size to reduce spatial dimensions.
3. **Conv2D Layer:** 64 filters, 3x3 kernel, ReLU activation.
4. **MaxPooling2D:** 2x2 pool size.
5. **Flatten Layer:** To convert 2D data into a 1D vector.
6. **Dense Layer:** 128 units with ReLU activation.
7. **Output Layer:** 2 units with **Softmax activation** for binary classification.

## 🚀 Key Features
- **End-to-End Pipeline:** Covers everything from image loading and preprocessing to model saving.
- **Real-time Detection:** Integrated with a webcam using OpenCV to provide live predictions.
- **High Performance:** Achieved near-perfect accuracy on the training data.
- **Automation:** The system automatically highlights the detected face with a green (MASK) or red (NO MASK) label.

## 📂 Project Structure
- `Face_Mask_Detection.ipynb`: Full training code and logic.
- `mask_model.h5`: The saved trained model (Legacy HDF5 format).
- `README.md`: Project documentation and setup guide.

## 📝 How to Run
1. Install dependencies: `pip install tensorflow opencv-python numpy`
2. Download the dataset from the Kaggle link provided.
3. Run the training script to generate `mask_model.h5`.
4. Run the real-time detection script to start the webcam feed.

---
**Developed by Shamal Dere**
