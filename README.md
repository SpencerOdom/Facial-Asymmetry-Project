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

---

## 🛠️ Technologies Used

- Python 3  
- OpenCV  
- MediaPipe  
- Matplotlib  
- NumPy  

---

## 📂 Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/face-asymmetry-detector.git
   cd face-asymmetry-detector
Install dependencies:

bash
Copy
Edit
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

🙋‍♂️ About Me
I developed this project as part of my interest in computer vision and medical imaging. Feel free to explore the notebook and reach out with questions or feedback!
