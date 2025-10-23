---
layout: default
---
# MRI Image Analysis Portfolio

## Project Overview
This project showcases the application of advanced **deep learning techniques** to the analysis of **magnetic resonance imaging (MRI)** datasets for **brain cancer detection and classification**. Originally developed as part of exploratory work in image-based science beyond astronomy, it applies methods honed in spectral and imaging data science to biomedical imaging.

---

## Objective
The main goal of this study is to automatically classify MRI brain scans into cancer types — **glioma**, **meningioma**, and **pituitary** — and identify non-cancerous cases using state-of-the-art computer vision models.

---


## Data Sources
- **Kaggle Brain Tumor MRI Dataset** — A large-scale dataset containing MRI images of diagnosed brain tumors.
- **The Cancer Imaging Archive (TCIA)** — Supplementary MRI data from the *Brain Tumor Progression* collection.


Combined, these datasets provided approximately **6,000 labeled MRI images** for model training and evaluation.


---


## Methods
- **Preprocessing & Labeling**: Performed with **Roboflow**, used for dataset organization and augmentation. Techniques included rotation, blurring, cropping, and brightness adjustments to improve model robustness.
- **Model Training**:
- Initial model: **YOLO (You Only Look Once)** — used for rapid object detection and localization.
- Current implementation: **PyTorch CNN classifier** for tumor-type classification.
- **Data Augmentation**: Applied transformations such as random rotations, Gaussian blurring, and adaptive cropping to expand the effective dataset size and mitigate overfitting.


---


## Model Performance
The **PyTorch CNN model** achieved an impressive **98.6% accuracy** on validation data.


### Common failure case
- **Issue**: Misclassification when MRI images were too dark.
- **Solution**: Retrained the model with additional brightness-adjusted images to improve robustness to illumination variation.


---

## Results Summary

| Tumor Type | Detection Accuracy |
|-------------|--------------------|
| Glioma      | 100%               |
| Meningioma  | > 87%              |
| Pituitary   | ~98%               |
| No Cancer   | Correctly classified in most cases |

<style>
table {
  border-collapse: collapse;
  margin: 1.5rem auto;
  width: 90%;
  max-width: 700px;
  background: rgba(0,0,0,0.03);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 0 20px rgba(0,0,0,0.1);
}
th, td {
  border: 1px solid rgba(0,0,0,0.1);
  padding: 0.75rem 1rem;
  text-align: center;
  color: #eee;
}
th {
  background: rgba(0,0,0,0.08);
  font-weight: 600;
  color: #fff;
}
tr:nth-child(even) {
  background: rgba(0,0,0,0.04);
}
tr:hover {
  background: rgba(0,0,0,0.12);
}
</style>



---


## Tools and Frameworks
- **Roboflow** — for dataset labeling and augmentation.
- **PyTorch** — for neural network implementation and training.
- **YOLOv5** — for initial object detection experiments.
- **NumPy**, **OpenCV**, **Matplotlib** — for preprocessing, visualization, and analysis.


---


## Conclusions
This project demonstrates that **AI-powered image analysis** methods commonly used in astrophysics can be successfully adapted for **medical imaging** tasks. The high classification accuracy underscores the potential for cross-disciplinary applications of machine learning in pattern recognition and data-driven diagnostics.


---
