# Drowsiness Detection System
This project implements a real-time drowsiness detection system using OpenCV, dlib, and Python. The system monitors a person's eyes to detect drowsiness and sounds an alarm if drowsiness is detected. It uses facial landmarks to analyze the blink ratio of the eyes and determine whether the person is sleepy, drowsy, or active.

# Features
Real-time detection of drowsiness based on eye blink patterns.
Alerts the user with an alarm sound when drowsiness is detected.
Displays the status (Active, Drowsy, Sleeping) on the video feed.
Uses OpenCV for video capture and image processing.
Utilizes dlib for facial landmark detection.

# Requirements
To run this project, you'll need the following dependencies:
Python 3.x
OpenCV
dlib
imutils
numpy
winsound (available on Windows by default)

# Installations
Install the required Python packages:
1)pip install opencv-python dlib imutils numpy
2)Download the shape_predictor_68_face_landmarks.dat file from dlib's official website and place it in the project directory.

# How It Works
1)Face Detection: The system uses dlib's pre-trained facial landmark detector to identify the 68 facial landmarks.
2)Eye Aspect Ratio Calculation: The eye aspect ratio (EAR) is calculated to determine whether the eyes are open or closed.
3)Blink Detection: The script checks the EAR to detect blinks and assess if the eyes are closed for too long, indicating drowsiness.
4)Alarm Trigger: If the system detects that the eyes have been closed beyond a certain threshold, it triggers an alarm sound to alert the user.

# Customization
Thresholds: You can adjust the thresholds for detecting drowsiness and sleep in the blinked function and the while loop conditions.
Alarm Sound: The alarm can be customized by modifying the play_alarm function.
