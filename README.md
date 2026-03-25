# 🚗 Driver Drowsiness Detection using Deep Learning

## 📌 Project Overview
Driver drowsiness is a major cause of road accidents. This project aims to detect driver fatigue using computer vision techniques by analyzing eye closure and yawning behavior from facial images.

---

## 🎯 Objectives
- Detect eye state (Open / Closed)
- Detect mouth state (Yawn / No Yawn)
- Classify driver fatigue into:
  - Alert (0)
  - Mild Fatigue (1)
  - Severe Fatigue (2)

---

## 🧠 Technologies Used
- Python
- TensorFlow / Keras
- Convolutional Neural Networks (CNN)
- Transfer Learning (MobileNetV2)
- OpenCV
- Matplotlib & Seaborn

---

## 📂 Dataset
- Contains facial images with 4 classes:
  - Eyes Open
  - Eyes Closed
  - Yawn
  - No Yawn
- Data split into:
  - Training set
  - Validation set
  - Test set

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Image resizing (224 × 224)
- Normalization (0–1 scale)
- Data augmentation:
  - Rotation
  - Zoom
  - Horizontal flip
  - Brightness adjustment

### 2. Model Development
- Custom CNN model built from scratch
- MobileNetV2 used for transfer learning

### 3. Model Training
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Performance monitored using validation data

---

## 📊 Results

| Model | Accuracy |
|------|---------|
| Custom CNN | ~75% |
| MobileNetV2 | ~89% |

👉 MobileNetV2 performed better due to pretrained feature extraction.

---

## 📈 Evaluation Metrics
- Accuracy
- Confusion Matrix
- Precision & Recall

---

## 🔄 Decision Logic

The 4-class output is converted into 3 fatigue levels:

| Class | Fatigue Level |
|------|--------------|
| Open / No Yawn | Alert (0) |
| Yawn | Mild Fatigue (1) |
| Closed | Severe Fatigue (2) |

---

## 📉 Fatigue Progression

A fatigue progression curve is generated to track how the driver's alertness changes over time.

---

## ⚠️ Limitations
- Performance depends on lighting conditions
- Requires clear facial visibility
- May not work well for extreme angles

---

## 💡 Future Improvements
- Real-time webcam integration
- Better dataset for improved accuracy
- Integration with vehicle safety systems

---

## 📌 Conclusion
This project successfully demonstrates a non-intrusive method for detecting driver drowsiness using deep learning and computer vision techniques, achieving high accuracy with MobileNetV2.

---

## 👩‍💻 Author
Diviya
