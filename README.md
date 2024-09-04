# 🧠 Brain Tumor Detection Segment-It Model 🧠
This repository contains the Training, Evaluation, and Testing code for our research on brain tumor detection, utilizing a combined MobileNetV2-SSD model with modified Feature Pyramid Network (FPN) levels. Our model is trained on a well-known brain tumor dataset from Kaggle, provided by Jun Cheng.

### 🚀 Project Overview 🚀 

The goal of this project is to detect and localize brain tumors in MRI-scanned images. By leveraging the lightweight yet powerful MobileNetV2 architecture in conjunction with a Single Shot Detector (SSD) and enhanced FPN layers, we aim to improve the detection accuracy while maintaining computational efficiency.

Dataset
We use the brain tumor dataset from Kaggle, which includes MRI scans of brains, labeled for the presence of tumors. Preprocessing steps were crucial to prepare this dataset for object detection. These steps included:

Grayscaling: Converting images to grayscale to reduce computational complexity.
Filtering: Applying image filters to enhance tumor features.
Segmentation: Segmenting the brain regions for better focus.
The dataset was split into training, validation, and testing sets, with additional JSON files created for object (tumor) detection coordinates.

We utilized Google Colab as our primary environment for training and testing, taking advantage of its GPU capabilities to speed up the process. Additionally, we used TensorBoard for real-time tracking of our training metrics and Roboflow for preprocessing and augmenting our dataset.


### ✨ Model Architecture


![Arch Model](https://github.com/user-attachments/assets/feda2ce2-99ad-41ac-998a-1d6027d20522)


Key Features:

MobileNetV2: Lightweight and efficient backbone.
SSD: Real-time object detection.
Modified FPN: Enhanced multi-scale detection for better accuracy.

### 🎯 Metrics

To evaluate our model's performance, we focused on the following key metrics:

Precision: The accuracy of the tumor predictions.
Recall: The ability to correctly identify tumors.
Dice Similarity Coefficient (DSC): Measure of similarity between the predicted and ground truth segmentation.
Intersection over Union (IoU): Overlap ratio between the predicted bounding box and the actual tumor region.
Similarity Index: Evaluates the similarity between the predicted and actual tumor shapes.
