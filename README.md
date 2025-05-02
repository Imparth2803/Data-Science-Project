# Skin Lesion Classification Using CNNs and ViTs

This project compares the performance of **Convolutional Neural Networks (CNNs)** and **Vision Transformers (ViTs)** on the **ISIC 2019 skin lesion dataset**. It investigates their strengths and weaknesses in classifying dermatoscopic images across multiple lesion types.

## Models Used
- **CNN (Keras/TensorFlow)**: Custom architecture with dropout, batch normalization, and L2 regularization.
- **ViT (PyTorch)**: Patch-based transformer encoder implemented from scratch.

## Dataset
- **ISIC 2019 Challenge Dataset
- Data sourced from: BCN_20000, HAM10000, MSK.
- Includes metadata on age, gender, anatomical site.

## Preprocessing
- Images resized to **64x64**.
- Normalized pixel values.
- Labels encoded for multiclass classification.

## Evaluation Metrics
- Accuracy
- Precision
- Recall 
- Specificity
- F1 Score

## Key Findings
- CNN achieved strong precision but struggled with recall for **melanoma** cases, showing signs of overfitting.
- ViT performed better in generalizing across validation data but required more data and computational resources.

## Dependencies
- Python 3.9+
- TensorFlow 2.x
- PyTorch 1.13+
- scikit-learn
- Matplotlib / Seaborn
- Google Colab (for GPU acceleration)

## How to Run
1. Clone the repository or upload the notebook to Google Colab.
2. Mount Google Drive and extract the ISIC 2019 dataset.
3. Run preprocessing cells.
4. Train CNN and/or ViT models.
5. Evaluate using classification report and confusion matrix.

---

**Author:** Parth Tawde  
**University of Hertfordshire – MSc Data Science**
