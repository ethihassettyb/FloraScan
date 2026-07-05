<h1 align="center">🌿 FloraScan - AI-Based Plant Disease Detection System</h1>

<p align="center">
An intelligent web application that leverages deep learning to identify plant diseases from leaf images and provide actionable insights for crop health management.
</p>

---

## 📖 Overview

FloraScan is a web-based plant disease diagnosis system developed using Flask and a VGG19 transfer learning model. The application enables users to upload plant leaf images, detect diseases with high accuracy, and receive detailed information including symptoms, possible causes, and recommended remedies.

The project demonstrates the practical application of Artificial Intelligence and Computer Vision in agriculture by offering a simple and efficient solution for early disease detection.

---

## ✨ Key Features

* 🌱 Plant disease detection using a VGG19 deep learning model
* 📷 Upload leaf images through an intuitive web interface
* 🔍 Prediction across 38 plant disease categories
* 📄 Automatic PDF report generation
* 💊 Displays disease symptoms and treatment recommendations
* ⚡ Fast and responsive Flask-based web application
* 📁 Automatically stores prediction history and generated reports

---

## 🛠 Technologies Used

* Python
* Flask
* TensorFlow / Keras
* VGG19 Transfer Learning
* HTML5
* CSS3
* JavaScript

---

## 📂 Dataset

This project uses the **New Plant Diseases Dataset (Augmented)** available on Kaggle.

The dataset is not included in this repository because of its size. It can be downloaded separately for model training.

---

## 🤖 Model Details

* Architecture: VGG19
* Framework: TensorFlow / Keras
* Input Resolution: 256 × 256
* Number of Classes: 38
* Transfer Learning Approach

---

## 🚀 Getting Started

1. Create a virtual environment.
2. Install the required dependencies.
3. Place the trained model file inside the project directory.
4. Run:

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:5000
```

---

## 📁 Project Structure

```text
FloraScan/
│
├── app.py
├── disease_info.py
├── requirements.txt
├── README.md
├── templates/
├── static/
└── notebooks/
```

---

## 👨‍💻 Developer

**Ethihas Setty**

Bachelor of Computer Applications (BCA)

AI & Machine Learning Enthusiast

---

## 📌 Disclaimer

This project was developed for educational and academic purposes to demonstrate the application of deep learning techniques in plant disease identification.

---

⭐ If you found this project useful, consider giving the repository a star!
