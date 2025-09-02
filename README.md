# 🖐️ Sign Language Detection

This project implements a **real-time sign language detection system** using **TensorFlow** and **OpenCV**.  
The goal is to bridge the communication gap between the hearing-impaired and others by translating sign language gestures into text or speech.

---

##  Features
-  Real-time sign detection using webcam.
-  Deep learning models (TensorFlow Object Detection API).
- 🗂 Custom dataset support for training your own gestures.
- 🖼 Image preprocessing & augmentation pipeline.
-  Evaluation metrics and visualization.
-  Easy-to-run scripts for training and inference.

---

## 📂 Project Structure
SignLanguageDetection/
│── Tensorflow/
│ ├── workspace/
│ │ ├── annotations/ # Label files (.xml/.csv)
│ │ ├── images/ # Train/Test images
│ │ ├── models/ # Trained models and checkpoints
│ │ └── pre-trained-models/ # Downloaded pre-trained TF models
│ └── scripts/ # Utility scripts (training, evaluation, etc.)
│── README.md # Project documentation



---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/anjaliy11/SignLanguageDetection.git
   cd SignLanguageDetection

   ---
## Create a virtual environment
conda create -n signlang python=3.10 -y
conda activate signlang

---
  ## Install dependencies
Install TensorFlow Object Detection API
git clone https://github.com/tensorflow/models Tensorflow/models
cd Tensorflow/models/research
protoc object_detection/protos/*.proto --python_out=.
pip install .
cd ../../..

---
## ▶️ Usage
## 1. Collect Images
Use your webcam to capture images for different gestures:
python Tensorflow/scripts/collect_images.py

---

## 2. Label Images
Label the collected images using LabelImg.

---

## 3. Train Model

python Tensorflow/scripts/train.py

---
## 4. Real-time Detection
Run the detection script:
python Tensorflow/scripts/detect.py



---
## Tech Stack
Python

TensorFlow 

 Keras
 
OpenCV

NumPy

 Pandas 
 
 Matplotlib
 
LabelImg (for annotation)







