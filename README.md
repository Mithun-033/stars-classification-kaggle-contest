# ⭐ Stars Classification – Kaggle Contest

This repository contains my solution for the **Kaggle Stars Classification** competition.  
The goal is to predict the **TargetClass** of stars using astrophysical features such as color index, absolute magnitude, and extracted spectral properties.

The project implements a complete **end-to-end machine learning pipeline** including preprocessing, feature engineering, model training, evaluation, and Kaggle submission generation.

---

## 📂 Project Structure

Star.ipynb  
&nbsp;&nbsp;↳ Main notebook (EDA, training, evaluation, prediction)

model6.pth  
&nbsp;&nbsp;↳ Trained PyTorch model

spec_enc.pkl  
&nbsp;&nbsp;↳ Saved LabelEncoder for SpectralClass

lum_enc.pkl  
&nbsp;&nbsp;↳ Saved LabelEncoder for LuminosityClass

scaler.pkl  
&nbsp;&nbsp;↳ Saved StandardScaler

submission.csv  
&nbsp;&nbsp;↳ Kaggle submission file

README.md  
&nbsp;&nbsp;↳ Project documentation

---

## 🧠 Features Used

- **B-V** – Color index (temperature indicator)
- **Amag** – Absolute magnitude
- **SpectralClass** – Extracted from spectral type
- **SubClass** – Numeric spectral subclass
- **LuminosityClass** – Extracted stellar luminosity class

---

## ⚙️ Feature Engineering

- Parsed `SpType` to extract spectral class, subclass, and luminosity class
- Encoded categorical features using `LabelEncoder`
- Scaled numerical features using `StandardScaler`
- Saved encoders and scaler to ensure consistent preprocessing on test data

---

## 🧪 Model

- Framework: **PyTorch**
- Architecture: Fully connected neural network with ReLU activations
- Loss Function: `BCEWithLogitsLoss`
- Optimizer: `AdamW`
- Task: Binary classification

---

## 📈 Evaluation

- Metric: **Accuracy**
- Local validation accuracy: **~97%**
- Loss curves monitored to ensure stable convergence

---

## 📤 Kaggle Submission

- Generated predictions on the test set using saved preprocessing artifacts
- Exported results to `submission.csv` in the required format

---

## 🚀 How to Run

1. Clone the repository
2. Install required dependencies
3. Open and run `Star.ipynb`
4. Upload `submission.csv` to Kaggle

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- PyTorch
- Matplotlib, Seaborn

---

## 🔗 Competition Link

https://www.kaggle.com/competitions/stars-classification

---

## 👤 Author

**Mithun**  
GitHub: https://github.com/Mithun-033
