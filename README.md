# CIFAR-10 Image Classification Web App

A deep learning web application that classifies images into 10 CIFAR-10 categories using a **CNN model built from scratch**, trained and deployed using **Flask**.  
The project also includes a **transfer learning model using VGG16** for performance comparison.

---

## ✅ Features

- 🧠 Deployed CNN model built from scratch using TensorFlow
- 🧪 Transfer learning experiment using VGG16 included in the project
- 🖼️ Upload and classify images via web interface
- 🔍 Predicts one of the 10 CIFAR-10 classes:
  - `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`
- 📊 Displays prediction confidence with a bar chart (Chart.js)
- 🌐 Responsive UI styled with Tailwind CSS

---

## 📂 Project Files

| File | Description |
|------|-------------|
| `cifar10_best_model.h5` | Trained CNN model (used in deployment) |
| `deploy.py` | Flask backend for serving predictions |
| `index.html` | Frontend web interface |
| `VGG16_transform_learning.ipynb` | VGG16-based transfer learning implementation |

---

## ⚙️ Setup Instructions

1. **Install dependencies:**
   ```bash
   pip install flask flask-cors tensorflow pillow numpy
   ```

2. **Start the Flask app:**
   ```bash
   python deploy.py
   ```

3. **Open in your browser:**
   ```
   http://localhost:5000
   ```

---

## 🧪 Model Summary

- **CNN Model:**
  - Custom architecture built from scratch
  - Trained on CIFAR-10 dataset (32×32 RGB images)
  - Output: 10-class softmax probabilities

- **VGG16 Transfer Learning:**
  - Pre-trained VGG16 model with modified top layers
  - Fine-tuned on CIFAR-10 for comparison

---

## 📌 Notes

- All uploaded images are resized and normalized automatically.
- CORS is enabled for local frontend-backend integration.
- The web interface is built with HTML, Tailwind CSS, and Chart.js.
