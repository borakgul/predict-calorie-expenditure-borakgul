# 🔥 Calories Burned Prediction – Kaggle Playground S5E5

This project was developed for the [Kaggle Playground Series - Season 5 Episode 5](https://www.kaggle.com/competitions/playground-series-s5e5) competition.  
The goal was to build a regression model that predicts the number of calories burned during physical activity based on physiological data.

---

## 📌 Overview

The dataset includes features such as:
- Age, Height, Weight
- Duration of activity
- Heart rate and body temperature
- Sex (encoded)

The target variable is `Calories`, which was predicted using various machine learning models.

---

## ⚙️ Features & Techniques

- 📐 **Feature Engineering**: BMI, Intensity, Age × BMI, Cardio Effort
- 🔢 **Label Encoding**: Converted `Sex` to numeric values
- 📉 **Log1p Transformation**: Applied to the target (`Calories`) to improve stability
- 📊 **Models Used**:
  - XGBoost
  - CatBoost
  - MLP (Keras/TensorFlow)
- 🔗 **Ensemble Method**: Weighted average (XGB: 0.45, CatBoost: 0.45, MLP: 0.10)

---

## 📈 Model Performance (Validation RMSE - log)

| Model     | Validation RMSE (log) |
|-----------|------------------------|
| XGBoost   | ~0.064                 |
| CatBoost  | ~0.0603                |
| MLP       | ~0.1988                |
| **Ensemble** | **0.06138**         |

---

## 🗂️ Files in This Repository

| File                      | Description                         |
|---------------------------|-------------------------------------|
| `predict-calories.ipynb`  | Full notebook with all steps        |
| `submission_xgb_fe.csv`   | XGBoost predictions                 |
| `submission_cb_fe.csv`    | CatBoost predictions                |
| `submission_nn_fe.csv`    | MLP predictions                     |
| `submission_ensemble.csv` | Final ensemble predictions          |

---

## 🚀 How to Run

You can open and run the notebook on [Kaggle Notebooks](https://www.kaggle.com/code) or locally using Jupyter:

```bash
pip install -r requirements.txt
jupyter notebook
```
## 🙏 Acknowledgements
### Thanks to Kaggle for organizing the Playground Series.
The competition provided a great opportunity to experiment with ensemble modeling and feature engineering.

## 📬 Author
### Bora AKGUL, Here is my personal website: **[www.borakgul.com](https://www.borakgul.com)**

## License

This project is licensed under the MIT License.
