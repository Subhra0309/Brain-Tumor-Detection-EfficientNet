# Brain Tumor Detection Using EfficientNet

## Overview

Brain tumors are among the most serious neurological disorders and require accurate diagnosis for effective treatment. Manual MRI analysis is time-consuming and depends heavily on radiologist expertise.

This project presents a deep learning-based brain tumor classification system using Convolutional Neural Networks (CNNs) and EfficientNet architectures. The system classifies MRI images into four categories:

* Glioma Tumor
* Meningioma Tumor
* Pituitary Tumor
* No Tumor

The objective is to assist medical professionals by providing an automated and reliable diagnostic support system.

---

## Dataset

**Dataset:** Brain Tumor MRI Dataset

Source:
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

### Classes

* Glioma
* Meningioma
* No Tumor
* Pituitary

### Dataset Statistics

| Split      | Images |
| ---------- | ------ |
| Training   | 4480   |
| Validation | 1120   |
| Testing    | 1600   |

Total classes: 4

---

## Methodology

### Data Preprocessing

* MRI image loading
* RGB to grayscale conversion
* Image resizing
* Data augmentation
* Normalization

### Models Implemented

#### 1. Custom CNN

* Convolutional Neural Network
* Adam Optimizer
* Binary Cross Entropy Loss

#### 2. EfficientNet-B3

* Transfer Learning
* Frozen backbone training
* Fine-tuning of deeper layers

#### 3. EfficientNet-V2-S

* Transfer Learning
* Feature extraction
* Fine-tuning

---

## Project Workflow

MRI Images
→ Preprocessing
→ Data Augmentation
→ Model Training
→ Validation
→ Testing
→ Tumor Classification

---

## Results

### Model Performance

| Model             | Accuracy |
| ----------------- | -------- |
| CNN               | 89.12%   |
| EfficientNet-B3   | 93.87%   |
| EfficientNet-V2-S | 94.06%   |

### Best Model

EfficientNet-V2-S achieved the highest test accuracy of **94.06%**.

---

## Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-Learn
* PIL
* Seaborn

---

## Repository Structure

```text
Brain-Tumor-Detection-EfficientNet/
│
├── notebooks/
│   └── Brain_Tumor_Classification.ipynb
│
├── reports/
│   └── Final_Report.pdf
│
├── screenshots/
│   ├── resized_images.png
│   ├── cnn_accuracy_curve.png
│   ├── cnn_confusion_matrix.png
│   ├── efficientnet_b3_curve.png
│   ├── efficientnet_b3_cm.png
│   ├── efficientnet_v2_curve.png
│   ├── efficientnet_v2_cm.png
│   ├── model_comparison.png
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Subhra0309/Brain-Tumor-Detection-EfficientNet.git
```

Move into the project directory:

```bash
cd Brain-Tumor-Detection-EfficientNet
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Open the notebook:

```bash
jupyter notebook
```

Run:

```text
notebooks/Brain_Tumor_Classification.ipynb
```

Update dataset paths according to your local system before training.

---

## Future Improvements

* Deploy as a Streamlit web application
* Add model inference pipeline
* Integrate Grad-CAM visualization
* Real-time MRI prediction
* Clinical validation on larger datasets
* Brain tumor segmentation support

---

## References

1. Brain Tumor MRI Dataset (Kaggle)

2. Tan, M., & Le, Q. V.
   EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks.
   ICML 2019.

3. Sajjad, M., Khan, S., Muhammad, K., Wu, W., Ullah, A., & Baik, S. W.
   Multi-grade Brain Tumor Classification Using Deep CNN with Extensive Data Augmentation.
   Journal of Computational Science, 2019.

---

## Author

**Subhrajit Jana**

M.Sc. Computer Science  
Ramakrishna Mission Vivekananda Educational and Research Institute

GitHub: https://github.com/Subhra0309

Email: [subhrajitjana2018@gmail.com](mailto:subhrajitjana2018@gmail.com)

```
```
