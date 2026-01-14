# **Drowsiness Detection Model**


## 📌 Overview

Driver drowsiness is a major contributor to road accidents, often preceded by signs such as prolonged eye closure, yawning, or abnormal head posture. Detecting these indicators early can significantly improve driver safety.

This project implements a real-time drowsiness detection system using computer vision and deep learning to analyze facial behavior from a live video stream. By combining modern object detection with classical vision techniques, the system identifies fatigue-related cues and triggers an auditory alert when drowsiness is detected.

The repository serves as both a functional safety prototype and a demonstration of real-time AI system integration, highlighting skills in deep learning, video processing, and applied computer vision.

## Features
🎥 Real-Time Video Stream Processing

Captures and processes live video frames using OpenCV

Optimized for low-latency inference to enable near-instantaneous alerts

Suitable for webcam-based or embedded camera setups

👤 Robust Face Detection Pipeline

YOLOv8 is used for fast and accurate full-face detection

Haar Cascade classifiers provide complementary detection for facial regions

Multi-model approach increases reliability under varying lighting and head poses

😴 Multi-Metric Drowsiness Detection

The system monitors three primary behavioral indicators:

Eye Closure Detection

Tracks eye visibility across frames

Identifies prolonged closure patterns associated with fatigue

Head Tilt Analysis

Detects abnormal head orientation or downward tilting

Useful for identifying micro-sleep or loss of posture control

Yawning Detection

Monitors mouth opening patterns

Detects frequent or extended yawns as a fatigue signal

🔊 Auditory Alert System

Integrates Pygame to play real-time warning sounds

Alerts are triggered when drowsiness thresholds are exceeded

Designed to immediately regain driver attention
