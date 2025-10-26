# 🗑️ Object Detection for Waste Management Project

## 📘 Overview
This repository contains the implementation of a **multi-class waste detection model** built using the **YOLOv8s architecture**. The project aims to automate the identification and classification of various types of waste to assist in **efficient waste management and recycling** systems. The model was trained on the **TACO (Trash Annotations in Context)** dataset, which includes 18 waste categories such as plastic bottles, cans, paper, and glass.

---

## 🎯 Project Objective
The goal of this project is to:
- Detect and classify different types of waste items in real-world images.
- Assist in smart waste management using **computer vision and deep learning**.
- Contribute toward environmental sustainability by enabling **automated waste sorting**.

---

## 🧠 Model Architecture
- **Base Model:** YOLOv8s (You Only Look Once, version 8 - Small)
- **Framework:** Ultralytics YOLOv8 (PyTorch backend)
- **Number of Classes:** 18 (based on the TACO dataset)
- **Image Size:** 640 × 640 pixels
- **Epochs:** 100
- **Optimizer:** Adam
- **Loss Function:** Object Detection Loss (composed of box loss, cls loss, and DFL loss)

---

## 📊 Dataset Description
**Dataset Name:** [TACO Trash Detection Dataset](https://tacodataset.org/)  
**Source:** Public dataset from Kaggle  
**Description:** A dataset of images annotated with 18 waste categories for object detection tasks.  
Each image contains one or more waste items labeled under:
> *Plastic, Metal, Paper, Glass, Cardboard, Textile, Organic, etc.*

---

## ⚙️ Training Environment
- **Platform:** Google Colab  
- **Hardware:** GPU (Tesla T4)  
- **Frameworks & Libraries:**  
  - Python 3.10  
  - PyTorch  
  - Ultralytics YOLOv8  
  - OpenCV  
  - NumPy  
  - Matplotlib  

---

## 📈 Results and Evaluation
| Metric | Value |
|--------|--------|
| **mAP@0.5** | **0.67** |
| **mAP@0.5:0.95** | **0.45** |
| **Precision** | **0.72** |
| **Recall** | **0.68** |
| **Validation Loss** | **1.041** |
| **Validation Accuracy** | **0.44** |

> The model shows strong generalization on diverse waste items and performs well in real-world scenarios.

---

## 🧾 Notebook File
The main notebook in this repository is:
`taco-trash-detection-yolov8s.ipynb`

It includes:
- Dataset preparation (TACO)
- Model training (YOLOv8s)
- Evaluation and visualization of predictions
- Detection results on validation images

---

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/object-detection-for-waste-management-project.git
   cd object-detection-for-waste-management-project
   ```
2. Install dependencies:
   ```bash
   pip install ultralytics opencv-python matplotlib numpy
   ```
3. Open and run the notebook:
   ```bash
   jupyter notebook taco-trash-detection-yolov8s.ipynb
   ```
4. The model will train and evaluate automatically using the configured parameters.

---

## 📂 Repository Structure
```
object-detection-for-waste-management-project/
│
├── taco-trash-detection-yolov8s.ipynb      # Main training and evaluation notebook
├── README.md                               # Project documentation
└── data/                                   # Dataset (optional local directory)
```

---

## 📚 Future Work
- Experiment with larger YOLOv8 variants (YOLOv8m or YOLOv8l)
- Deploy as a **real-time waste detection system** using a webcam
- Integrate with IoT devices for **smart bin automation**

---

## 🧑‍💻 Author
**Assad Ullah Khan**  
Research Assistant – Digital Image Processing Lab  
Islamia College University, Peshawar  
📧 Email: [assadullahkhan556@gmail.com](mailto:assadullahkhan556@gmail.com)

---

## 🏆 Acknowledgment
Special thanks to **Dr. Mohammad Sajjad (Associate Professor)** for his supervision and guidance throughout this research project.

---

## 📜 License
This project is licensed under the **MIT License** – feel free to use and modify for research or educational purposes.

---

> “Automating waste detection through AI and vision systems can help pave the way for a cleaner, smarter, and more sustainable planet.”
