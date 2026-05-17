#  AI Drowsiness Detection System

A real-time Computer Vision and AI-based monitoring system that detects signs of drowsiness using facial landmark tracking and Eye Aspect Ratio (EAR) analysis.

The system continuously monitors eye movement through a webcam and triggers an alert when prolonged eye closure is detected.

---

# 🚧 Project Status

 **Project Currently In Progress**

This project is still being actively improved and expanded with more advanced Computer Vision and AI features.

💡 This project demonstrates an early-stage intelligent driver monitoring system and can be further enhanced with additional AI-powered safety features.

📌 Current implementation focuses mainly on eye-based drowsiness detection using adaptive thresholding and timer-based logic.

---

# 📌 Project Overview

Driver fatigue and micro-sleep are major causes of road accidents worldwide.

This project was developed to provide a non-intrusive real-time monitoring system capable of detecting prolonged eye closure and warning the user before dangerous situations occur.

The system combines:

* Computer Vision
* Facial Landmark Detection
* Eye Aspect Ratio (EAR)
* Adaptive Thresholding
* Real-Time Webcam Processing
* Timer-Based Drowsiness Logic

The application captures live webcam input, analyzes eye behavior frame-by-frame, and activates an alert when drowsiness is detected.

---

# 🌍 Main Purpose of the Project

The major purpose of this project is to improve safety by reducing accidents caused by driver fatigue and micro-sleep.

This type of system can be used in:

* Smart transportation systems
* Driver monitoring systems
* Industrial machine monitoring
* Safety surveillance systems
* Smart vehicles and embedded AI systems

The project demonstrates how Artificial Intelligence and Computer Vision can be used to monitor human behavior in real time and provide instant safety alerts.

---

# 🎯 Current Objectives (Current Development Focus)

This project is still evolving.
The following are the major components currently implemented in this version of the system:

* Detect facial landmarks in real time
* Isolate and monitor eye regions
* Calculate Eye Aspect Ratio (EAR)
* Differentiate blinking from drowsiness
* Implement adaptive threshold calibration
* Trigger alerts during prolonged eye closure
* Perform real-time webcam monitoring

📌 These represent the current development focus of the project and form the foundation for future improvements.

---

# 🧠 Tech Stack

| Technology          | Description                         | Contribution to Project                                                        |
| ------------------- | ----------------------------------- | ------------------------------------------------------------------------------ |
| Python              | High-level programming language     | Used as the core programming language for implementing the entire system logic |
| OpenCV (cv2)        | Computer Vision library             | Used for webcam access, image processing, frame handling, and visual display   |
| MediaPipe Face Mesh | Facial landmark detection framework | Used to detect 468 facial landmarks and isolate eye regions                    |
| NumPy               | Numerical computing library         | Used for mathematical operations and array processing                          |
| SciPy               | Scientific computing library        | Used for Euclidean distance calculation in EAR computation                     |
| PlaySound           | Audio playback library              | Used to trigger alarm sound during drowsiness                                  |
| Jupyter Notebook    | Interactive notebook environment    | Used for development, testing, experimentation, and visualization              |

---

# 🖥️ System Workflow

```text
                 ┌────────────────────┐
                 │   Webcam Input     │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Face Detection     │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Facial Landmark    │
                 │ Mapping (468 pts)  │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Eye Landmark       │
                 │ Extraction         │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ EAR Calculation    │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Adaptive Threshold │
                 │ Calibration        │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Eye Closure        │
                 │ Detection          │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Timer Validation   │
                 └─────────┬──────────┘
                           ↓
                 ┌────────────────────┐
                 │ Alarm Trigger      │
                 └────────────────────┘
```

---

# 📂 Project Structure

```bash
Drowsiness-Alert-System/
│
├── notebooks/
│   ├── task_2_1_webcam_landmarks.ipynb
│   ├── task_2_2_ear_calculation.ipynb
│   └── task_2_3_drowsiness_alert_adaptive.ipynb
│
├── assets/
│   └── audio/
│       └── alarm.wav
│
├── outputs/
│   ├── screenshots/
│   └── videos/
│
├── src/
│   ├── models/
│   └── utils/
│
├── requirements.txt
└── README.md
```

## 📁 Folder Explanation

| Folder/File                              | Purpose                                                   |
| ---------------------------------------- | --------------------------------------------------------- |
| notebooks/                               | Contains all Jupyter notebooks used during development    |
| task_2_1_webcam_landmarks.ipynb          | Handles webcam access and facial landmark detection       |
| task_2_2_ear_calculation.ipynb           | Implements Eye Aspect Ratio (EAR) calculation             |
| task_2_3_drowsiness_alert_adaptive.ipynb | Implements adaptive thresholding and drowsiness detection |
| assets/audio/                            | Stores alarm sound files                                  |
| alarm.wav                                | Audio alert triggered during drowsiness                   |
| outputs/screenshots/                     | Stores project screenshots and visual outputs             |
| outputs/videos/                          | Stores demo videos and recordings                         |
| src/models/                              | Reserved for future AI/ML model integration               |
| src/utils/                               | Reserved for utility/helper functions                     |
| requirements.txt                         | Contains required project libraries                       |
| README.md                                | Project documentation                                     |

