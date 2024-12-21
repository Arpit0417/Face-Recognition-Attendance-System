# Face Recognition Attendance System

This repository contains a Python-based Face Recognition Attendance System that utilizes a K-Nearest Neighbors (KNN) classifier for efficient and accurate face recognition. The system is designed to automate attendance marking by capturing, training, and recognizing faces in real-time, while also logging attendance data.

---

## Features

- **Face Registration**: Capture and store new user facial data for training.
- **Face Recognition**: Identify registered users in real-time and mark attendance.
- **Streamlit Dashboard**: View daily attendance records in an interactive interface.
- **CSV Logs**: Automatically generate and save timestamped attendance records in CSV format.

---

## System Overview

### 1. Face Data Registration (`add_faces.py`)
- Captures facial images using the webcam.
- Processes and stores the facial data locally for training.
- Dynamically updates the dataset with new user entries.

### 2. Real-Time Recognition and Attendance Logging (`test.py`)
- Leverages a pre-trained KNN model to recognize faces in real-time.
- Logs attendance into a timestamped CSV file.
- Displays the live webcam feed with user names overlayed.

### 3. Attendance Viewer (`app.py`)
- A lightweight dashboard created using Streamlit.
- Allows users to view the current day's attendance dynamically.

---

## Prerequisites

Ensure the following are installed before proceeding:
- **Python**: Version 3.7 or above
- **Libraries**:
  - OpenCV
  - NumPy
  - scikit-learn
  - pandas
  - Streamlit
- **Webcam**: Required for capturing and recognizing faces.
- `haarcascade_frontalface_default.xml`: Included in OpenCV's data for face detection.

---

## Setup Instructions

### 1. Clone the Repository:
```bash
git clone https://github.com/username/face-recognition-attendance.git
cd face-recognition-attendance
