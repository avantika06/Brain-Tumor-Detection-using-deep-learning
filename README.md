# Brain Tumor Detection & Report Generation using Deep Learning

## Project Overview
This project aims to develop a machine learning-based approach for brain tumor detection using MRI scans. By utilizing both traditional machine learning models (Support Vector Machine and Random Forest) and deep learning techniques (Convolutional Neural Network), we provide an efficient and automated system for detecting and classifying brain tumors into three categories: Glioma, Meningioma, and Pituitary tumors.


## Motivation
Brain tumors pose a significant health risk, and early detection is crucial for effective treatment. Traditional diagnostic methods involve invasive procedures and expensive imaging techniques. Our project leverages machine learning and deep learning to provide a non-invasive, cost-effective, and efficient solution for brain tumor detection.


## Objectives
- Implement and compare traditional machine learning models (SVM, Random Forest) for brain tumor classification.
- Develop a deep learning model (CNN with EfficientNet) for improved accuracy in tumor detection.
- Utilize Grad-CAM to highlight key image regions influencing model predictions.
- Evaluate model performance using accuracy, precision, recall, F1-score, and confusion matrix.

---

## Dataset
The dataset used in this project was sourced from Kaggle and consists of **7,023 MRI scans** categorized into:
- **Glioma**
- **Meningioma**
- **Pituitary**
- **No Tumor**

## Data Preprocessing
- **Grayscale Conversion**: Standardizes color channels to enhance feature extraction.
- **Scaling & Resizing**: Ensures uniformity in image dimensions.
- **Feature Extraction**:
  - Gaussian Blurring
  - Gabor Filters
  - Gray-Level Co-occurrence Matrices (GLCM)
- **Deep Learning Preprocessing**:
  - EfficientNet architecture for feature extraction and classification.

## Methodologies
### 1. Support Vector Machine (SVM)
- Used for classification based on extracted features.
- Achieved **76% accuracy**.
- Strong performance for **Pituitary (82%)**, weaker for **Meningioma (61%)**.

### 2. Random Forest
- Ensemble learning technique using multiple decision trees.
- Achieved **89% accuracy**.
- Strong detection for **No Tumor (94%)** and **Pituitary (92%)** but requires improvement for other classes.

### 3. Convolutional Neural Network (CNN)
- Utilized **EfficientNet** for feature extraction.
- Achieved **92.12% accuracy**.
- Integrated **Grad-CAM** for explainability by highlighting key MRI regions responsible for tumor classification.

## Evaluation Metrics
- **Accuracy**: Overall model correctness.
- **Precision**: Ratio of true positive predictions to total predicted positives.
- **Recall**: Ratio of true positive predictions to total actual positives.
- **F1-score**: Harmonic mean of precision and recall.
- **Confusion Matrix**: Visualization of model prediction performance.

---

## Results
| Model | Accuracy | Glioma Precision | Meningioma Precision | Pituitary Precision | No Tumor Precision |
|--------|----------|------------------|----------------------|----------------------|------------------|
| SVM | 76% | 83% | 61% | 88% | 89% |
| Random Forest | 89% | 89% | 80% | 92% | 94% |
| CNN (EfficientNet) | 92.12% | 91% | 85% | 94% | 97% |

### Grad-CAM Visualization
- Highlights critical regions in MRI scans that influence classification.
- Provides **explainability** to medical practitioners.

---



## Conclusion
- **CNN with EfficientNet** outperformed traditional ML models, achieving **92.12% accuracy**.
- **Grad-CAM** provided interpretability, making deep learning more useful for medical applications.
- The project demonstrates **strong potential for AI-assisted medical diagnostics**, paving the way for future advancements in brain tumor detection.

