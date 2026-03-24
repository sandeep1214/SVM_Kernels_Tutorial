# 📊 SVM Kernels: Geometric Intuition & Performance Analysis

## 📌 Overview

This repository presents a comprehensive tutorial on **Support Vector Machines (SVMs)**, with a focus on understanding how different kernel functions influence decision boundaries and model performance.

**The tutorial explores:**
- Linear, Polynomial, and RBF kernels
- The concept of maximum margin hyperplanes
- The kernel trick and higher-dimensional mapping
- The effect of kernel choice on both simple and complex datasets

---

## 🎯 Learning Objectives

This project aims to:

- Explain the concept of **maximum margin hyperplanes**
- Demonstrate the **kernel trick** and its role in non-linear classification
- Compare **Linear, Polynomial, and RBF kernels**
- Analyse model behaviour on both **simple and complex datasets**
- Evaluate performance using **quantitative metrics**

---

## 📂 Project Structure

- `SVM_Kernels_Tutorial.ipynb` – Full tutorial with code, explanations, and visualisations  
- `images/` – Exported figures (decision boundaries and 3D surfaces)  
- `README.md` – Project overview and usage instructions  

---

## 🧠 Core Concepts

### 🔹 Maximum Margin Principle

SVMs aim to find the hyperplane that maximises the margin between classes, improving generalisation to unseen data.

### 🔹 Support Vectors

Only a subset of training points (support vectors) determine the decision boundary, making SVMs memory-efficient and robust.

### 🔹 Kernel Trick

Instead of explicitly transforming data into higher dimensions, SVMs use kernel functions to compute inner products efficiently in transformed feature spaces.

---

## ⚙️ Key Hyperparameters

### **C (Regularisation Parameter)**
Controls the trade-off between margin width and classification error.

- High C → low bias, risk of overfitting  
- Low C → higher bias, better generalisation  

### **γ (Gamma - RBF Kernel)**
Determines how far the influence of a single training example reaches.

- High γ → complex, tightly fitted boundaries  
- Low γ → smoother, more general boundaries  

---

## 📊 Dataset Strategy

### 1. Baseline: Iris Dataset

- 2 classes: Setosa vs Versicolor  
- 2 features: Petal length and width  
- Nearly linearly separable  

→ Used to demonstrate baseline kernel behaviour  

---

### 2. Challenge Case: Moons Dataset

- Synthetic non-linear dataset  
- Interleaving half-circles  

→ Used to highlight the limitations of linear kernels and the strength of RBF  

---

## 🧪 Experiments

### 🔹 Decision Boundary Visualisation

Each kernel is applied to both datasets to illustrate:

- Linear separability  
- Increasing boundary complexity  
- Kernel-induced transformations  

---

### 🔹 3D Decision Surface (RBF)

A 3D visualisation demonstrates how the RBF kernel effectively **maps data into a higher-dimensional space**, where a linear separation becomes possible.

---

### 🔹 Quantitative Evaluation

Model performance is evaluated using:

- Accuracy  
- Classification report (precision, recall, F1-score)  

---

## 📈 Results Summary

| Kernel     | Complexity | Iris Accuracy | Key Observation                       |
|------------|-----------|--------------|-------------------------------------|
| Linear     | Low       | ~95–100%     | Effective for linearly separable data |
| Polynomial | Medium    | ~95–100%     | Introduces controlled curvature       |
| RBF        | High      | ~100%        | Handles complex, non-linear patterns  |

### Key Insight

While all kernels perform well on the Iris dataset, the **Moons dataset clearly demonstrates that only the RBF kernel can correctly model non-linear structures**.

---

## 📊 Visualisations

This project includes:

- 2D decision boundary plots (colour-blind friendly)  
- Side-by-side kernel comparisons  
- 3D surface plots of decision functions  
- Descriptive text for accessibility  

---

## 🛠️ Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/sandeep1214/SVM_Kernels_Tutorial.git
cd SVM_Kernels_Tutorial
```

### 2. Install dependencies
```bash
pip install numpy matplotlib scikit-learn
```

### 3. Run the notebook
```bash
jupyter notebook SVM_Kernels_Tutorial.ipynb
```

---

## ⚠️ Model Selection Insights

Choosing the correct kernel is task-dependent:

### Linear Kernel
- Best for high-dimensional, sparse data (e.g. text classification)  
- Fast and interpretable  

### Polynomial Kernel
- Useful when feature interactions are important  
- Risk of overfitting with high degree  

### RBF Kernel
- Default choice for non-linear problems  
- Highly flexible but sensitive to hyperparameters  

---

## 💡 Intuition

> Complex non-linear decision boundaries in low-dimensional space often correspond to simple linear separations in higher-dimensional space.

The RBF kernel effectively "lifts" the data into this space, enabling linear separation of otherwise entangled patterns.

---

## 🧾 Conclusion

- Kernel choice fundamentally affects SVM performance  
- Linear models are efficient but limited  
- Polynomial kernels add controlled flexibility  
- RBF kernels provide powerful non-linear modelling  

👉 Effective use of SVM requires careful tuning of:

- C (regularisation)  
- γ (RBF kernel)  
- degree (polynomial kernel)  

---

## 📎 References

- Boser, B., Guyon, I., & Vapnik, V. (1992). *A Training Algorithm for Optimal Margin Classifiers*  
- Cortes, C., & Vapnik, V. (1995). *Support Vector Networks*  
- Bishop, C. M. (2006). *Pattern Recognition and Machine Learning*  
- Géron, A. (2019). *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow*  
- Scikit-learn Documentation: https://scikit-learn.org/stable/modules/svm.html  

---

## 🔗 Repository

https://github.com/sandeep1214/SVM_Kernels_Tutorial

---

## ♿ Accessibility Notes

- Colour-blind friendly colormap (`viridis`) used in all plots  
- Clear axis labels and titles  
- Visual descriptions included in tutorial for screen readers  
