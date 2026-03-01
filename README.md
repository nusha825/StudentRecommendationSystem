# 🎓 Neural Network-Based University Event Recommender System

## 📌 Project Overview

This project implements a Deep Learning-based Content Recommender System designed to recommend university events to students based on their academic performance, interests, and participation behavior.

The system demonstrates an end-to-end Machine Learning pipeline including data preprocessing, feature engineering, neural network modeling, evaluation, and prediction.

## 🎯 Problem Statement

Universities conduct various academic, technical, sports, and cultural events.  
However, event notifications are often generic and not personalized.

This project answers:

How can student academic and interest data be used to intelligently recommend relevant event categories?


## 🏗 System Architecture

Student Data  
↓  
Data Cleaning & Preprocessing  
↓  
Feature Engineering  
↓  
Feature Scaling (StandardScaler)  
↓  
Train/Test Split  
↓  
Neural Network Model  
↓  
Softmax Probability Output  
↓  
Recommended Event Category  


## 📊 Dataset Features

The model uses structured student data including:

- GPA
- Interest_AcademicWorkshop
- Interest_CareerDev
- Interest_TechMeetups
- Interest_Sports
- Interest_CulturalPrograms
- Interest_SocialActivities
- ParticipatedBefore
- EventTypesAttended
- Hypothetical Event Preferences
- Skill Development Preferences

## 🧹 Data Preprocessing

- Missing values handled using fillna(0)
- Feature selection based on dataset availability
- Rule-based label creation
- StandardScaler used for normalization
- 80/20 train-test split with stratification

Why normalization?
Neural networks are sensitive to scale differences. Scaling improves convergence and stability.

## 🧠 Model Architecture

Dense (128, ReLU)  
Dropout (0.3)  
Dense (64, ReLU)  
Dropout (0.2)  
Dense (32, ReLU)  
Output Layer (Softmax – 4 Classes)

Optimizer: Adam  
Loss Function: Sparse Categorical Crossentropy  

## 📈 Evaluation Metrics

- Accuracy
- Precision (Weighted)
- Recall (Weighted)
- F1-Score
- Confusion Matrix

The confusion matrix shows strong diagonal dominance, indicating correct classification across major categories.

## 🎯 Sample Prediction

Example Output:

Predicted Category: Technical & Innovation  
Confidence Score: 0.87  

The model selects the category with highest Softmax probability.


## ⚠ Limitations

- Labels are rule-based (heuristic)
- Not a collaborative filtering system
- No real-time interaction tracking
- Cold-start problem not handled


## 🚀 Future Improvements

- Neural Collaborative Filtering
- Top-N Event Recommendation
- Real-time personalization
- REST API deployment (FastAPI)
- Cloud deployment (AWS/Azure)

## 🛠 Tech Stack

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

## ▶️ How to Run

1. Clone repository  
2. Install dependencies  
3. Run the notebook or main script  


## 👩‍💻 Author

Nusha AGF  
Machine Learning & Deep Learning Enthusiast
