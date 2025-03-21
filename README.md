# Hand Gesture Volume Controller

## Overview
The Hand Gesture Volume Controller is a computer vision-based project that allows users to control system volume using hand gestures. It utilizes OpenCV for video capture and image processing, MediaPipe for hand tracking, and Pycaw for interacting with the system's audio settings.

## Features
- Detects hand movements using a webcam.
- Tracks the distance between the thumb and index finger.
- Adjusts the system volume based on finger distance.
- Displays a real-time volume bar and percentage.
- Shows FPS (Frames Per Second) on the screen.

## Requirements
- Python 3.x
- OpenCV (`cv2`)
- NumPy
- MediaPipe (for hand tracking)
- Pycaw (for audio control)
- Comtypes (for Windows audio interface)

## Installation
1. Clone the repository or download the script.
2. Install the required dependencies:
   ```bash
   pip install opencv-python numpy mediapipe pycaw comtypes
   ```
3. Run the script:
   ```bash
   python hand_gesture_volume.py
   ```

## Usage
1. Ensure your webcam is functional.
2. Run the script and place your hand in front of the camera.
3. Adjust the volume by bringing your thumb and index finger closer or farther apart.
4. Close the script window to exit.

## How It Work
- The script captures video frames from the webcam.
- The `handtrackingmodule` detects hand landmarks.
- The distance between the thumb and index finger is mapped to the system volume range.
- Volume changes dynamically as the finger distance varies.
- A volume bar and percentage indicator provide visual feedback.

## Acknowledgment
- OpenCV for image processing.
- MediaPipe for hand tracking.
- Pycaw for audio control.

## License
This project is open-source and free to use. Modify and distribute as needed.
