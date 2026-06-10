# ML-Based-Transformer-Diagnostics-
An end-to-end Machine Learning pipeline bridging Power Systems and AI. By analyzing continuous operational data, this tool predicts transformer efficiency, estimates losses, and detects anomalies early—enabling smart grids to shift from reactive repairs to data-driven predictive maintenance for critical assets.
# ⚡ Transformer Performance Prediction via Machine Learning

This Industry 4.0 project bridges core Electrical Engineering and AI to predict power transformer performance. Using machine learning on operational data, the pipeline estimates losses, predicts efficiency, and detects early anomalies—shifting high-voltage asset management from reactive repairs to intelligent predictive maintenance.

## 📖 Overview
Power transformers are the critical backbone of modern electrical grids, but in traditional power systems, maintenance is often scheduled manually or executed only after a fault occurs—leading to severe downtime and massive replacement costs. This project solves that inefficiency by bridging core electrical engineering with Artificial Intelligence to develop an Industry 4.0 solution. By ingesting continuous operational data, the machine learning pipeline accurately predicts efficiency curves, estimates losses, and flags abnormal health statuses before hardware degradation happens. Ultimately, it serves as a robust proof-of-concept for integrating AI into high-voltage asset management, allowing operators to shift from reactive repairs to intelligent predictive maintenance.

## 🎯 Objectives
- **Performance Analysis:** Evaluate operational data to establish baseline performance metrics under fluctuating loads.
- **Efficiency & Loss Prediction:** Model and predict expected efficiencies and core/copper losses under varying operational factors.
- **Anomaly Detection:** Identify abnormal operating states and thermal behavior before they lead to critical hardware failures.
- **Asset Health Estimation:** Provide continuous health status monitoring for high-value grid components.
- **Predictive Maintenance:** Support preemptive maintenance scheduling to minimize footprint downtime and optimize grid reliability.

## 🛠️ Tech Stack
- **Data Engineering:** Python, Pandas, NumPy
- **Machine Learning:** Scikit-Learn (Random Forest Regressor, Isolation Forest)
- **Visualization:** Matplotlib
- **Development Environment:** Google Colab

## 🌐 Domain Applications
- Power Systems & Smart Grids
- Industrial Asset Management
- Industry 4.0 Automated Diagnostics

## 📊 Dataset Description
The model processes operational transformer data representing various load conditions and ambient states. Key parameters include:
- **Electrical Parameters:** Active Power (kW), Reactive Power (kVAR), Voltage (V), Current (A), and Power Factor.
- **Thermal Parameters:** Top Oil Temperature (TOT) and Winding Temperature Indicator (WTI) metrics.
- **Engineered Features:** Calculated Copper Losses ($I^2R$), fixed Core Losses, and theoretical operational efficiency formulas utilized to train baseline performance benchmarks.

📈 Key Results & Visualizations
(Note: Replace these placeholders with your actual screenshots from the images/ folder once your Colab Notebook runs successfully.)

DGA Ratio Mapping (Exploratory Data Analysis): Mapped standard industry Dissolved Gas Analysis (DGA) ratios to visually cluster transformer thermal states, clearly distinguishing between safe baseline operations and degraded zones (e.g., low-temperature heating vs. high-energy arcing).

Unsupervised Fault Isolation (Isolation Forest): Deployed a multi-dimensional anomaly detection algorithm to autonomously flag irregular chemical signatures. This pipeline successfully acts as an early warning predictive maintenance system without relying on historically labeled failure logs.
## 📂 Repository Structure
```text
├── data/
│   └── transformer_operational_data.csv   # Raw operational dataset
├── notebooks/
│   └── transformer_prediction.ipynb       # Main ML pipeline & EDA
├── images/
│   ├── dga_ratio_plot.png              # Visual plots for README documentation
│   └── anomalies_plot.png                 
└── README.md                              # Main project documentation
