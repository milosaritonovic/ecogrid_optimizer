# EcoGrid Optimizer: EV Infrastructure Analysis

## Project Overview
EcoGrid is a startup managing a national network of Electric Vehicle (EV) charging stations. This project serves as a comprehensive "Clean Energy Report" designed for stakeholders and investors. It demonstrates the ability to ingest raw, inconsistent sensor data, perform complex time-series analysis, and derive human-centric business insights.

## Technical Challenges Overcome
* **Data Sanitization:** Resolved significant "sensor noise" including inconsistent null values (`NaN`, `??`, `NULL`) and non-standard status strings.
* **Time-Series Alignment:** Implemented rolling 7-day averages and monthly resampling using the latest Pandas `ME` (Month-End) frequency standards to detect long-term trends.
* **Relational Mapping:** Merged high-frequency sensor logs with operator metadata to correlate human experience levels with machine output.

## Key Business Insights: "The Experience Paradox"
The analysis revealed a counter-intuitive performance trend:
1. **The Mid-Tier Peak:** Mid-level operators consistently outperformed Seniors by ~5-8%, suggesting a "Productivity Sweet Spot" where technical skill is high but administrative burden is low.
2. **The 2026 Senior Collapse:** A significant dip in Senior output was detected in 2026. 
   * **Diagnosis:** Further investigation showed this coincided with a "Junior Staffing Crunch." 
   * **Conclusion:** Senior experts were diverted from optimization tasks to handle basic maintenance, leading to specialist burnout and reduced grid efficiency.



## Featured Visualizations
* **Monthly Energy Trends:** Seasonal fluctuations in EV charging demand.
* **Performance by Experience:** A multi-line comparison showing the divergence between Junior, Mid, and Senior tiers.

## How to Run
1. Clone the repo: `git clone https://github.com/yourusername/ecogrid-optimizer.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Open `ecogrid_optimizer.ipynb` in Jupyter or VS Code.

## Tech Stack
* **Language:** Python 3.11+
* **Libraries:** Pandas (Data Manipulation), NumPy (Numerical Logic), Matplotlib/Seaborn (Visualization)
* **Environment:** Databricks / Jupyter Notebook
