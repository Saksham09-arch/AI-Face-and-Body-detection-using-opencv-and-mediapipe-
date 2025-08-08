# MediaPipe & FER Real-Time Gesture, Emotion, and Posture Detection

This project is an advanced Python application that leverages [MediaPipe](https://google.github.io/mediapipe/) and the [FER library](https://github.com/justinshenk/fer) to deliver **real-time hand, face, and full-body landmark detection, emotion recognition, gesture status, and posture analysis** from a webcam feed.

## Features

- **Hand Tracking & Gestures**
  - Accurately detects and labels palm and fingertip positions for each hand.
  - Recognizes when each hand (left and right) is fully open, displaying clear on-screen messages.
  - Visualizes fingertip movement trails for both hands.
  - Measures the 3D distance (meters, approximate) between the wrists of both hands when visible and extended.

- **Face Landmark & Emotion Recognition**
  - Identifies key facial features (forehead, eyes, nose, lips, chin, ears) and visualizes them.
  - Integrates FER (Facial Emotion Recognition) to assess real-time emotions, smoothing results for stability.
  - Includes a custom metric for detecting "Sleepy" or "Active" states based on eye openness.

- **Pose Detection & Feedback**
  - Marks and labels important body joints.
  - Calculates pose confidence to indicate landmark visibility and tracking accuracy.
  - Assesses and displays sitting posture quality (e.g., "Good Posture" or "Poor Posture").

- **User Experience**
  - Offers multiple color themes for better visibility.
  - Fullscreen video processing with keyboard controls:
    - `q` to quit
    - `space` to pause/resume
    - `s` to take a screenshot
    - `c` to change theme
  - Overlayed instructions, status messages, and measurement outputs (emotion, gesture, distance, posture).

## Requirements

- Python 3.7–3.11
- OpenCV
- MediaPipe
- Numpy
- FER
- MTCNN (dependency for FER face detection)
- (Install with: `pip install opencv-python mediapipe numpy fer mtcnn`)

## Use Cases

- Interactive gesture recognition and tracking demonstrations.
- Real-time classroom, gaming, or remote collaboration attention analytics.
- Development and rapid prototyping for HCI (Human-Computer Interaction) systems.
- Research in behavioral detection, affective computing, or personal ergonomics feedback.
