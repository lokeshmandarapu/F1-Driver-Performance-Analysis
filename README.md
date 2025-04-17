# F1-Driver-Performance-Analysis

An R Markdown– and PowerPoint–based statistical computing project that explores Formula 1 driver performance from recent seasons, using principal component analysis (PCA), clustering, regression, and time‑series forecasting.

## 📊 Project Overview

- **Objective:**  
  – Reduce multivariate driver statistics (grid position, lap times, consistency, points) to two principal components.  
  – Cluster drivers into performance tiers (“Champions & Contenders,” “Midfield Performers,” “Developing Talents”).  
  – Forecast lap‑time trends for pit‑stop strategy using time‑series regression.  
  – Package insights in an interactive PPT deck for stakeholders.

- **My Role:**  
  Focused on **time‑series analysis** — modeling lap‑time degradation with XGBoost regression, evaluating R² and RMSE, and generating pit‑stop alerts based on predicted performance drops.

## 🗂 Data

- **Source:** Official F1 API plus CSVs (Results, Laps, Weather).  
- **Contents:**  
  - Race outcomes (grid position, finish position, points)  
  - Lap-level data (lap time, tire compound, sector splits)  
  - Weather metrics (temperature, humidity, wind)  

## ⚙️ Requirements

- **R** ≥ 4.0  
- **R packages:**  
  ```r
  install.packages(c(
    "tidyverse",
    "FactoMineR",
    "factoextra",
    "cli",
    "xgboost",
    "zoo"
  ))