---

# ⚙️ Setup & Installation Guide

## 1️⃣ Create Project Folder

```bash
Drowsiness-Alert-System
```

---

## 2️⃣ Open Terminal Inside Project Folder

Using File Explorer:

* Open the project folder
* Click the address bar
* Type:

```bash
cmd
```

* Press Enter

---

## 3️⃣ Create Virtual Environment

```bash
python -m venv venv
```

---

## 4️⃣ Activate Virtual Environment

```bash
venv\Scripts\activate
```

---

# 📦 Install Required Libraries

```bash
pip install opencv-python mediapipe numpy scipy matplotlib jupyter ipykernel playsound==1.2.2
```

---

# 🔧 MediaPipe Version Fix

```bash
pip uninstall mediapipe -y
```

```bash
pip install mediapipe==0.10.9
```

---

# 📓 Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# 📝 Create Notebook Files

```text
task_2_1_webcam_landmarks.ipynb
task_2_2_ear_calculation.ipynb
task_2_3_drowsiness_alert_adaptive.ipynb
```

---

# ▶️ How to Run the Project

1. Activate virtual environment

```bash
venv\Scripts\activate
```

2. Launch Jupyter Notebook

```bash
jupyter notebook
```

3. Open:

```text
task_2_3_drowsiness_alert_adaptive.ipynb
```

4. Run all notebook cells sequentially

5. Ensure webcam access is enabled

6. Keep eyes open during calibration stage

7. System begins monitoring automatically

---

# 👁️ Facial Landmark Detection

MediaPipe Face Mesh is used to detect facial landmarks in real time.

The system detects:

* 468 facial landmarks
* Eye landmark coordinates
* Real-time facial movement

Specific landmarks around the eyes are continuously extracted for eye monitoring and EAR calculation.

---

# 📐 Eye Aspect Ratio (EAR)

The Eye Aspect Ratio (EAR) is a mathematical formula used to determine whether the eyes are open or closed.

The formula compares:

* Vertical eye distances
* Horizontal eye width

## EAR Formula

<img width="943" height="787" alt="EAR FORMULAR" src="https://github.com/user-attachments/assets/fa591949-852a-4a34-9647-dda339acea27" />


# 📊 EAR Interpretation

| Eye State      | EAR Behavior              |
| -------------- | ------------------------- |
| 👁️ Eyes Open  | Higher EAR values         |
| 👀 Blinking    | Temporary EAR drop        |
| 😴 Eyes Closed | EAR drops below threshold |

---

# 🧩 Adaptive Thresholding

Instead of using one fixed threshold for all users, the system performs adaptive threshold calibration.

This allows the system to personalize detection for different eye shapes and facial structures.

---

## 🔍 Adaptive Thresholding Process

### Step 1 — Calibration Phase

During startup:

* The system requests the user to keep eyes open
* EAR samples are collected continuously
* 100 frames are collected

```text
Collecting Samples: 100/100
```

---

### Step 2 — Average EAR Calculation

The system computes the average EAR value from collected samples.

## Average EAR Formula

Where:

* (EAR_i) = EAR value for each frame
* (N) = Total number of frames collected

---

### Step 3 — Adaptive Threshold Generation

The personalized threshold is generated using:

## Adaptive Threshold Formula

The constant 0.75 is used as a scaling factor to determine the eye-closure boundary.

---

# ⏱️ Timer-Based Drowsiness Logic

The system does not immediately classify blinking as drowsiness.

---

## Logic Used

### If:

```text
EAR < Adaptive Threshold
```

The eyes are considered closed.

---

### Then:

A timer starts counting how long the eyes remain closed.

---

## Decision Logic

| Eye Closure Duration       | System Decision |
| -------------------------- | --------------- |
| Short Duration             | Blink           |
| Long Duration (4+ seconds) | Drowsiness      |

---

# 🔊 Alarm System

When prolonged eye closure is detected:

* A visual alert appears on screen
* An alarm sound is triggered automatically

This acts as an immediate safety warning mechanism.

---

# 📸 Visual Results

## Facial Landmark Detection

<img width="1919" height="1079" alt="FACIAL LANDMARK" src="https://github.com/user-attachments/assets/79c8ca9a-25ea-43f2-b479-17c336860be1" />


Brief Description:

