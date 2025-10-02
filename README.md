# NFL Betting Model
Project Overview:

# 🏈 NFL Betting Model: Over/Under Predictions

## 💡 Project Overview

This repository contains the source code and data for an NFL betting model designed to predict the **Over/Under** outcomes of NFL games using historical data and machine learning.

---

## 🚀 Latest Updates & Status

The model has been **updated and re-calibrated for the 2025 NFL season** and is now focused on the single, enhanced **Model 2.0** architecture.

* **Maintenance:** The repository will receive new predictions and model-tuning updates **almost every other week** throughout the NFL season.
    * As of 10/04/2024: **64% success rate**

---

## 🧠 Current Model Development

The core of the project is the enhanced Version 2.0 of the model, which uses a **KNeighborsClassifier** with several critical improvements for stability and accuracy:

* **Data Preprocessing Pipeline:** Pipelines are implemented to streamline data cleaning and preparation.
* **Outlier Handling (LOF):** **Local Outlier Factor (LOF)** is used to identify and handle anomalous data points, making the model more robust.
* **Data Scaling:** Numerical features are scaled to ensure they are on a similar range, preventing features with large values from dominating the model.
* **Feature Selection (Masks):** Masks are used to selectively include or exclude features during training and evaluation for optimal performance.

***

## 📊 Data Acquisition

* **NFL Data:** Historical NFL data was scraped from NFL Pro-Reference for the seasons **2014 to 2023** to create a comprehensive dataset.
* **Vegas Lines:** Vegas lines for all the seasons were also scraped and stored in separate CSV files.

---

## 📁 Repository Structure

| File Name | Description |
| :--- | :--- |
| `Model2.0.ipynb` | The Jupyter Notebook containing the current, fully implemented version of the model (Version 2.0) logic and prediction code. |
| `NFL_Data_2025.ipynb` | Code used for scraping, cleaning, and extending the data for the new 2025 season. |
| `nfl_gamelogs_2015-2024_NEW.csv` | The raw NFL game logs data used by the model. |
| `nfl_gamelogs_vegas_2015-2024_NEW.csv` | The combined game logs and Vegas lines data. |
| `nfl_vegas_lines_2015-2024_NEW.csv` | The raw historical Vegas lines data. |

---

## ✨ Future Work

Future updates will focus on incorporating the following enhancements to boost accuracy:

* Implement the planned feature for **weighted games and seasons** to give more importance to recent data.
* Explore additional features and data sources to improve model accuracy.
* Experiment with different machine learning algorithms and techniques.
* Implement real-time betting strategies based on model predictions.
