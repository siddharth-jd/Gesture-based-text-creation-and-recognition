# Gesture-based-text-creation-and-recognition
This project implements a Virtual Notepad using hand gesture recognition and computer vision. It allows users to draw on the screen, control brightness and system volume, and even predict handwritten digits using a trained deep learning model — all without touching a physical device.

# Features
Hand Tracking using MediaPipe

Draw/Erase on a virtual canvas using finger gestures

Brightness and Volume Control via hand gestures

Digit Prediction using a custom-trained CNN model on the canvas drawing

Customizable UI with header images for tool selection

# Requirements
Install dependencies using pip:

pip install opencv-python mediapipe numpy tensorflow pycaw comtypes wmi

# Additional Notes:

pycaw and wmi are used for volume and brightness control (Windows only).

TensorFlow is used for digit recognition.

A webcam is required for real-time gesture tracking.

# Model Training
The CNN for digit recognition is trained using the cnn_model.ipynb notebook. It uses standard digit datasets (like MNIST) and outputs a .h5 model used for prediction in the main script.

# Controls
Gesture	                                        Function
Two fingers up over top bar	                    Select tool (pen/eraser/control)
One finger (index)	                            Draw or erase
Thumb + Index pinch	                            Adjust brightness or volume
Tool "Predict" Button	                          Predict drawn digit
Press s	                                        Save canvas as image
Press q	                                        Quit

# How to Run
python VirtualNotepad.py
Ensure your webcam is active. Move your hand in front of the camera to interact with the virtual canvas.

# Libraries used: 
OpenCV, MediaPipe, TensorFlow, Pycaw, WMI
