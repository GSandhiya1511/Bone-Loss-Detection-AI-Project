# Bone Loss Detection in Dental X-rays using YOLOv8
Overview
This project demonstrates the use of YOLOv8 for detecting bone loss regions in dental X-ray images. The dataset of ~2,800 annotated images was obtained from Roboflow. The model was trained on Google Colab (GPU) for 20 epochs using transfer learning, achieving strong detection results.

Key Results
  1. Precision: 53.88%
  2. Recall: 49.23%
  3. mAP@50: 47.24%

Features
  1. Detects bone loss in dental X-rays.
  2. Includes trained weights (best.pt) and sample predictions.
  3. Built with Python, PyTorch, OpenCV, and Roboflow API.

Dataset

        Source: Roboflow (Dadad-RVG v5 dataset).

        Images: ~2,800 annotated dental X-rays.

        Split: 2,405 for training and 387 for validation.

     

1) Rationale for Choosing YOLOv8
   
YOLOv8 (You Only Look Once, version 8) was chosen because:

i. Best for Object Detection: It’s a state-of-the-art real-time object detection model,
ideal for identifying specific regions like bone loss in dental X-rays.

ii. Pre-trained Weights: YOLOv8n (nano) allows transfer learning, meaning it
adapts quickly with smaller datasets.

iii. Speed & Accuracy: YOLOv8n is optimized for faster training on free Google
Colab GPUs while maintaining high accuracy.

iv. Easy Integration: Roboflow provides YOLOv8-ready datasets, which makes
training seamless.


3) Model Performance Evaluation Metrics
   
The key metrics we consider are:
i. mAP50 (Mean Average Precision at IoU 0.5): Measures detection accuracy
(higher is better).

ii. Precision: Measures how many detected regions are correct (less false positives).

iii. Recall: Measures how many actual regions were detected (less false negatives).

iv. Loss Values: Box loss, class loss, and DFL loss indicate how well the model is
learning during training.

  Precision (P): ~53.88%
  
  Recall (R): ~49.23%
  
  mAP@50: ~47.24%
  
  mAP@50-95: ~27.88%
  

3) Why Metrics Are Not Perfect
   
i. Small Dataset: With limited X-ray images, the model can’t generalize perfectly.

ii. Class Imbalance: If bone loss cases are fewer than normal cases, detection is
harder.

iii. Image Quality: Low-resolution or varying brightness of X-rays affects feature
learning.


5) Steps to Improve Metrics
   
i. Increase Dataset Size: Add more annotated X-ray images for bone loss.

ii. Data Augmentation: Apply flips, rotations, brightness/contrast changes to
increase variety.

iii. Train for More Epochs (e.g., 50+): Allows the model to learn deeper features.

iv. Use a Larger YOLOv8 model (YOLOv8m or YOLOv8l): Improves accuracy
(requires more GPU power).

v. Hyperparameter Tuning: Adjust learning rate, batch size, and image size for
better performance.


Author
Sandhiya G
Computer Science Graduate | Data Analysis & AI/ML Enthusiast
