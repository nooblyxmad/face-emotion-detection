# Emotion Recognition using DeepFace
Involves the applying of DeepFace, OpenCV, and Python to develop a real-time facial expression detection system. Human emotions that can be detected are: angry, happy, sad, surprise, and neutral. GUI consists of a HUD design that shows the emotions with the confidence level. The app works properly as it applies a timed emotion detection approach.

---
# AI Face Emotion HUD

A real-time, cyber-styled **Emotion Recognition HUD** (Heads-Up Display) built with Python. This tool uses your webcam to detect facial expressions and visualizes them through a sleek, neon-themed interface using `DeepFace` and `OpenCV`.

---

## Features:

* **Real-Time Detection:** Live analysis of facial expressions.
* **Sleek HUD UI:** Custom-drawn interface with neon pink accents and a central targeting box.
* **Multi-Emotion Tracking:** Monitors 5 key emotional states simultaneously:
    * `Angry`, `Happy`, `Sad`, `Surprise`, and `Neutral`.
* **Performance Optimized:** Only runs heavy AI analysis every 0.6 seconds to ensure high FPS and smooth video playback.
* **Visual Analytics:** Side panel with dynamic progress bars indicating confidence levels for each emotion.

---

## Tech Stack:

* **Python 3.x**
* **OpenCV:** For video processing and UI rendering.
* **DeepFace:** AI framework for emotion recognition, using DeepFake .
* **TensorFlow:** Backend for the deep learning models.

---

## Installation Process:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/nooblyxmad/face-emotion-detection
   cd AI-Face-Emotion-HUD
2. **Install dependencies:**
   ```bash
   pip install opencv-python deepface tf-keras
3. **Run the application:**
   ```bash
   python main.py

---

## How It Works

* **Webcam Feed:** The script captures frames from your default camera (cv2.VideoCapture(0)).
* **Analysis Loop:** To prevent lag, the AI (DeepFace.analyze) runs on a slight delay defined by ANALYZE_EVERY.
* **UI Overlay:** * The Box: A "targeting" box stays fixed in the center for the user to align their face.
* **The Bars:** The left panel shows the intensity of all tracked emotions.
* **The Label:** The top-most detected emotion is highlighted in Neon Pink.

## Configuration
* You can easily tweak the performance directly in the script:
  ```bash
  # modify analysis frequency (low = more ai updates, higher = smoother video)
  ANALYZE_EVERY = 0.6 

  # change the UI colours
  NEON_PINK = (255, 0, 255)
  WHITE = (255, 255, 255)
