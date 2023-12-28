
# DrowseSense-Vision-Based-Driver-Drowsiness-Monitoring

## Overview
This project aims to enhance road safety by detecting driver drowsiness using vision-based techniques. It offers a real-time fatigue warning system by monitoring facial features, enabling proactive measures to prevent accidents due to driver fatigue.
## Key Features
 **Drowsiness Detection:** Utilizes facial landmarks to calculate Eye Aspect Ratio (EAR) for detecting drowsiness.
- **Real-time Alert System:** Issues alerts upon detecting signs of driver fatigue.
- **Technologies Used:** Python (OpenCV, dlib), C++ (esp32cam), WiFi connectivity.

## Components
### Python Code (Driver Drowsiness Detection)
- Utilizes OpenCV and dlib libraries to:
  - Capture video frames from the webcam.
  - Detect facial landmarks for eye aspect ratio calculation.
  - Trigger alerts upon detecting drowsiness.

### Hardware Code (ESP32CAM)
- Enables ESP32CAM functionality for capturing images.
- Provides three resolution options: low, medium, and high.
- Hosts a web server to access the captured images.

## Setup Instructions
1. **Python Setup:**
   - Install required Python libraries: `scipy`, `imutils`, `pygame`, `dlib`, `cv2`.
   - Ensure the pre-trained shape predictor file (`shape_predictor_68_face_landmarks.dat`) is available.
   - Connect a webcam to your system.

2. **ESP32CAM Setup:**
   - Configure WiFi credentials in the ESP32CAM code.
   - Adjust GPIO pin configuration as per your hardware setup.

3. **Execution:**
   - Run the Python script for real-time driver drowsiness monitoring.
   - Deploy the ESP32CAM code to enable image capture and hosting via a web server.

## Usage
1. Run the Python script to activate the driver drowsiness monitoring system.
2. Access captured images from ESP32CAM by navigating to:
   - `/cam-lo.jpg` for low-resolution images.
   - `/cam-mid.jpg` for medium-resolution images.
   - `/cam-hi.jpg` for high-resolution images.

## Notes
- Ensure proper hardware setup and connectivity for both the Python script and ESP32CAM.
- Adjust the threshold and frame check parameters in the Python script for optimal drowsiness detection based on your requirements.

---
