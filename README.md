# MARINE_SHIP_DETECTION_USING_YOLO_AND_COMPUTER_VISION

# YOLOv8 Ship Detection 

This repository contains a deep learning-based solution for detecting ships in aerial imagery using **YOLOv8**, a state-of-the-art object detection model. The goal is to identify marine vessels accurately from drone or satellite images, which can assist in maritime surveillance, port management, and defense applications.


## 📁 Dataset

The dataset is obtained from kaggle and here is the link : https://www.kaggle.com/datasets/siddharthkumarsah/ships-in-aerial-images

- **Label Format**: YOLO format (bounding boxes with `class x_center y_center width height`).

---

## 🚀 Model Training

We used the **YOLOv8s** (small) model from Ultralytics for lightweight yet powerful detection.

### 🔧 Training Settings:
**Model**: `yolov8s.pt`
**Epochs**: 50
**Batch size**: 16
**Image size**: 640x640

### ✅ Evaluation Metrics:
`box_loss`: Localization loss for bounding boxes  
`cls_loss`: Classification loss for object classes  
`dfl_loss`: Distribution Focal Loss used in box regression  
`mAP50-95`: Mean Average Precision across IoU thresholds 0.5 to 0.95  
`mAP50`: mAP at IoU = 0.5  
`mAP75`: mAP at IoU = 0.75  



## 🧪 Results

- **Visual Inference**: Plotted detections on 20 random test images  
- **Quantitative Results**:
| Metric      | Value |
|-------------|-------|
| mAP50-95    | 0.309  |
| mAP50       | 0.509  |
| mAP75       | 0.330  |


