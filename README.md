# Amazon ML Challenge 2024

## Feature Extraction from Images

This repository contains our solution for the **Amazon ML Challenge 2024**, focused on extracting entity values from product images. The challenge is to develop a robust pipeline for extracting key information, such as weight, volume, and dimensions, directly from images, which is critical in domains like healthcare, e-commerce, and content moderation.

---

## Problem Overview

In digital marketplaces, product images often lack detailed textual descriptions, necessitating an automated approach to extract crucial details. Our solution addresses this by:

1. Downloading and loading images from given URLs.
2. Extracting text content from images.
3. Preprocessing the extracted text.
4. Extracting desired entity values using advanced Natural Language Processing (NLP) techniques.

---

## Approach

### 1. Loading Images
- We utilized Python scripts to download product images from the provided public URLs.
- Efficient image handling was ensured using libraries like `Pillow` and `OpenCV`.

### 2. Text Extraction
- **OCR with Tesseract**: Leveraged Tesseract OCR and OpenCV for text extraction from images.
- Applied preprocessing techniques such as thresholding and noise removal to improve OCR accuracy.

### 3. Text Preprocessing
- Cleaned and standardized extracted text to remove unwanted characters and noise.
- Tokenized text for efficient entity value identification.

### 4. Desired Text Extraction
- Used custom **NLP pipelines** to identify and extract required entity values (e.g., weight, volume) from the preprocessed text.
- Ensured output consistency with predefined allowed units using mappings from `constants.py`.

---

## Solution Highlights
- **Accuracy**: Optimized F1 score through precise text extraction and preprocessing techniques.
- **Scalability**: Designed to handle large datasets with varied image formats and text complexities.
- **Modularity**: Each component is modular for easier testing and improvements.

---
