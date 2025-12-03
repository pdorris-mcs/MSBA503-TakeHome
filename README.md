# Object Detection Comparison: YOLOv8 vs Faster R-CNN
MSBA 503 — Take-Home Assignment  
Author: *Your Name*

## 📌 Overview
This project compares the performance of two deep learning object detection models:
- **YOLOv8m** (Ultralytics)
- **Faster R-CNN (ResNet50-FPN)** (TorchVision)

Each model was run on a collection of ~10 images.  
For both models, I recorded:
- Number of objects detected  
- Average confidence score  
- Maximum confidence score  
- Unique object classes identified  
- Inference time (seconds)  
- Additional image metadata (width, height, aspect ratio, brightness)

The results were compiled into a final comparison table included in the written submission.

---

## 🚀 Notebooks
All code is contained in the following notebooks:

### **1. YOLO Object Detection**
`notebooks/Object Detection (YOLO).ipynb`
- Loads YOLOv8m model  
- Runs detection over all images  
- Extracts confidence, labels, runtime  
- Saves results table  

### **2. Faster R-CNN Object Detection**
`notebooks/Object Detection (Faster RCNN).ipynb`
- Loads TorchVision Faster R-CNN model  
- Runs detection over the same image set  
- Extracts confidence, labels, runtime  
- Saves results table  

---

## 📊 Output Data
<img width="7665" height="4134" alt="df_results" src="https://github.com/user-attachments/assets/a2600b47-cbc4-4954-b93f-b776f0bf1d2d" />
