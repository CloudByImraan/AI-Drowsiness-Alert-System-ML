# 😴 AI Drowsiness Detection System

A real-time Computer Vision and AI-based monitoring system that detects signs of drowsiness using facial landmark tracking and Eye Aspect Ratio (EAR) analysis.

The system continuously monitors eye movement through a webcam and triggers an alert when prolonged eye closure is detected.

---

## 🚧 Project Status

⚠️ **Project Currently In Progress**

This project is still being actively improved and expanded with more advanced Computer Vision and AI features.

💡 This project demonstrates my current approach and can be further enhanced with more advanced features and optimizations.

📌 Represents an early-stage implementation with room for future expansion.

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

# 🎯 Objectives

The main objectives of this project are to:

* Detect facial landmarks in real time
* Isolate and monitor eye regions
* Calculate Eye Aspect Ratio (EAR)
* Differentiate blinking from drowsiness
* Implement adaptive threshold calibration
* Trigger alerts during prolonged eye closure

---

# 🧠 Technologies Used

* Python
* OpenCV (cv2)
* MediaPipe Face Mesh
* NumPy
* SciPy
* PlaySound
* Jupyter Notebook

---

# 🖥️ System Workflow

```text id="drowflow1"
Webcam Input
      ↓
Face Detection
      ↓
Facial Landmark Mapping
      ↓
Eye Landmark Extraction
      ↓
EAR Calculation
      ↓
Adaptive Threshold Calibration
      ↓
Eye Closure Detection
      ↓
Timer-Based Validation
      ↓
Alarm Trigger
```

---

# 📂 Project Structure

```bash id="drowstruct1"
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

---

# 👁️ Facial Landmark Detection

MediaPipe Face Mesh is used to detect facial landmarks in real time.

Specific landmarks around the eyes are extracted continuously, enabling accurate tracking of eye movement during live webcam processing.

---

# 📐 Eye Aspect Ratio (EAR)

The Eye Aspect Ratio (EAR) is a mathematical formula used to determine whether the eyes are open or closed.

The formula compares:

* Vertical eye distances
* Horizontal eye width

### EAR Formula

```text id="earformula1"
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 ||p1 - p4||)
```

---

# 📊 EAR Interpretation

 | Eye State       | EAR Behavior              |
 | --------------  | ------------------------- |
 | 👁️ Eyes Open   | Higher EAR values         |
 | 👀 Blinking    | Temporary EAR drop        |
 | 😴 Eyes Closed | EAR drops below threshold |

---

# 🧩 Adaptive Thresholding

Instead of using a fixed threshold for all users, the system implements adaptive threshold calibration.

During startup:

* The system observes the user's normal eye behavior
* Calculates the average EAR
* Generates a personalized threshold value

This improves accuracy across different facial structures and eye shapes.

---

# ⏱️ Drowsiness Detection Logic

The system does not immediately classify blinking as drowsiness.

Instead:

* A timer starts when the eyes close
* If eye closure persists for several frames/seconds, the system classifies the state as drowsiness

This helps reduce false alarms caused by natural blinking.

---

# 🔊 Alert System

When prolonged eye closure is detected:

* A visual warning appears on screen
* An alarm sound is triggered automatically

This acts as an immediate safety warning mechanism.

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

This project belongs to the fields of:

* Artificial Intelligence (AI)
* Computer Vision
* Human Monitoring Systems
* Embedded Safety Systems

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

# 👨‍💻 Author

Imraan Muhammad Sani

---
