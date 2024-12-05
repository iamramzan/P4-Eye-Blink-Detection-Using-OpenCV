# P2-Eye-Blink-Detection-Project

In this project, I developed an Eye Blink Detection Model using OpenCV, NumPy, and Python. This project focuses on detecting blinks in real time, leveraging computer vision techniques. While it’s a fairly straightforward task, it’s essential to have a basic understanding of OpenCV and face landmark detection as they form the foundation of this implementation.

🔧 Tools and Libraries Used
- Python 3: The primary programming language for developing the script.
- NumPy: Used for efficient data manipulation and array operations.
- OpenCV: The go-to open-source library for computer vision tasks. It enables real-time video frame capture, image processing, and facial landmark detection.

🧩 Step-by-Step Process
1. Install Required Packages:
Ensure all necessary libraries, such as OpenCV and NumPy, are installed. Use pip install opencv-python and pip install numpy to set up your environment.
2. Initialize and Read from the Webcam:
Set up the webcam to capture live video frames using OpenCV’s VideoCapture function.
3. Convert Frames to Grayscale:
Convert the captured video frames to grayscale for faster processing and to enhance the accuracy of detection algorithms.
4. Apply Filters to Remove Noise:
Use image filtering techniques (e.g., Gaussian Blur) to clean up the frames and reduce noise. This step helps improve the robustness of the detection process.
5. Detect the Face Region:
Use a pre-trained Haar Cascade or DNN-based face detector in OpenCV to identify the face region within each frame. This face region will then be used to locate the eyes.
6. Extract the Region of Interest (ROI):
Extract the face region (roi_face) from the frame, which will be passed to the eye classifier for further analysis.
7. Detect Eye Objects:
Use a pre-trained eye classifier to detect eyes within the face region. Measure the size and position of the detected eyes to determine the state (open or closed).
8. Verify Detection:
Ensure the detection is running accurately and verify that eyes are being identified correctly.
9. Check for Eyes Before Starting Blink Detection:
Confirm the presence of eyes in the initial setup to avoid false detections and improve accuracy.
10. Start Blink Detection:
Implement a logic to monitor eye state changes (open → closed → open) to detect blinks. Track and log the number of blinks in real time.

👨‍💻 Key Features
- Real-time eye tracking and blink detection using a webcam.
- Noise reduction for improved detection accuracy.
- Facial region isolation for faster processing.
- Scalable and customizable for various use cases like drowsiness detection and gaze monitoring.

<img src="https://github.com/iamramzan/P2-Eye-Blink-Detection-Project/blob/main/Eye_Blink_Detection.png">
