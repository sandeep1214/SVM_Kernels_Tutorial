# 📊 SVM Kernels Tutorial – Understanding Decision Boundaries

## 📌 Overview
This project explores **Support Vector Machines (SVMs)** and demonstrates how different kernel functions affect decision boundaries.

Using the **Iris dataset**, we visualize how:
- Linear kernels create straight decision boundaries  
- Polynomial kernels introduce curvature  
- RBF kernels model complex, non-linear relationships  

The goal is to build intuition around the **kernel trick** and how SVMs handle non-linear data.

---

## 🧠 Objectives
- Understand how SVM works for classification  
- Compare different kernel functions:
  - Linear
  - Polynomial
  - RBF (Gaussian)  
- Visualize decision boundaries in 2D  
- Explore how kernel choice impacts model performance  

---

## 📂 Dataset
We use the **Iris dataset** with the following setup:
- Features:  
  - Petal Length  
  - Petal Width  
- Classes:
  - Setosa  
  - Versicolor  
- Total samples used: **100 (binary classification)**  

---

## ⚙️ Technologies Used
- Python  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## 🚀 Project Workflow

### 1. Data Preparation
- Load dataset from `sklearn.datasets`
- Filter to 2 classes for visualization
- Split into train/test sets
- Standardize features using `StandardScaler`

---

### 2. Models Implemented

#### 🔹 Linear Kernel
- Creates a **straight-line decision boundary**
- Works best for **linearly separable data**
```python
SVC(kernel='linear', C=1.0)
```
#### 🔹Polynomial Kernel
- Produces curved decision boundaries
- Controlled by degree parameter  
```python
SVC(kernel='poly', degree=3, C=1.0)
```
#### 🔹 RBF (Gaussian) Kernel
- Maps data into higher-dimensional space
- Handles complex non-linear patterns
```python
SVC(kernel='rbf', C=1.0, gamma=0.5)

```

---
## 📈 Visualizations

### ✅ Decision Boundaries
Each kernel is visualized using a 2D plot showing:
- Data points
- Classification regions
- Decision boundary
  
### ✅ 3D Visualization (RBF)
- Displays the decision function surface
- Helps understand how non-linear separation works in higher dimensions

  ---

  
## 🧪 Key Concepts

### 🔹 Kernel Trick
Instead of explicitly transforming data, SVM computes inner products in higher-dimensional space using kernel functions.

### 🔹 Why Kernels Matter
- Linear kernel → simple, interpretable
- Polynomial kernel → moderate complexity
- RBF kernel → highly flexible

**Choosing the wrong kernel can lead to:**
- Underfitting
- Overfitting

  ---
  
## 📊 Results Summary
| Kernel     | Behavior                        | Use Case                    |
| ---------- | ------------------------------- | --------------------------- |
| Linear     | Straight boundary               | Linearly separable data     |
| Polynomial | Smooth curved boundary          | Moderate non-linearity      |
| RBF        | Highly flexible, complex shapes | Complex/non-linear patterns |

---

## 💡 Intuition

A key insight:
- Non-linear boundaries in 2D often become linear in higher dimensions.
- The RBF kernel effectively transforms the data so that a linear separator can exist in that higher-dimensional space.

  ---

## 🧾 Conclusion
- Kernel selection is critical in SVM performance
- Linear is simple and fast
- Polynomial adds controlled complexity
- RBF is powerful but sensitive to parameters

  ---

### 👉 Always experiment with:
- C (regularization)
- degree (polynomial)
- gamma (RBF)

 ---
  
## 📎 References
- Boser, Guyon, Vapnik (1992) – Optimal margin classifiers
- Cortes & Vapnik (1995) – Support Vector Networks
- Scikit-learn Documentation - https://scikit-learn.org/stable/modules/svm.html

  ---

## 🔗 Repository
https://github.com/sandeep1214/SVM_Kernels_Tutorial
