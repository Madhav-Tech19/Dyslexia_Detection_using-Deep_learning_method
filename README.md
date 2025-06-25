# Dyslexia Detection from Handwritten Images using Deep Learning

This repository contains the implementation of the paper:

**[Deep Learning-Based Model for Detecting Dyslexia Using Handwritten Images](https://www.researchgate.net/publication/376751665)**  
*Yazeed Alkhurayyif, Abdul Rahaman Wahab Sait – Journal of Disability Research, 2023*

---

## 🧠 Overview

The project aims to detect dyslexia in children by analyzing their handwritten images using a lightweight deep learning pipeline. It employs image preprocessing, feature extraction using YOLOv7, and classification using a MobileNetV2 + SSD-Lite model.

---

## 🗂 Repository Structure

- `pre_processing.ipynb`  
  Applies image enhancement using CLAHE, resizing (512×512), normalization, and data augmentation.

- `training.ipynb`  
  Loads extracted features, builds and trains the classification model (MobileNetV2 + SSD Lite), evaluates performance metrics like accuracy, F1-score, mAP, and mIoU.

- `features.pkl`  
  Pickled feature vectors extracted using the YOLOv7 model, used for classification training.

---

## 🧰 Requirements

- Python 3.8+
- TensorFlow / Keras
- OpenCV
- NumPy
- Scikit-learn
- Matplotlib
- PyYAML (for YOLOv7 configuration if needed)

Install using:

```bash
pip install -r requirements.txt
```
## 📊 Dataset
We use the publicly available Dyslexia Handwriting Dataset from Kaggle (2019) and augment it with additional handwritten samples.

Classes:

Normal

Reversal (Dyslexia)

## 🪶 Model Architecture
YOLOv7 – Feature extraction

MobileNetV2 + SSD-Lite – Classification (normal vs dyslexic handwriting)

Adam Optimizer – Hyperparameter tuning

## 📌 Citation
@article{alkhurayyif2023dyslexia,
  title={Deep Learning-Based Model for Detecting Dyslexia Using Handwritten Images},
  author={Yazeed Alkhurayyif and Abdul Rahaman Wahab Sait},
  journal={Journal of Disability Research},
  volume={2},
  number={4},
  pages={89--98},
  year={2023},
  doi={10.57197/JDR-2023-0059}
}

## 🔖 License
This project is released under the MIT License.
