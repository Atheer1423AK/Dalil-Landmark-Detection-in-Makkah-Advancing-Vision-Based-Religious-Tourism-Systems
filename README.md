# 🕋 Dalil: Landmark Detection in Makkah

Dalil is a computer vision system designed to detect and classify key religious landmarks in Makkah.  
Using fine-tuned YOLOv11 models, it supports the development of vision-based tourism assistance and enhances the visitor experience through AI-powered landmark recognition.

---

## 📖 Overview
This project fine-tunes **YOLOv11n** and **YOLOv11s** models for detecting major Makkah landmarks, including:
- AlSafa-and-Marwah Mountain
- Blackstone
- Clocktower
- Jamarat
- Kaaba
- Maqam Ibrahim
- Yemeni Corner

By combining **extensive data augmentation**, **optimized training**, and **model comparison**, we achieve high-accuracy detection suitable for tourism, guidance systems, and cultural heritage applications.

---

## ✨ Features
- **High-accuracy detection** of Makkah landmarks.
- **YOLOv11 small and nano models** for performance optimization.
- **Extensive preprocessing & augmentation**:
  - Resizing (640×640), auto-orientation, horizontal flip
  - Saturation & brightness adjustment
  - Gaussian blur, CLAHE, random crop
  - Night, fog, glare, and dust particle effects
- **Inference pipeline** integrated for real-time detection.
- **Evaluation with Precision, Recall, F1-Score, mAP@0.5, and MAE**.

---

## 📊 Results

| Model    | Precision | Recall  | F1 Score | mAP@0.5 | MAE     |
|----------|-----------|---------|----------|---------|---------|
| YOLOv11n | 100%      | 96.20%  | 98.00%   | 97.70%  | 0.0383  |
| YOLOv11s | 99.40%    | 95.70%  | 95.70%   | 97.60%  | 0.0368  |

YOLOv11n delivers a **perfect precision score (100%)** and higher F1-score, while YOLOv11s achieves slightly lower precision but marginally better MAE.

---

## 📂 Pipeline
![PHOTO-2025-05-03-17-49-02](https://github.com/user-attachments/assets/12b22938-c361-4c5e-a0f9-3aef0da8b005)


**Steps:**
1. **Dataset Collection** → Makkah Landmark Dataset.
2. **Data Augmentation** → Night/fog effects, random crops, saturation changes, etc.
3. **Model Training** → Fine-tuning YOLOv11n & YOLOv11s.
4. **Inference** → Detect landmarks in images/videos.
5. **Interpretation** → Use ALLam model for interpretation.

---

## 📦 Dataset
The dataset is available here:  
[📥 Makkah Landmark Dataset on Roboflow](https://universe.roboflow.com/makkah-landmarks/makkah-landmarkd)



