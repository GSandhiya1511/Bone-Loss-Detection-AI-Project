# 🦷 Dental Bone Loss Detection using YOLOv8

This project focuses on detecting **bone loss in dental X-ray images** using a YOLOv8 object detection model. It was developed as part of an AI/ML assignment provided by **Rugas Technologies**, using a labeled dataset sourced from **Roboflow** and trained on **Google Colab** with GPU acceleration.

## Project Objective
To build an AI model capable of identifying bone loss in dental radiographs with high accuracy and efficiency using modern deep learning tools.

---

## Dataset
- **Source:** Roboflow – Dadad-RVG v5 dataset  
- **Format:** YOLO annotation (bounding boxes)  
- **Classes:** 9 (focused on bone loss)  
- **Split:**
  - Training: 2,405 images  
  - Validation: 387 images  

---

##  Model Architecture
- **Model:** YOLOv8n (Nano version – lightweight and fast)
- **Training Tool:** [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- **Epochs:** 20  
- **Batch Size:** 16  
- **Image Size:** 640x640  
- **Transfer Learning:** Enabled with pretrained weights (`yolov8n.pt`)  

---

##  Tools & Libraries Used
- Python, NumPy, Pandas
- OpenCV, PyTorch, Roboflow
- Google Colab (GPU – Tesla T4)
- Ultralytics YOLOv8
- Matplotlib (for visualization)

---

##  Model Performance
- **Precision:** 81.5%
- **Recall:** 74.2%
- **mAP@50:** 78.1%
- **mAP@50–95:** 53.9%

Training and validation metrics are visualized using `results.png`.

---

##  Sample Predictions
Model outputs were saved and visualized to highlight bone loss areas in X-rays. A sample set is included in `predictions.zip`.

---

##  Files Included
- `best.pt`: Trained YOLOv8 model weights  
- `predictions.zip`: Output images with predictions  
- `results.csv`: Training metrics per epoch  
- `README.md`: Project description  

---
## [Prediction File](https://drive.google.com/file/d/16yOvC8fiPGH0QbWhW6DGo1y_37_Lc9Fm/view?usp=sharing)


## 🔗 Links
- 📬 [Project Showcase on LinkedIn](https://www.linkedin.com/in/gsandhiya1511/overlay/projects/1163901460/multiple-media-viewer/?profileId=ACoAADsaTh0B0l7HqKHGolptY1PVakT7nYf16-w&treasuryMediaId=1753511969213) 
- 📁 [Colab Notebook](https://colab.research.google.com/drive/1Vb4YZHHz5gJUvjMYBHwiCvN7LhxIIJlW#scrollTo=79cfqUPUzfYi)  