* Shows real-time facial landmark mapping
* Demonstrates eye region tracking using MediaPipe

---

## EAR Monitoring

<img width="1919" height="1068" alt="EAR MONITORING" src="https://github.com/user-attachments/assets/65c1c189-8d33-42c5-9c6f-f53bde18892f" />


Brief Description:

* Shows EAR values changing dynamically
* Demonstrates eye-open and eye-closed states

---

## Adaptive Threshold Calibration

<img width="1914" height="1079" alt="CALIBRATION PROCESS" src="https://github.com/user-attachments/assets/54792820-430f-4413-8500-f85d11942250" />


Brief Description:

* Shows calibration stage during sample collection
* System observes user's normal eye behavior

---

## Calibration Complete

<img width="1919" height="1079" alt="COMPLETED CALIBRATION" src="https://github.com/user-attachments/assets/d1b34c3f-cc53-4ebc-bd53-9ae86b94f416" />


Brief Description:

* Displays calculated Average EAR
* Displays generated Adaptive Threshold

---

## Drowsiness Alert Detection

<img width="1919" height="1079" alt="DROWSINESS DETECTION" src="https://github.com/user-attachments/assets/cfebcaa2-7f54-4ae7-9f94-c74dbb1f2dff" />


Brief Description:

* Shows prolonged eye closure detection
* Alarm triggered after timer validation

---

# ✅ Features

* Real-time webcam monitoring
* Facial landmark detection
* EAR calculation
* Adaptive threshold calibration
* Blink vs drowsiness differentiation
* Audio alert system
* Real-time video processing

---

# ⚠️ Current Limitations

Although functional, the system still has some limitations:

* Focuses mainly on eye behavior
* Does not yet detect yawning
* No head pose estimation
* Performance may reduce under poor lighting
* Webcam quality may affect detection accuracy
* Glasses or occlusion may reduce reliability

---

# 🚀 Possible Improvements

Future versions may include:

* Head pose estimation
* Yawning detection
* Deep learning-based fatigue classification
* Mobile deployment
* Edge AI deployment (Raspberry Pi / Jetson Nano)
* Smart vehicle dashboard integration
* Cloud-based monitoring systems

---

# 🌍 Real-World Applications

Possible deployment areas include:

* Smart vehicles
* Driver assistance systems
* Transportation safety systems
* Industrial machine monitoring
* Edge AI cameras
* Smart surveillance systems

---

# 🖥️ Project Type

## Real-Time Computer Vision & AI Monitoring System

The project combines:

* AI-based facial analysis
* Real-time video processing
* Human behavior monitoring
* Intelligent alert systems

---

# 📈 Future Deployment Possibilities

| Deployment Type         | Description                        |
| ----------------------- | ---------------------------------- |
| Desktop Application     | Local webcam monitoring            |
| Edge AI Device          | Raspberry Pi / Jetson Nano         |
| Smart Vehicle Dashboard | Automotive safety integration      |
| Mobile Application      | Smartphone camera monitoring       |
| IoT Monitoring System   | Cloud-connected fatigue monitoring |

---

# 📚 Learning Context

This project was developed as part of a practical learning journey involving:

* Computer Vision
* Real-time AI systems
* Facial feature extraction
* Human behavioral analysis
* Machine Learning concepts

---

# 🙏 Acknowledgement

This project was developed with the support of:

[NCAIR (National Centre for Artificial Intelligence and Robotics)](https://ncair.nitda.gov.ng/?utm_source=chatgpt.com) — An agency under [NITDA (National Information Technology Development Agency)](https://nitda.gov.ng/?utm_source=chatgpt.com) dedicated to advancing Artificial Intelligence, Robotics, and emerging technologies in Nigeria.

We extend our sincere gratitude to the entire NCAIR/NITDA program cohort for mentorship, collaboration, and technical guidance throughout the development of this project.

---

# 👨‍🏫 Program Facilitators

| Role                   | Name             | LinkedIn                                                                                         |
| ---------------------- | ---------------- | ------------------------------------------------------------------------------------------------ |
| Lead Facilitator       | Shaddai Adeniran | [Shaddai Adeniran LinkedIn](https://linkedin.com/in/shaddai-adeniran?utm_source=chatgpt.com)     |
| Supporting Facilitator | Stephen Ayuba    | [Stephen Ayuba LinkedIn](https://linkedin.com/in/stephen-ayuba?utm_source=chatgpt.com)           |
| Supporting Facilitator | Rizama Victor    | [Rizama Victor LinkedIn](https://linkedin.com/in/rizama-victor-b63266226?utm_source=chatgpt.com) |

---

# 👨‍💻 Contributors

* Imran Muhammad Sani
* Comrade Inusa Emmanuel

---

# 📄 License

This project is intended for educational, research, and learning purposes.
