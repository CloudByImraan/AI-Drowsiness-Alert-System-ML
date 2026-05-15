🎤 PRESENTATION SLIDE STRUCTURE
 AI Drowsiness Alert System
Real-Time Driver Fatigue Detection Using Computer Vision

SLIDE 1 — TITLE PAGE
 AI Drowsiness Alert System
Real-Time Driver Fatigue Detection Using Computer Vision
Presented By:
Imran Muhammad Sani
Comrade Inusa Emmanuel

SLIDE 2 — INTRODUCTION
📌 Introduction
Driver fatigue and micro-sleep are major causes of road accidents worldwide.
Many accidents occur because drivers become sleepy without realizing it.
This project was developed to create a real-time intelligent monitoring system that detects signs of drowsiness using:

Artificial Intelligence (AI)
Computer Vision
Facial Landmark Detection
The system monitors eye behavior through a webcam and alerts the driver before falling asleep.

SLIDE 3 — SITUATION (STAR METHOD)
🟦 Situation
Many road accidents are caused by:

Driver fatigue
Long driving hours
Lack of sleep
Micro-sleep during driving
There was a need for a system that could:

Monitor the driver in real time
Detect signs of drowsiness early
Warn the driver before dangerous situations occur

SLIDE 4 — TASK (STAR METHOD)
🟨 Task
The main objectives of this project were to:

Access live webcam video
Detect facial landmarks in real time
Isolate eye regions
Calculate Eye Aspect Ratio (EAR)
Detect eye closure duration
Differentiate blinking from drowsiness
Trigger an alarm during prolonged eye closure

Additional Features Implemented
✅ Adaptive Thresholding
✅ Timer-Based Detection
✅ Real-Time Audio Alert System

SLIDE 5 — TECHNOLOGIES & WORKFLOW
🛠️ Technologies Used
Programming Language

Python
Libraries Used
OpenCV
MediaPipe
NumPy
SciPy
Playsound
Concepts Applied
Computer Vision
Facial Landmark Detection
Feature Extraction
Real-Time Video Processing
Eye Aspect Ratio (EAR)

🖥️ System Workflow
Webcam Input---Face Detection---Facial Landmark Mapping---Eye Landmark Extraction---EAR Calculation---Adaptive Threshold Calibration---Eye Closure Detection ---Timer-Based Validation---Alarm Trigger

SLIDE 6 — ACTION (PART 1)
🟩 Action — Facial Landmark Detection
The system uses:

OpenCV for webcam access
MediaPipe Face Mesh for facial landmark detection
What the System Detects
468 facial landmarks
Real-time eye landmark coordinates
Facial movement tracking

The webcam continuously monitors the driver's face and eye movement.
📷 (Insert Facial Landmark Screenshot Here)

SLIDE 7 — ACTION (PART 2)
🟩 Action — EAR Calculation
The Eye Aspect Ratio (EAR) was used to determine whether the eyes are open or closed.
EAR Formula

📊 EAR Interpretation
Eye StateEAR Behavior👁️ Eyes OpenHigher EAR values👀 BlinkingTemporary EAR drop😴 Eyes ClosedEAR drops below threshold
The EAR value changes dynamically depending on eye movement.
📷 (Insert EAR Screenshot Here)

SLIDE 8 — ACTION (PART 3)
🟩 Action — Adaptive Threshold & Timer Logic
To reduce false alarms and improve accuracy, we implemented:
✅ Adaptive Thresholding
✅ Timer-Based Eye Closure Detection

How It Works
Adaptive Thresholding
The system first observes the user’s normal eye state
Multiple EAR samples are collected
A personalized threshold is generated automatically
Timer Logic
Short eye closure → Blink
Long eye closure (4+ seconds) → Drowsiness
This helped reduce false positives caused by normal blinking.

SLIDE 9 — ADAPTIVE THRESHOLD DEMONSTRATION
🟩 Adaptive Threshold Demonstration
The system first performs a calibration stage before monitoring begins.
During calibration:

Multiple EAR samples are collected
The average EAR is calculated
A personalized adaptive threshold is generated
This allows the system to adapt to:
Different eye shapes
Small eyes
Lazy eyes
Individual facial differences

Calibration Stages
📷 Screenshot 1
CALIBRATING...KEEP EYES OPENCollecting Samples: 62/100Current EAR: 0.355
📷 Screenshot 2
Calibration CompleteAverage EAR: 0.356Adaptive Threshold: 0.268
📷 Screenshot 3
EAR: 0.141Threshold: 0.268

SLIDE 10 — RESULT
🟥 Result
Project Outcome
✅ Successfully detected facial landmarks in real time
✅ EAR updated dynamically during monitoring
✅ Differentiated blinking from drowsiness
✅ Triggered audio alarm during prolonged eye closure
✅ Worked successfully on standard laptop hardware

Final Output
The system can monitor a driver in real time and warn them before falling asleep.
📷 (Insert Drowsiness Alert Screenshot Here)

SLIDE 11 — REAL-WORLD TESTING & LIMITATIONS
🟨 Real-World Testing
The project was tested under different real-world conditions to evaluate performance and reliability.

Successful Cases
✅ Bright environment
✅ Normal indoor lighting
✅ Direct face visibility

Challenging Cases
⚠️ Dark environments reduced accuracy
⚠️ Glasses sometimes affected eye landmark detection
⚠️ Partial face obstruction affected tracking
These observations helped identify areas for future improvement.
📷 (Insert Bright Environment Screenshot Here)
📷 (Insert Dark Environment Screenshot Here)
📷 (Insert Glasses Screenshot Here)

SLIDE 12 — LIMITATIONS & FUTURE IMPROVEMENTS
⚠️ Current Limitations
The current system mainly focuses on:

Eye behavior monitoring
EAR-based drowsiness detection
Existing Limitations
No yawning detection yet
No head pose estimation
Performance reduces under poor lighting
Webcam quality affects detection accuracy
Glasses or occlusion may reduce reliability

 Future Improvements
Future versions may include:
Yawning detection
Head pose estimation
Deep learning-based fatigue classification
Mobile deployment
Edge AI deployment
Smart vehicle dashboard integration
Cloud-based monitoring systems

SLIDE 13 — DEPLOYMENT & CONCLUSION
🌍 Deployment & Real-World Applications
This project belongs to the fields of:

Artificial Intelligence (AI)
Computer Vision
Human Monitoring Systems
Embedded Safety Systems
Possible Deployment Areas
Smart vehicles
Driver assistance systems
Transportation safety systems
Industrial machine monitoring
Edge AI cameras
Smart surveillance systems

🖥️ Project Type
Real-Time AI & Computer Vision Monitoring System
The project combines:
AI-based facial analysis
Real-time video processing
Human behavior monitoring
Intelligent alert systems

✅ Conclusion
This project demonstrates how Artificial Intelligence and Computer Vision can improve safety by detecting driver drowsiness in real time.
The system provides a strong foundation for future intelligent driver-assistance technologies.