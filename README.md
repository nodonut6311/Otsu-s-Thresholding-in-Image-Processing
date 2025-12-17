# Optical Character Recognition & Image Thresholding with OpenCV and Tesseract

This repository contains **two Google Colab notebooks** that introduce fundamental computer vision concepts using **OpenCV**, **Tesseract OCR**, and **Python**.

The goal of this project is to build **strong intuition around OCR preprocessing**, intensity histograms, and **automatic thresholding** — essential skills for anyone getting started with **computer vision, machine learning, and deep learning**.

---

##  Contents

### 1. Basic OCR using Tesseract
**Notebook:** `tesseract_impl.ipynb`

This notebook demonstrates how to:
- Read an image using OpenCV
- Convert the image to grayscale
- Apply binary thresholding
- Extract text using **Tesseract OCR (via pytesseract)**

 Focus:
- Understanding the OCR pipeline
- Learning why preprocessing improves text recognition
- Working with clean black-text-on-white-background images

---

### 2. Grayscale Intensity Histogram & Otsu’s Thresholding
**Notebook:** `Otsu's.ipynb`

This notebook focuses on **data-driven threshold selection** by:
- Plotting the **grayscale intensity histogram**
- Using a **log-scaled histogram** to visualize pixel distributions
- Applying **Otsu’s thresholding** to compute the optimal threshold automatically
- Visualizing the chosen threshold on the histogram

 Focus:
- Understanding how pixel intensity distributions work
- Eliminating arbitrary threshold values
- Learning histogram-based segmentation concepts

---

## Modules Required 
```bash
import cv2
import pytesseract
import matplotlib.pyplot as plt
```
Define path :
```bash
pytesseract.pytesseract.tesseract_cmd = "/usr/bin/tesseract"
```

---
##  Key Concepts Covered

- Grayscale conversion
- Image intensity histograms
- Log-scaled histogram visualization
- Binary thresholding
- Otsu’s automatic threshold selection
- OCR preprocessing with OpenCV
- Text extraction using Tesseract

---

##  How to Run

Each notebook is designed to run entirely in **Google Colab**.

1. Open the notebook in Colab
2. Run the installation cells
3. Upload your own image when prompted
4. Execute the cells step-by-step to observe the results

No local setup required.

---

##  Notes

- These notebooks focus on **printed text**, not handwritten text
- Images with a **white background and dark text** work best
- Deep learning OCR models are intentionally avoided to emphasize fundamentals

---

## Future Improvements

- Adaptive thresholding for uneven lighting
- Morphological operations for noise removal
- Deep learning OCR comparison (EasyOCR / TrOCR)
- Word-level bounding box visualization
- Multi-language OCR support


