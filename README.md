# Object Detection Comparison: YOLOv8 vs Faster R-CNN  
**MSBA 503 – Take-Home Assignment**  
Author: **Patrick Dorris**

---

## 📌 Overview  
This project compares the performance of two modern deep-learning object detection models:

- **YOLOv8m** (Ultralytics)
- **Faster R-CNN (ResNet50-FPN)** (TorchVision)

Both models were evaluated on a dataset of ~10 images.  
For each image, I extracted the following metrics:

- **Number of objects detected**  
- **Average confidence score**  
- **Maximum confidence score**  
- **Unique object classes identified**  
- **Model inference time (seconds)**  
- **Predicted object class labels**  
- **Additional image metadata**: width, height, aspect ratio, brightness  

These results were compiled into a comparison table used in the written submission and shown below in the **Final Output Data** section.

---

## 📁 Notebook

All code for this project is contained in a single Jupyter notebook:

### **📘 `take_home_assignment.ipynb`**
This notebook contains the full workflow for this project, including:

- Loading and preparing the image dataset  
- Running **YOLOv8m** (Ultralytics) on ~10 images  
- Running **Faster R-CNN (ResNet50-FPN)** (TorchVision) on the same images  
- Extracting detection outputs (labels, bounding boxes, confidence scores)  
- Calculating per-image metrics:
  - Number of detections  
  - Average and maximum confidence  
  - Unique classes detected  
  - Inference time  
  - Additional image metadata (width, height, aspect ratio, brightness)

- Combining YOLO and Faster R-CNN results into a unified Pandas DataFrame  
- Exporting the final comparison table as a CSV and PNG image  
- Producing visuals and summary data used in the written report  

This notebook is self-contained and can be run start-to-finish to reproduce all analysis and output tables included in this repository.

---

## 🧪 Methods  

### **Image-Level Features**  
In addition to model predictions, I calculated simple image metadata using Python tools (PIL, NumPy):

- Width & height  
- Aspect ratio  
- Average brightness (pixel mean)  

### **Detection-Level Features**  
Each model outputs for every image:

- List of detected classes  
- Number of unique classes  
- Mean and max confidence score  
- Total objects detected  

These allow direct, image-by-image comparison.

---

## 📦 Dependencies  
All required dependencies are listed in `requirements.txt`.

---

## 📊 Final Output Data
<img width="7665" height="4134" alt="df_results" src="https://github.com/user-attachments/assets/a2600b47-cbc4-4954-b93f-b776f0bf1d2d" />
