# CNN-LSTM for Residential Energy Consumption Prediction

This project reproduces the key methodology and experiments from the paper  
**["Predicting residential energy consumption using CNN-LSTM neural networks"](https://doi.org/10.1016/j.energy.2019.03.015)** published in *Energy* (2019).

We implement a hybrid **CNN-LSTM** deep learning architecture for multivariate, multi-step forecasting of residential electricity consumption, and evaluate its performance across various time granularities: **minute**, **hour**, **day**, and **week**.

---

## Project Structure

```
.
├── Notebooks/             # Jupyter Notebooks for data preprocessing, modeling, and evaluation and pdf
├── Paper/                 # Sourse paper
└── README.md              # Project documentation
```

## 🚀 Getting Started

Run the main notebook

You can launch the core notebook in your environment (local or Colab):

```bash
jupyter Notebook notebooks/energy_prediction.ipynb
```

## 🧠 Model Overview

The implemented model follows the original paper's architecture:

* **2D Convolutional layers**: To extract spatial patterns from multivariate features
* **LSTM layer**: To capture temporal dependencies across time steps
* **Dense layers**: For multi-step output forecasting

Three models are compared:

* Linear Regression (baseline)
* LSTM
* CNN-LSTM (hybrid)

Each is evaluated on RMSE across multiple time resolutions.

---

## 📊 Dataset

* **Source**: UCI Machine Learning Repository
* **Dataset**: [Residential Building Data Set](https://archive.ics.uci.edu/ml/datasets/Residential+Building+Data)
* Contains time-stamped records of residential energy use and weather variables.

---

## 📄 Reference

> H. Yildiz, J. I. Bilbao, and A. B. Sproul, "Predicting residential energy consumption using CNN-LSTM neural networks," *Energy*, vol. 176, pp. 562–570, 2019.
> [DOI: 10.1016/j.energy.2019.03.015](https://doi.org/10.1016/j.energy.2019.03.015)

---

## 📜 License

This project is licensed under the MIT License.

---

