# 🎗️ Breast Cancer Detection using Deep Learning

A deep learning project for classifying breast cancer mammography images as **benign** or **malignant** using multiple CNN architectures. Built and trained on the **CBIS-DDSM** dataset via Kaggle.

---

## 📌 Project Overview

Breast cancer is one of the leading causes of cancer-related deaths worldwide. Early and accurate detection is critical. This project applies transfer learning and custom CNN models to mammogram images to assist in the classification of mass pathology.

---

## 📂 Repository Structure

```
BreastCancerDetection/
│
├── FINAL_CODE.ipynb              # Main notebook: data loading, EDA, model training & evaluation
├── EXTRA_METHOD_GIT.ipynb        # Additional model: PCXRNet34 custom architecture
├── Research Paper.docx   # Full research paper
└── LINK OF THE DATA SET.docx     # Dataset source links
```

---

## 📊 Dataset

**CBIS-DDSM (Curated Breast Imaging Subset of DDSM)**

The dataset includes:
- Full mammogram images
- Cropped region-of-interest (ROI) images
- ROI mask images
- Mass case descriptions (train & test CSV files)

> 📎 Dataset links are available in `LINK OF THE DATA SET.docx`  
> Dataset source: [Kaggle - CBIS-DDSM Breast Cancer Image Dataset](https://www.kaggle.com/datasets/awsaf49/cbis-ddsm-breast-cancer-image-dataset)

---

## 🧠 Models Implemented

| Model | Type | Notes |
|---|---|---|
| **InceptionResNetV2** | Transfer Learning | Pre-trained on ImageNet |
| **ResNet50** | Transfer Learning | Fine-tuned last 5 layers |
| **VGG16** | Transfer Learning | Fine-tuned last 5 layers |
| **VGG19** | Transfer Learning | Fine-tuned last 5 layers |
| **PCXRNet34** | Custom CNN | Built from scratch (Extra Method) |

All models use:
- Binary classification: `BENIGN` vs `MALIGNANT`
- Optimizer: Nadam / Adam
- Loss: Categorical Crossentropy
- Metrics: Accuracy, AUC, F1-Score, Cohen's Kappa

---

## 🔧 Tech Stack

- Python 3
- TensorFlow / Keras
- OpenCV (`cv2`)
- Scikit-learn
- Pandas, NumPy
- Matplotlib, Seaborn
- TensorFlow Addons (`tensorflow_addons`)

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/BreastCancerDetection.git
   cd BreastCancerDetection
   ```

2. **Set up the dataset**  
   Download the CBIS-DDSM dataset from Kaggle and place it under:
   ```
   ../input/cbis-ddsm-breast-cancer-image-dataset/
   ```
   Or run directly on **Kaggle Notebooks** (recommended — no setup needed).

3. **Open the notebook**
   ```bash
   jupyter notebook FINAL_CODE.ipynb
   ```

> ✅ Recommended: Run on [Kaggle](https://www.kaggle.com) for GPU access and pre-loaded dataset paths.

---

## 📈 Results

Training and validation accuracy curves are plotted for each model. Evaluation metrics include:
- Accuracy
- AUC (Area Under ROC Curve)
- F1 Score
- Cohen's Kappa

Refer to `FINAL_CODE.ipynb` for full results and `Research Paper.docx` for detailed analysis.

---

## 👩‍💻 Author

**Umme Tasneem Firdose**  
📄 [Research Paper included in repository]

---

## 📜 License

This project is for academic and research purposes only.
