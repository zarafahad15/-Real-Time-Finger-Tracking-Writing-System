# -Real-Time-Finger-Tracking-Writing-System
Air-Writing System

Real-Time Finger Tracking and Touchless Handwriting (MediaPipe + OpenCV)

The Air-Writing System allows users to write in mid-air using only their index finger. A webcam tracks fingertip movements in real time and renders the handwriting on a digital canvas. No stylus or touchscreen is required.

This project demonstrates a modern approach to touchless human–computer interaction using computer vision and hand landmark detection.

⸻

Features
	•	Real-time index-finger tracking using MediaPipe Hands
	•	Touchless handwriting through natural finger gestures
	•	Digital canvas overlay for drawing strokes
	•	Smooth line rendering using OpenCV
	•	Works with any standard webcam

⸻

Technologies Used
	•	Python 3.7+
	•	OpenCV
	•	MediaPipe Hands
	•	NumPy

⸻

Installation

1. Install dependencies

pip install opencv-python mediapipe numpy

2. Run the program

python air_writing.py


⸻

Project Structure

air-writing-system/
 ┣ src/
 ┃ ┗ air_writing.py
 ┗ README.md


⸻

How It Works

Hand Detection

The system uses MediaPipe Hands to detect 21 hand landmarks. The index fingertip (landmark 8) is used for drawing.

Finger Position Tracking

The fingertip’s normalized coordinates are converted into pixel coordinates on the screen.

Gesture Recognition

Writing mode is activated when the index fingertip is positioned above its lower knuckle (landmark 6). This indicates that the user intends to draw.

Canvas Rendering

A persistent digital canvas is layered over the camera feed. When in writing mode, lines are drawn between consecutive fingertip positions.

⸻

Usage Instructions
	•	Point upward with your index finger to start drawing
	•	Lower your finger to stop drawing
	•	Move your hand in the air to create strokes
	•	Press ESC to close the application

⸻

Applications
	•	Touchless whiteboard systems
	•	Human–computer interaction (HCI) research
	•	AR/VR gesture input
	•	Digital art
	•	Interactive STEM and education tools
	•	Accessibility-focused interfaces

⸻

Future Enhancements
	•	Stroke smoothing with Bezier curves
	•	Undo/redo gesture controls
	•	Color and thickness adjustment
	•	Save output to file
	•	Support for multi-hand drawing
	•	Optional OCR to convert handwriting into text

⸻

License

This project is released under the MIT License.

⸻
