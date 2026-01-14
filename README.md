# **Drowsiness Detection Model**


## 📌 Overview

Driver drowsiness is a major contributor to road accidents, often preceded by signs such as prolonged eye closure, yawning, or abnormal head posture. Detecting these indicators early can significantly improve driver safety.

This project implements a real-time drowsiness detection system using computer vision and deep learning to analyze facial behavior from a live video stream. By combining modern object detection with classical vision techniques, the system identifies fatigue-related cues and triggers an auditory alert when drowsiness is detected.

The repository serves as both a functional safety prototype and a demonstration of real-time AI system integration, highlighting skills in deep learning, video processing, and applied computer vision.

## Features
🎥 Real-Time Video Stream Processing

 - Captures and processes live video frames using OpenCV
  
 - Optimized for low-latency inference to enable near-instantaneous alerts
  
 - Suitable for webcam-based or embedded camera setups

👤 Robust Face Detection Pipeline

 - YOLOv8 is used for fast and accurate full-face detection
  
 - Haar Cascade classifiers provide complementary detection for facial regions
  
 - Multi-model approach increases reliability under varying lighting and head poses

😴 Multi-Metric Drowsiness Detection

 - The system monitors three primary behavioral indicators:
  
 - Eye Closure Detection
  
 - Tracks eye visibility across frames
  
 - Identifies prolonged closure patterns associated with fatigue
  
 - Head Tilt Analysis
  
 - Detects abnormal head orientation or downward tilting
  
 - Useful for identifying micro-sleep or loss of posture control
  
 - Yawning Detection
  
 - Monitors mouth opening patterns
  
 - Detects frequent or extended yawns as a fatigue signal

🔊 Auditory Alert System

 - Integrates Pygame to play real-time warning sounds
  
 - Alerts are triggered when drowsiness thresholds are exceeded
  
 - Designed to immediately regain driver attention

## Technical Architecture

Camera Input (OpenCV)
        ↓
Frame Preprocessing
        ↓
Face Detection (YOLOv8 / Haar Cascade)
        ↓
Facial Feature Evaluation
        ↓
Heuristic Drowsiness Rules
        ↓
Audio Alert (Pygame)

 ## 📊 Drowsiness Detection Methodology

The system evaluates multiple visual indicators on a per-frame basis:

- Eye Closure: Detects whether eyes appear open or closed in the current frame

- Head Tilt: Identifies abnormal head orientation or downward posture

- Yawning: Detects mouth opening patterns associated with fatigue

Alerts are triggered when one or more indicators exceed predefined thresholds. While the system does not use temporal aggregation or sequence-based models, combining multiple cues improves robustness compared to single-indicator detection.

## 🧩 Use Cases

- Driver safety monitoring prototypes

- Research and experimentation in computer vision–based fatigue detection

- Human behavior analysis projects

- Educational demonstrations of real-time AI systems

- Foundations for more advanced driver monitoring solutions

## 🚀 Future Improvements

Potential extensions include:

- Temporal thresholds (e.g., sustained eye closure over time)

- Facial landmark–based eye and mouth metrics

- Sequence modeling with LSTM or temporal CNNs

- Improved robustness under low-light conditions

- Deployment on embedded platforms (Jetson, Raspberry Pi)
