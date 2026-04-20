# 🧠 Brain Tumor Detection — YOLOv8

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![YOLOv5](https://img.shields.io/badge/YOLOv5-00FFFF?style=for-the-badge&logo=github&logoColor=black)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-FF6F00?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

> A deep learning model that detects and classifies brain tumors from MRI scans using YOLOv5 object detection — achieving **80–90% accuracy**.

---

## 📌 Overview

Brain tumor detection is a critical step in medical diagnosis. Manual analysis of MRI scans is time-consuming and prone to human error. This project leverages **YOLOv8**, a state-of-the-art object detection model, to automatically detect and localize brain tumors in MRI images — providing fast, reliable results that can assist medical professionals.

---

## 🎯 Key Results

| Metric | Score |
|--------|-------|
| **Accuracy** | 80–90% |
| **Model** | YOLOv8 |
| **Task** | Object Detection & Classification |
| **Input** | MRI Brain Scan Images |

---

## Sample Results


<img width="1920" height="869" alt="Screenshot (254)" src="https://github.com/user-attachments/assets/62cd67d4-31c7-4f35-a43d-2dd6e34c8e21" />


---

## Tech Stack

- **Model:** YOLOv5 (Ultralytics)
- **Language:** Python
- **Dataset:** Brain Tumor MRI Dataset (YOLOv5 PyTorch format)
- **Task:** Object Detection & Localization

---

##  Project Structure

```
brain-tumor-detection/
│
├── train/                  # Training images & labels
├── valid/                  # Validation images & labels
├── test/                   # Test images & labels
├── data.yaml               # Dataset configuration
├── README.md               # Project documentation
└── results/                # Output predictions & metrics
```

---

##  How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Aishascreations/brain-tumor-detection.git
cd brain-tumor-detection
```

### 2. Install Dependencies
```bash
pip install torch torchvision
pip install ultralytics
```

### 3. Train the Model
```bash
python train.py --img 640 --batch 16 --epochs 50 --data data.yaml --weights yolov5s.pt
```

### 4. Run Detection on an Image
```bash
python detect.py --weights runs/train/exp/weights/best.pt --img 640 --source your_image.jpg
```

---

## Dataset

The dataset is structured in **YOLOv5 PyTorch format** and contains:
- **Training set** — MRI images with labeled tumor regions
- **Validation set** — for model evaluation during training
- **Test set** — for final performance assessment

> Dataset sourced from [Roboflow Brain Tumor Detection Dataset](https://roboflow.com)

---

## Future Improvements

- [ ] Deploy as a web app using Flask or Streamlit
- [ ] Expand dataset for better generalization
- [ ] Add tumor type classification (glioma, meningioma, pituitary)
- [ ] Integrate with a medical imaging dashboard

---

## Author

**Aishat Onakoya**
- 📧 [onakoyaaishat5@gmail.com](mailto:onakoyaaishat5@gmail.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/aishat-onakoya-233627272/)
- 🐙 [GitHub](https://github.com/Aishascreations)

---

⭐ *If you found this project useful, consider giving it a star!*
