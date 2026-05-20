# Casting Defect Detection

## 📖 Overview
This project applies deep learning (MobileNetV2) to classify industrial casting product images into **defective** and **non-defective** categories.  
Defect detection is critical in manufacturing to reduce waste and ensure product quality.  
The notebook demonstrates transfer learning, data preprocessing, and evaluation on a real-world dataset.

---

## 📂 Dataset
- **Source:** [Kaggle Casting Product Dataset](https://www.kaggle.com/code/nxvt3w/castingdefdetector)  
- **Classes:**  
  - `def_front` → defective castings  
  - `ok_front` → non-defective castings  
- Preprocessing included resizing, normalization, and augmentation.


##My Kaggle Notebook
[Kaggle Notebook](https://www.kaggle.com/code/nxvt3w/castingdefdetector)

---

## ⚙️ Model & Approach
- **Architecture:** MobileNetV2 (pretrained on ImageNet)  
- **Training setup:**  
  - Optimizer: Adam (LR = 0.001)  
  - Loss: CrossEntropy  
  - Batch size: 32  
- **Steps:**  
  - Transfer learning with fine-tuning  
  - Data augmentation for robustness  
  - Evaluation with confusion matrix and accuracy metrics

---

## 📊 Results
- **Validation Accuracy:** ~98  
- **Confusion Matrix Highlights:**  
  - Defective correctly predicted: 442  
  - Okay correctly predicted: 259  
- The model shows strong classification performance with minimal misclassifications.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/tiwarinishtha123/casting-defect-detection.git
   cd casting-defect-detection
