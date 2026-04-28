# 😴 Drowsiness Alert System (Computer Vision Project)

A real-time computer vision system that detects driver drowsiness using facial landmarks and Eye Aspect Ratio (EAR) analysis.

---

## 📌 Project Overview

This project uses facial landmark detection and mathematical analysis to monitor eye behavior in real-time and trigger an alert when signs of drowsiness are detected.

It is based on:

* Facial landmark detection
* Eye Aspect Ratio (EAR) calculation
* Real-time video processing
* Audio alert system

---

## 🚧 Project Status: **🟡 IN PROGRESS**

This project is currently under development.

### Completed:

* Webcam setup using OpenCV
* Facial landmark detection implemented
* Eye region extraction

### In Progress:

* EAR threshold tuning
* Alert system optimization
* Full system integration

---

## 📂 Project Structure

```bash
Drowsiness-Alert-System/
│
├── notebooks/
│   └── task_2_1_webcam_landmarks.ipynb
│
├── src/
│   ├── utils/
│   └── models/
│
├── assets/
│   ├── audio/
│   └── images/
│
├── outputs/
│   ├── videos/
│   └── screenshots/
│
├── requirements.txt
└── README.md
```

---

## 🎯 Objectives

### Task 2.1 – Facial Landmark Mapping

* Capture live webcam feed
* Detect face landmarks using MediaPipe / dlib
* Highlight eye regions in real time

---

### Task 2.2 – Eye Aspect Ratio (EAR)

* Extract key eye landmarks
* Compute EAR using Euclidean distance
* Display real-time EAR values

---

### Task 2.3 – Alert System

* Define EAR threshold
* Track consecutive frames
* Trigger audio alarm when drowsiness is detected

---

## 🛠️ Tools & Technologies

* Python
* OpenCV (cv2)
* MediaPipe / dlib
* NumPy
* SciPy
* Pygame / playsound

---

## 🧠 Key Concepts

* Computer Vision
* Facial Landmark Detection
* Feature Extraction
* Real-time Video Processing
* Threshold-based Alert Systems

---

## 📊 Expected Output

* Live webcam feed
* Eye landmarks displayed in real-time
* EAR value shown on screen
* Alarm triggered when eyes remain closed

---

## 🔮 Future Improvements

* Improve accuracy using deep learning models
* Add mobile deployment version
* Optimize real-time performance
* Add fatigue detection beyond eye tracking

---

## 👨‍💻 Author

Imraan Muhammad Sani

---
