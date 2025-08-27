# Airfoil Self-Noise Prediction with Machine Learning

This repository contains the implementation and analysis of the **ENG345 Term Project**, where various machine learning models were applied to predict the **Scaled Sound Pressure Level (SPL)** of airfoils based on aerodynamic and acoustic features.

The project explores multiple regression techniques and neural network architectures to reduce reliance on computationally expensive CFD simulations in aeroacoustics.

---

## 📌 Project Overview
- **Objective:** Predict airfoil noise levels (SPL) using machine learning models.  
- **Dataset:** [NASA Airfoil Self-Noise Dataset (UCI ML Repository)](https://archive.ics.uci.edu/dataset/291/airfoil+self+noise)  
- **Features Used:**
  - Frequency  
  - Angle of Attack (AoA)  
  - Chord Length  
  - Free-Stream Velocity  
  - Suction-Side Displacement Thickness  
  - **Engineered Feature:** Reynolds Number = Free-Stream Velocity × Chord Length  

- **Target Variable:** Scaled Sound Pressure Level (SPL)  

---

## ⚙️ Methods Applied
The following regression models were implemented and compared:

1. **Linear Regression**  
2. **Polynomial Regression** (degree up to 4)  
3. **Random Forest Regressor**  
4. **Support Vector Regressor (SVR)** with RBF kernel  
5. **Artificial Neural Networks (ANN)**  
   - With **Stochastic Gradient Descent (SGD)**  
   - With **Mini-Batch Gradient Descent**  

---

## 📊 Results Summary
Performance was evaluated using **Mean Squared Error (MSE)** and **R² Score**:

- **Best Model:** Random Forest Regressor  
  - MSE ≈ **3.28**  
  - R² ≈ **0.93**  
- **Neural Networks (ANN):** Good performance with R² ≈ 0.81  
- **Polynomial Regression (deg=4):** R² ≈ 0.77  
- **Support Vector Regressor (RBF):** R² ≈ 0.72  
- **Linear Regression:** Weakest model (R² ≈ 0.56)  

📌 **Conclusion:** Random Forest achieved the best trade-off between accuracy and efficiency, significantly outperforming traditional regression methods.

## Notes
- **You can find detailed project as pdf file in the repository**
