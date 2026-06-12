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
├── FINAL_CODE.ipynb              # Main notebook: data loading, EDA, all model training & evaluation
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

> 📎 Dataset source: [Kaggle - CBIS-DDSM Breast Cancer Image Dataset](https://www.kaggle.com/datasets/awsaf49/cbis-ddsm-breast-cancer-image-dataset)

---

## 🧠 Models & Results

All models trained for **10 epochs** with binary classification: `BENIGN` vs `MALIGNANT`

| Model | Test Accuracy | Test AUC | F1 Score |
|---|---|---|---|
| **DenseNet169** | 72.35% | 0.7677 | 0.7184 |
| **DenseNet121** | 70.59% | 0.7447 | 0.6988 |
| **InceptionResNetV2** | 64.12% | 0.6996 | 0.6332 |
| **MobileNetV2** | 61.76% | 0.6479 | 0.6176 |
| **MobileNet** | 60.00% | 0.6516 | 0.5995 |
| **VGG16** | 57.06% | 0.6337 | 0.5317 |
| **InceptionV3** | 59.41% | 0.6462 | 0.5865 |
| **ResNet50** | 52.35% | 0.5857 | 0.4804 |
| **ResNet101** | 54.71% | 0.6122 | 0.3536 |
| **VGG19** | 47.65% | 0.5179 | 0.4370 |

> 🏆 **Best performing model: DenseNet169** with 72.35% accuracy and 0.7677 AUC

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
   git clone https://github.com/UmmeTasneem/BreastCancerDetection.git
   cd BreastCancerDetection
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the dataset**  
   Download the CBIS-DDSM dataset from Kaggle and place it under:
   ```
   ../input/cbis-ddsm-breast-cancer-image-dataset/
   ```
   Or run directly on **Kaggle Notebooks** (recommended — no setup needed).

4. **Open the notebook**
   ```bash
   jupyter notebook FINAL_CODE.ipynb
   ```

> ✅ Recommended: Run on [Kaggle](https://www.kaggle.com) for GPU access and pre-loaded dataset paths.

---

## 📈 Evaluation Metrics

Each model is evaluated using:
- **Accuracy** — overall classification correctness
- **AUC** — Area Under the ROC Curve
- **F1 Score** — balance between precision and recall
- **Cohen's Kappa** — agreement beyond chance

---

## 👩‍💻 Author

**Umme Tasneem Firdose**  
📄 Research paper included in repository

---

## 📜 License

This project is for academic and research purposes only.
