# Power Transformation on Crop Yield Dataset 🌾

This project demonstrates the application of **Power Transformation** techniques to improve prediction accuracy on a **Crop Yield Dataset**. The model uses **7 agricultural parameters** to predict both the **R² score** and the **total yield**.

---

## 📘 Overview

Power transformation techniques are used to make data **more Gaussian-like**, especially when features are skewed. This helps machine learning models perform better.

---

## 🚜 Dataset

The dataset contains multiple samples with features related to crop conditions, such as:
- Soil type
- Rainfall
- Temperature
- Fertilizer usage
- Seed quality
- Irrigation level
- Pesticide use

**Target Variable**: Total Crop Yield

---

## 🔄 Transformation Techniques Used

### 1. **Box-Cox Transformation**
- Requires input to be **positive**.
- Stabilizes variance and makes the data more normal-like.

### 2. **Yeo-Johnson Transformation**
- Works on both **positive and negative** values.
- Useful when the dataset has a mix of value ranges.

Both transformations were applied using `sklearn.preprocessing.PowerTransformer`.

---

## 🧠 Workflow

1. Load and explore the crop yield dataset.
2. Identify skewed features.
3. Apply `Box-Cox` and `Yeo-Johnson` transformations.
4. Split the data into train and test sets.
5. Train a regression model.
6. Predict total yield and compute **R² score**.

---

## 📈 Model Output

- **R² Score**: Indicates how well the model explains variance in the yield.
- **Predicted Total Yield**: Based on 7 input features.

---

## 🛠️ Libraries Used

- `pandas`, `numpy` for data handling
- `matplotlib`, `seaborn` for visualization
- `sklearn` for modeling and power transformations

---

## 🔧 Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
