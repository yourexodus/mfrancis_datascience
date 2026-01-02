# 🚲 Data Modeling: Supervised Learning
## Project: Capital Bikeshare Demand Forecasting

### The Problem & Objective
The objective is to **predict the total ridership** of Capital Bikeshare in any given hour. By accurately forecasting demand, we can create analytical tools to:
* Optimize **infrastructure planning** (where to build stations).
* Automate **maintenance scheduling** based on expected wear and tear.
* Ensure **bike availability** through proactive system rebalancing.



[Image of a supervised learning process diagram]


---

### Core Q&A
**What are we predicting?** The `total_rentals` (count) per hour.

**What are the key drivers (Features)?** Weather conditions, temperature, humidity, and whether it is a working day or holiday.

**What does one row represent?** One specific hour of one day.

**Is the data clean?** Yes. I renamed the target variable to `total_rentals` to avoid coding conflicts and ensured the `datetime` index was properly formatted for time-series analysis.

---

### The Results



* **Temperature Impact:** For every **1°C increase** in temperature, the model shows an average increase of **9.17 rentals**.
* **Baseline Demand:** Even at **0°C**, the model predicts a baseline of approximately **6 rentals** per hour.

---
###
Requirements
pandas
numpy
seaborn
matplotlib
scikit-learn
scipy
statsmodels

### Technical Implementation
* **Algorithm:** Linear Regression (Supervised Learning)
* **Tools:** Python, Scikit-Learn, Pandas
* **Evaluation:** Coefficients ($\beta_1$) and Intercepts ($\beta_0$) were validated against real-world logic.