# Brain Tumor Detection Using Deep Learning (CNN)

## Overview

Brain Tumor Detection Using Deep Learning is a web-based application designed to assist in the automated detection and classification of brain tumors from MRI images. The system utilizes a Convolutional Neural Network (CNN) trained on MRI scan datasets to identify tumor types and provide predictions with confidence scores.

The application combines a FastAPI backend for model inference and a React-based frontend for an intuitive user experience, enabling users to upload MRI scans and receive real-time predictions.

---

## Features

* Upload MRI images through a user-friendly web interface.
* Automated brain tumor detection using a trained CNN model.
* Real-time prediction and classification.
* Confidence score generation for each prediction.
* FastAPI-powered REST API for model serving.
* React frontend for seamless interaction.
* Image preprocessing and normalization before prediction.

---

## Tech Stack

### Backend

* Python
* FastAPI
* TensorFlow / Keras
* OpenCV
* NumPy
* Pandas
* Pillow (PIL)
* Uvicorn

### Frontend

* React.js
* Vite
* Axios
* HTML5
* CSS3
* JavaScript

### Machine Learning

* Convolutional Neural Networks (CNN)
* Image Preprocessing
* Deep Learning
* Computer Vision

---

## System Architecture

```text
MRI Image
    │
    ▼
Image Preprocessing
    │
    ▼
CNN Model
    │
    ▼
FastAPI Backend
    │
    ▼
Prediction Result
    │
    ▼
React Frontend
```

---

## Project Structure

```text
Brain-Tumor-Detection/
│
├── backend/
│   ├── main.py
│   ├── predict.py
│   ├── requirements.txt
│   ├── model/
│   │   └── brain_tumor_model.h5
│   └── utils/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── screenshots/
│   ├── homepage.png
│   └── prediction result.png
│
├── README.md
└── .gitignore
```

---

## Dataset

The model was trained on publicly available MRI brain tumor datasets containing multiple categories of brain scans. The dataset consists of MRI images categorized into different tumor classes and normal brain scans.

### Data Preprocessing

* Image resizing
* Normalization
* Data cleaning
* Feature extraction
* Train-test split

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/Brain-Tumor-Detection.git

cd Brain-Tumor-Detection
```

---

### Backend Setup

```bash
cd backend

pip install -r requirements.txt

uvicorn main:app --reload
```

The backend server will start at:

```text
http://127.0.0.1:8000
```

---

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

The frontend application will start at:

```text
http://localhost:5173
```

---

## API Endpoint

### Predict Tumor

**Endpoint**

```http
POST /predict
```

### Input

MRI Image File

### Sample Response

```json
{
  "prediction": "Glioma",
  "confidence": 96.8
}
```

---

## Screenshots

### Home Page

<img width="1895" height="1078" alt="homepage" src="https://github.com/user-attachments/assets/3ef76ca1-84fd-4501-83fd-c68d21428f54" />


### Prediction Result

<img width="1918" height="1076" alt="prediction result" src="https://github.com/user-attachments/assets/c6bf7947-3dcb-4149-bc9c-31ecb82899cc" />


---

## Results

The trained CNN model successfully classifies MRI scans and provides predictions with confidence scores. Performance was evaluated using standard machine learning metrics such as:

* Accuracy
* Precision
* Recall
* F1 Score

---

## Future Enhancements

* Improve classification accuracy using advanced architectures.
* Deploy the application on cloud platforms.
* Add Explainable AI (XAI) visualizations.
* Support multiple MRI formats.
* Develop a mobile application version.
* Integrate patient report generation.

---

## Learning Outcomes

Through this project, the following skills were developed:

* Deep Learning Model Development
* Convolutional Neural Networks (CNN)
* Computer Vision
* Image Processing
* REST API Development
* Full-Stack Web Development
* FastAPI Integration
* React Frontend Development
* Model Deployment Concepts

---

## License

This project is developed for educational and research purposes.
