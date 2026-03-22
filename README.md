# SVM Kernels and Their Effect on Decision Boundaries

This repository contains an educational tutorial on **Support Vector Machines (SVM)**. The focus is on demonstrating how different kernel functions (Linear, Polynomial, and RBF) transform data and influence the shape of decision boundaries.

## 🚀 Tutorial Overview
This tutorial is designed to teach users the mathematical intuition and practical implementation of SVM kernels using the Iris dataset.

### Key Technical Concepts Covered:
- **The Kernel Trick:** Understanding how data is mapped to higher-dimensional spaces.
- **Mercer's Theorem:** The mathematical requirements for a function to be a valid kernel.
- **Lagrangian Dual Problem:** How SVM optimization is solved in practice.
- **Hyperparameter Tuning:** Exploring the effects of `degree` (Polynomial) and `gamma` (RBF).

## 📊 Visualizations
The tutorial includes high-quality, color-blind friendly visualizations:
- **2D Decision Boundaries:** Comparing Linear, Polynomial, and RBF separations.
- **3D Surface Plots:** Visualizing the RBF decision function's "elevation" in feature space.

## ♿ Accessibility Features
This project was built with accessibility in mind to ensure all learners can benefit:
- **Color-Blind Friendly:** Uses the `Viridis` colormap, which is perceptually uniform.
- **Alternative Text:** Detailed Markdown descriptions are provided below every figure for screen-reader users.
- **Structural Clarity:** Uses hierarchical headers and LaTeX for mathematical notation.

## 🛠️ How to Run the Code
To reproduce the plots and analysis locally:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/sandeep1214/SVM_Kernels_Tutorial.git](https://github.com/sandeep1214/SVM_Kernels_Tutorial.git)
2. **Install Dependencies:**
   Ensure you have Python installed, then run:
   ```bash
   pip install numpy matplotlib scikit-learn
3. **Open the Notebook:**
   Launch Jupyter Notebook or JupyterLab and open
   `24174419_SVM_Kernels_Tutorial_.ipynb`

## 📚 References
- Boser, B., Guyon, I., & Vapnik, V. (1992). A training algorithm for optimal margin classifiers.
- Cortes, C., & Vapnik, V. (1995). Support-vector networks. Machine Learning.
- Scikit-learn Documentation: [SVM Module](https://scikit-learn.org/stable/modules/svm.html)
