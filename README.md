# Real-Time Macro Nowcasting & Risk Tracking System

An institutional-grade macroeconomic dashboard that extracts real-time economic signals and quantifies recession risk using data pipeline automation, unsupervised machine learning, and predictive regressions.

## 🚀 Key Features
- Automated Data Pipeline: Fetches 30 distinct macroeconomic indicators spanning credit, production, labor, and housing directly via the St. Louis Fed (FRED) API.
- Data Engineering & Stationarity: Cleans ragged data edges, aligns reporting frequencies to a consistent monthly grid, and applies appropriate stationarity transformations (YoY%, YoY Differences, Levels).
- Signal Extraction via PCA: Utilizes Principal Component Analysis (PCA) to extract the underlying common denominator from noisy macroeconomic data to build a Composite Activity Index.
- Recession Nowcasting: Employs a Probit statistical regression model to compute the real-time probability of the economy currently experiencing a recession.
- 12-Month Predictive Modeling: Runs an independent forward-predictive model utilizing the Treasury Yield Curve (10Y-3M spread) to flag mid-term economic shifts.

## 📊 Dashboard View
Tip: Insert your final dashboard screenshot here! To do this, drag and drop your dashboard image directly into this Markdown editor file, and GitHub will auto-generate the image tag.

## 🛠️ Tech Stack
- Language: Python
- Data Infrastructure: Pandas, NumPy
- Modeling & Analytics: Scikit-Learn (PCA), Statsmodels (Probit Regression)
- Visualization: Interactive Plotly graphics
- Data Source: Federal Reserve Economic Data (FRED) API
