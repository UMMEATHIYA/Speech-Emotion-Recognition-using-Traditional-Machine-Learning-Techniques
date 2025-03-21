# Speech Emotion Recognition using Traditional Machine Learning Techniques

## Overview
This project focuses on Speech Emotion Recognition (SER), which enables machines to interpret human emotions from voice data. The study involves the use of traditional machine learning techniques and feature extraction methods to classify emotions from speech recordings.

## Dataset
The dataset used for this project is the **Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS)**, containing 7,356 recordings from 24 professional actors (12 male, 12 female). The dataset includes the following emotions:
- Neutral
- Calm
- Happy
- Sad
- Angry
- Fearful
- Disgust
- Surprised

## Feature Extraction
Feature extraction is a crucial step in SER, and the following features were extracted using **Librosa**:
- **Mel-Frequency Cepstral Coefficients (MFCCs)** – Captures timbre features
- **Chroma Features** – Captures harmonic and tonal aspects
- **Spectral Features** – Includes spectral centroid, bandwidth, and roll-off
- **Zero-Crossing Rate (ZCR)** – Identifies high-energy emotions
- **RMS Energy** – Differentiates high-energy (anger) and low-energy (sadness) emotions

## Methodology
Once the features were extracted, multiple traditional machine learning classifiers were trained and evaluated:

### Machine Learning Models
| Model | Accuracy |
|--------|------------|
| **Support Vector Machines (SVM)** | 70.23% |
| **Random Forest** | 68.45% |
| **K-Nearest Neighbors (KNN)** | 55.35% |
| **Logistic Regression** | 70.238% |
| **Multi-Layer Perceptron (MLP)** | 75.35% |

### Data Preprocessing
- **Normalization** – Scaled values for model consistency
- **Noise Reduction** – Applied filters for better speech clarity
- **Feature Selection** – Used Principal Component Analysis (PCA) and Recursive Feature Elimination (RFE)
- **Train-Test Split** – 75% training, 25% testing

## Challenges & Limitations
- **Background Noise** – Addressed using MFCCs and Log-Mel Spectrograms
- **Computational Cost** – Algorithms like SVM and KNN are expensive
- **Data Imbalance** – Handled with **Synthetic Minority Over-Sampling Technique (SMOTE)**
- **Feature Extraction Challenges** – Real-time processing constraints
- **Dataset Bias** – Limited to English accents

## Future Directions
- **Deep Learning Approaches** – CNNs, RNNs, Transformers for better feature extraction
- **Real-Time Processing** – Optimization for low-latency applications
- **Multi-Modal Learning** – Integrating speech with video for improved accuracy

## Conclusion
- Traditional machine learning techniques provide effective and interpretable results for SER.
- Feature extraction (MFCC, Spectrograms) plays a key role in classification.
- Future improvements may involve hybrid models combining deep learning and traditional approaches.

---

### Author
**Umme Athiya**  
Graduate Student, DePaul University  

For more details, refer to the **Final Project Report**.

