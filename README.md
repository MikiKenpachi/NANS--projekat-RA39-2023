# 📈 Analysis and Prediction of S&P 500 Short-Term Log-Returns

**Numerical Algorithms and Numerical Software (NANS) Course Project** *Faculty of Technical Sciences, University of Novi Sad*

---

## 📖 Project Overview

This project presents a comprehensive study focused specifically on the **analysis and prediction of short-term logarithmic returns (log-returns)** of the **S&P 500** index. 

The core objective is to model the financial time series using statistical and machine learning methods. Log-returns are utilized instead of raw price data as they are more suitable for achieving stationarity and providing a robust evaluation of high-frequency market movements and volatility.

> **Note:** While this documentation is in English for portfolio purposes, the **Jupyter Notebook analysis and comments are written in Serbian**, in accordance with the university course requirements.

### 📊 Methodology & Models
The study evaluates four distinct approaches to financial data:
* **ARIMA** – Linear modeling and analysis of autocorrelation structures to capture returns.
* **Facebook Prophet** – Non-linear modeling to identify underlying daily and weekly trends.
* **GARCH** – Advanced volatility modeling to assess risk and volatility clustering.
* **PCA Analysis** – Dimensionality reduction to understand the internal structure of market sectors.

---

## 🛠️ Tech Stack & Libraries

| Category | Tools |
| :--- | :--- |
| **Language** | Python 3.x |
| **Data Processing** | `Pandas`, `NumPy` |
| **Time Series** | `Statsmodels`, `pmdarima`, `Prophet`, `arch` |
| **Machine Learning** | `Scikit-learn` (PCA) |
| **Visualization** | `Matplotlib`, `Seaborn` |

---

## 📂 Project Structure

The repository is organized modularly to ensure clean code and easy maintenance:

* `notebook.ipynb` – **Main Entry:** Full analysis workflow and result interpretation (in Serbian).
* `preprocessing.py` – Data ingestion and log-return transformation.
* `stationarity.py` – Statistical testing (ADF test) and ACF/PACF analysis.
* `arima_model.py` – ARIMA implementation with **Walk-Forward Validation**.
* `prophet_model.py` – Non-linear trend forecasting using Facebook Prophet.
* `garch_model.py` – Volatility clustering analysis.
* `pca_analysis.py` – Principal Component Analysis of market sectors.
* `evaluation.py` – Centralized performance metrics (**MAE**, **RMSE**, **MASE**).

---

## 📈 Key Insights & Conclusions

* **Market Efficiency:** Log-returns exhibit properties close to white noise, confirming the high efficiency and unpredictability of short-term price movements.
* **Volatility Clustering:** Successfully captured and modeled using a **GARCH(1,1)** approach, showing that "shocks" in the market tend to persist.
* **Validation Integrity:** Used **Walk-Forward Validation** to eliminate *look-ahead bias*, strictly simulating real-world forecasting conditions.
* **PCA Findings:** The first principal component (**PC1**) captures the broad market movement, while **PC2** effectively separates cyclical from defensive sectors.

---

## 👥 Author
**Miloš Trišić** (RA 39/2023)  
*Department of Computing and Control / Applied Computer Science and Informatics*

## 📄 License
This project was developed for educational purposes at the **Faculty of Technical Sciences (FTN)**.
