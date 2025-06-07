Overview:

This ASL Detector is a real-time hand sign recognition application powered by computer vision and deep learning. It detects and classifies American Sign Language (ASL) characters using a webcam. The system captures hand landmarks using MediaPipe, processes them with OpenCV, and classifies gestures using a custom-trained keypoint classifier.

Usage:

When you run appl.py, the application starts in real-time inference mode by default. You can switch modes using the following keys:

• Press n: Inference mode (default)

• Press k: Manual data capture mode

• Press d: Automatic dataset processing mode

• Press c: Clear the current text

Table of Contents:

1. Features

2. Requirements

3. Installation

4. Model Training

5. Contributing

6. License

Features:

• Real-time ASL detection via webcam

• Hand tracking with MediaPipe

• Gesture classification using a custom-trained keypoint classifier

• Automatic word formation based on stable gesture detection

• Dataset generation and logging for model training

Requirements:

• Python 3.x

• OpenCV

• MediaPipe

• Pillow

• NumPy

• Pandas

• Seaborn

• Scikit-learn

• Matplotlib

• TensorFlow 2.16.1 (for TFLite conversion compatibility)

Installation:

1. Clone the Repository:

git clone https://github.com/ChandanNayak01/American-Sign-Language-Detection.git
cd American-Sign-Language-Detection

2. Install Dependencies:

pip install -r requirements.txt

3. Run the Application:

python appl.py

Model Training:

Data Collection

Manual Data Collection

• Press "k" to enter keypoint logging mode.

• Press any uppercase letter (A-Z) to record hand landmarks.

• Data is stored in model/keypoint_classifier/keypoint.csv.

Automated Data Collection

• Press "d" to process a dataset from folders.

• Images from model/dataset/dataset 1 are analyzed and keypoints saved.

Ensure the dataset path is correct in appl.py before running automated mode.

Training

Use the Jupyter notebook keypoint_classification.ipynb:

• Update NUM_CLASSES if changing the number of gestures.

• Update keypoint_classifier_label.csv accordingly.

• Execute all cells sequentially to train and export the model.

Model Structure:

Contributing

We welcome contributions to enhance this project! Feel free to:

1. Fork the repository

2. Create a new branch for your improvements

3. Commit and push your changes

4. Open a pull request
