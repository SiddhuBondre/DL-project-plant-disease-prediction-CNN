# DL-project-plant-disease-prediction-CNN

# 🌿 Plant Disease Prediction using CNN (Deep Learning)

This deep learning project uses **Convolutional Neural Networks (CNNs)** to automatically detect plant diseases from leaf images. The goal is to assist farmers and agronomists by providing an efficient, accurate, and scalable solution to identify crop diseases at early stages.

---

## 🧠 Problem Statement

Manual detection of plant diseases is time-consuming and error-prone. With advancements in computer vision and deep learning, we can automate the classification of diseases in plants using leaf image data.

---

## 📁 Dataset

- **Source**: [PlantVillage Dataset (Kaggle / offline)]  
- **Classes**: 38+ (depends on crop types: tomato, apple, potato, etc.)  
- **Image Format**: RGB (JPG/PNG)  
- **Categories**: Healthy and multiple disease classes  
- **Dataset Split**:
  - Training Set
  - Validation Set
  - Test Set (optional)

---

## 🔧 Technologies & Tools Used

- Python 3.x
- TensorFlow / Keras
- OpenCV / PIL
- NumPy, pandas
- Matplotlib, seaborn
- Google Colab / Jupyter Notebook

---

## 🧱 Project Structure

plant-disease-prediction/
│
├── dataset/ # Images organized by class folders
├── notebooks/ # Jupyter/Colab notebooks
├── models/ # Saved CNN model (.h5)
├── images/ # Sample prediction images
├── app/ # Optional: Streamlit or Flask app
├── plant_disease_cnn.py # Model training script
├── README.md # Project documentation
└── requirements.txt # Python dependencies



---

## 📊 Exploratory Data Analysis (EDA)

- Number of images per class
- Sample images visualization
- Image dimensions and quality
- Class imbalance check (bar plots)

---

## 🏗️ Model Architecture (CNN)

Basic CNN model (can be extended with Transfer Learning):

```text
Input Layer (image: 128x128x3)
↓
Conv2D + ReLU + MaxPooling
↓
Conv2D + ReLU + MaxPooling
↓
Flatten
↓
Dense Layer + ReLU
↓
Dropout
↓
Output Layer (Softmax for multiclass)


