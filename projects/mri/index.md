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
