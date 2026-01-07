# Facial Expression Recognition: Preprocessing Techniques Comparison

## 📌 Project Overview
This project presents a comparative study of multiple **image preprocessing techniques** applied to the **same facial expression recognition model**. The objective is to analyze how different preprocessing methods affect model performance and to identify the technique that produces the best results.

Instead of modifying the model architecture, all experiments were conducted using the **same model configuration**, ensuring a fair comparison where preprocessing is the only changing factor.

A total of **four approaches** were evaluated, including a baseline case where **raw images were directly fed into the model without any preprocessing**.

---

## 📂 Dataset
- **Dataset Name:** CK+48 Facial Expression Dataset  
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/shawon10/ckplus  

The dataset consists of grayscale facial expression images resized to **48×48 pixels**, categorized into multiple emotion classes.

---

## 🧪 Preprocessing Techniques Used
The following preprocessing techniques were implemented and evaluated independently:

1. **No Preprocessing (Baseline)**
   - Raw images directly passed to the model.
   - Used as a reference for performance comparison.

2. **Gaussian Blur**
   - Noise reduction using Gaussian filtering.
   - Helps smooth facial features and suppress high-frequency noise.

3. **Histogram Equalization**
   - Enhances contrast by redistributing intensity values.
   - Improves feature visibility under varying lighting conditions.

4. **Thresholding and Contour Detection**
   - Applies thresholding followed by contour extraction.
   - Highlights facial structure and edges.

---

## 🧠 Model Details
- **Model Type:** Convolutional Neural Network (CNN)
- **Input Shape:** 48 × 48 × 1 (grayscale)
- **Training Setup:**
  - Same architecture for all experiments
  - Identical train-validation split
  - Same hyperparameters across all preprocessing techniques

This setup ensures that performance differences are solely due to preprocessing methods.

---

## 📊 Evaluation
- Model performance was evaluated using accuracy and loss metrics.
- All preprocessing techniques were compared under identical conditions.
- The preprocessing method yielding the best validation performance was selected as the optimal approach.

Detailed results and training procedures are available in the respective notebooks.

---

## 📁 Repository Structure
```bash
├── IMPR 1 normal.ipynb
├── Gaussian_blur.ipynb
├── Histogram_equilisation.ipynb
├── Thresholding and Contour detection.ipynb
└── README.md
