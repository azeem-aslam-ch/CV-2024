# 🏭 Industrial Object Detection using YOLOv8 & YOLOv9

A deep learning–based object detection system for industrial environments using YOLOv8 and YOLOv9. The project focuses on identifying and localizing industrial components such as tools, parts, safety gear, or equipment from real-world images or videos.

---

## 📌 Features

- 🎯 Real-time detection of industrial tools and objects
- 📦 Multi-class classification using YOLOv8 & YOLOv9
- 📈 Model training on custom-labeled industrial dataset
- 📊 Comparison of detection performance (mAP, FPS, size)
- 🚀 Works in both Google Colab and local setups
- 🖼️ Visual result samples with bounding boxes

---

## 🧠 Models Used

| Model   | Version | Framework   | Key Benefit           |
|---------|---------|-------------|------------------------|
| YOLOv8s | v8.1    | Ultralytics | Fast + lightweight     |
| YOLOv9s | v9.0    | Ultralytics | Higher accuracy & robustness |

---

## 🗂️ Dataset

- **Source**: Custom images from industrial plant floors & warehouse
- **Annotations**: Roboflow (YOLO format)
- **Classes**: Wrench, Screwdriver, Drill, Conveyor, Machine, Box, Worker Helmet
- **Augmentation**: Mosaic, flip, brightness, noise

---

## ⚙️ Google Colab Setup

👉 [Open in Google Colab](https://colab.research.google.com/github/azeem-aslam-ch/Industrial_object_detection/blob/main/Industrial_Detection_YOLOv8_YOLOv9.ipynb)

---

## 🚀 Training

### 🧠 YOLOv8

```python
!yolo task=detect mode=train model=yolov8s.pt data=data.yaml epochs=100 imgsz=640
