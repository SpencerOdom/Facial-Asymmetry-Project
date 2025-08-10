# Face Asymmetry Detector

This project implements a facial asymmetry detection system using **MediaPipe Face Mesh** and computer vision techniques in Python. The goal is to quantify and visualize asymmetry between the left and right sides of a face by analyzing facial landmarks.

---

## 📋 Project Overview

Facial asymmetry can serve as a significant biomarker in medical diagnostics, particularly for neurological conditions. This project extracts facial landmarks using MediaPipe’s Face Mesh model, calculates deviations between symmetric landmark pairs, and computes an asymmetry score to quantify how symmetrical a face is.

---

## 🚀 Features

- Detects and visualizes facial landmarks from input images  
- Defines a facial midline using nose landmarks for accurate symmetry comparison  
- Calculates per-point deviation between symmetric landmark pairs  
- Computes an overall asymmetry score (in pixels) indicating degree of facial asymmetry  
- Visualizes deviations with color-coded overlays for easy interpretation  

8/9/25
- Added additional notebook that includes:
     - Welcome screen
     - Live camera feed
     - Prompts when the user has not aligned their face with the camera
     - countdown timer and snapshot feature
     - Asymmetry score evaluation 

Needs much improvement, but a good base to work from. My camera quality/ lighting hinders performance, but it's realistic to what users have at home.

Future Updates:
To help offset potential lighting/environmental factors, I will add additional pairs of symmetrical points to use in calculating the final asymmetry score, taken from the user's face.

---

## 🛠️ Technologies Used

- Python 3  
- OpenCV  
- MediaPipe  
- Matplotlib  
- NumPy  

---

## 📂 Usage

1. Clone this repository & download libraries:

   ```bash
   git clone https://github.com/SpencerOdom/Facial-Asymmetry-Project.git
   cd Facial-Assymetry-Project
   pip install mediapipe opencv-python matplotlib numpy



Add your input face image (e.g., newface.jpg) to the project folder.

Run the Jupyter notebook or Python script to analyze facial asymmetry.

📈 Example Output
Facial Asymmetry Score: A numerical value (in pixels) quantifying the overall asymmetry.

Visualizations: Color-coded images highlighting landmark pairs contributing most to asymmetry.

🎯 Interpretation of Results
Asymmetry Score (px)	Interpretation
0–30	Very symmetrical
30–80	Mild asymmetry (normal variation)
80–150	Noticeable asymmetry
150+	Significant asymmetry or pose issues

## Instructions to Run the Live Camera Notebook

### Prerequisites
- Python installed  
- Webcam connected and accessible  
- Required libraries installed:  
  ```bash
  pip install opencv-python mediapipe numpy


Open the notebook (Virtual_Neurologist_LiveCam.ipynb) in Jupyter Notebook or JupyterLab.

Run the notebook cells sequentially until you reach the cell that opens the webcam feed.

When the webcam window opens:

Position your face centered horizontally in front of the camera.

Follow the on-screen instructions to adjust your face position.

Hold still once the countdown starts (5 seconds) to let the system capture your image.

After the countdown, the system will take a snapshot, calculate your facial asymmetry score, and show the result with an interpretation.

Press any key on the result window or ‘q’ in the live webcam window to exit.


🙋‍♂️ About Me
I developed this project as part of my interest in computer vision. Feel free to explore the notebook and reach out with questions or feedback!
