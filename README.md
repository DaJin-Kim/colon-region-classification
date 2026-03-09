# Colon Region Classification using Optical Flow

This project focuses on automatic classification of colon regions using colonoscopy videos.  
The goal is to support real-time navigation and localization during colonoscopy procedures.

The system utilizes optical flow features extracted from colonoscopy video frames to capture motion patterns inside the colon.

Both **real colonoscopy videos** and the **Mikoto colonoscopy simulator** were used for model training and evaluation.

---

# Overview

Colonoscopy is a key procedure for detecting colorectal diseases such as polyps and colorectal cancer.  
However, accurately identifying the current region of the colon during the procedure can be difficult.

This project aims to develop an AI system that can automatically classify colon regions based on video input.

The approach leverages motion information extracted from colonoscopy videos to improve region classification performance.

---

# Dataset

Two types of datasets were used:

### Real Colonoscopy Data
Videos collected from real colonoscopy procedures.

### Mikoto Colon Simulator
Synthetic colonoscopy videos generated from the Mikoto training simulator.

Example dataset frames:

![Dataset Example_1](images/dataset_example_1.png)
![Dataset Example_2](images/dataset_example_2.png)

---

# Method

The proposed approach uses **optical flow** to capture motion patterns between consecutive frames in colonoscopy videos.

The workflow is as follows:

1. Extract video frames from colonoscopy recordings
2. Compute optical flow between consecutive frames
3. Use motion features as input to the classification model
4. Predict the colon region

---

# Model Pipeline

![Model Pipeline](images/pipeline.png)

The pipeline consists of the following steps:

1. Colonoscopy video input
2. Optical flow extraction
3. Feature learning with a deep neural network
4. Colon region classification

---

# Real-Time Inference

The model was designed to support **real-time colon region classification** during colonoscopy procedures.

Example prediction results:

![Prediction Example](images/prediction_example.png)

---

# Results

The model achieved strong performance in classifying colon regions from colonoscopy videos.

Evaluation metrics include:

- Accuracy
- Confusion Matrix
- Per-region classification performance

Example evaluation results:

![Confusion Matrix](images/results_confusion_matrix.png)

---

# Repository Structure


colon-region-classification
│
├ README.md
├ images
│ ├ pipeline.png
│ ├ dataset_example.png
│ └ prediction_example.png
│
├ models
│
├ optical_flow
│
└ results


---

# Applications

- Colonoscopy navigation assistance
- Automated colon region recognition
- AI-assisted colonoscopy systems
