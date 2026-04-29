# 😴 Drowsiness Alert System (Computer Vision Project)

A real-time computer vision system that detects driver drowsiness using facial landmarks and Eye Aspect Ratio (EAR) analysis.

---

## 📌 Project Overview

Driver fatigue is a major cause of road accidents. This project aims to detect signs of drowsiness in real-time by analyzing eye behavior using computer vision techniques.

The system uses:

* Facial landmark detection
* Feature extraction (eye regions)
* Eye Aspect Ratio (EAR) computation
* Real-time webcam processing
* Threshold-based alert mechanism

---

## 🚧 Project Status: 🟡 In Progress

### ✅ Completed

* Webcam integration using OpenCV
* Facial landmark detection using MediaPipe
* Eye region extraction
* Eye Aspect Ratio (EAR) calculation and live display

### 🔄 Upcoming

* EAR threshold logic
* Frame-based drowsiness detection
* Audio alert system integration

---

## 📂 Project Structure

```bash
Drowsiness-Alert-System/
│
├── notebooks/
│   ├── task_2_1_webcam_landmarks.ipynb
│   └── task_2_2_EAR_calculation.ipynb
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

## 🎯 Project Tasks

### 🔹 Task 2.1 — Webcam & Facial Landmark Mapping

* Access live webcam feed
* Detect facial landmarks using MediaPipe Face Mesh
* Extract and highlight eye regions in real-time

📌 **Outcome:**
Real-time face tracking with visible eye landmark points.

---

### 🔹 Task 2.2 — Eye Aspect Ratio (EAR) Calculation

* Extract 6 key landmarks per eye
* Compute EAR using Euclidean distance
* Display EAR value live on screen

📌 **Key Insight:**

* Eyes open → EAR ≈ 0.25 – 0.35
* Blink → EAR drops briefly
* Eyes closed → EAR < 0.20

📌 **Outcome:**
A dynamic EAR value that reflects eye state in real time.

---

### 🔹 Task 2.3 — Drowsiness Detection & Alert (Upcoming)

* Define EAR threshold (e.g., < 0.25)
* Track consecutive frames
* Trigger alarm when eyes remain closed

📌 **Expected Outcome:**
Automatic alert system when drowsiness is detected.

---

## ⚙️ Environment Setup

1. Create project folder

2. Open terminal inside folder:

   ```bash
   cmd
   ```

3. Create virtual environment:

   ```bash
   python -m venv venv
   ```

4. Activate environment:

   ```bash
   venv\Scripts\activate
   ```

5. Install dependencies:

   ```bash
   pip install opencv-python mediapipe numpy scipy matplotlib jupyter ipykernel
   ```

6. Fix MediaPipe issue:

   ```bash
   pip uninstall mediapipe -y
   pip install mediapipe==0.10.9
   ```

7. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

---

## 🛠️ Technologies Used

* Python
* OpenCV (cv2)
* MediaPipe
* NumPy
* SciPy
* Jupyter Notebook

---

## 🧠 Key Concepts

* Computer Vision
* Facial Landmark Detection
* Feature Extraction
* Geometric Analysis (EAR)
* Real-time Video Processing

---

## 📊 Expected Output

* Live webcam feed
* Eye landmarks displayed
* Real-time EAR value
* (Upcoming) Audio alert when drowsiness is detected

---

## 🔮 Future Improvements

* Deep learning-based eye state classification
* Improved robustness under low lighting
* Mobile or embedded system deployment
* Head pose and yawning detection

---

## 👨‍💻 Author

Imraan Muhammad Sani\

---
