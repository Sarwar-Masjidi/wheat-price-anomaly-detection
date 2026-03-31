
## 📌 Project Overview

During my final year of university, I developed this project as part of my thesis.  
I used an **8,000-row dataset** of daily wheat prices in Central Asia to build an anomaly detection system.

Key points:

- **Raw price detection**: F1 score ~0.25 using Isolation Forest.  
- **Seasonally adjusted detection**: F1 score improved to ~0.85 using rolling median to handle seasonal harvest cycles.  
- **Visualization**: Price trends, rolling median, and detected anomalies are visualized in the Jupyter notebook.  

This project highlights the importance of **understanding the context behind the data**, not just the algorithm.

---

## 📂 Repository Structure


wheat-price-anomaly-detection/
├─ data/ # Contains the wheat_prices.csv dataset (8,000 rows)
├─ notebooks/ # Jupyter notebooks demonstrating analysis
│ └─ 01_baseline_model.ipynb
├─ src/ # Python scripts (currently empty, contains init.py)
├─ results/ # Model outputs, plots, and analysis (currently placeholder.txt)
├─ README.md # Project description
├─ requirements.txt # Python dependencies


---

## 📝 Dataset

- **File:** `data/wheat_prices.csv`  
- **Columns:**  
  - `date`: Date of the wheat price  
  - `price`: Daily wheat price (Central Asia)  

- **Rows:** 8,000  

---

## 🧪 Key Features

- **Rolling median filter**: Handles seasonal effects and smooths the series.  
- **Residual calculation**: Difference between actual price and rolling median.  
- **Isolation Forest**: Detect anomalies in raw and seasonally adjusted data.  
- **Evaluation**: F1-score comparison to highlight improvement with seasonal adjustment.  
- **Visualization**: Plots of raw prices, rolling median, true anomalies, and model predictions.  

---

## 📈 How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt
Open the notebook:
jupyter notebook notebooks/01_baseline_model.ipynb
Explore:
Rolling median smoothing
Residual calculation
Isolation Forest anomaly detection
Visualization of true vs detected anomalies
⚡ Results
Baseline (raw prices): F1 score ~0.25
With seasonal adjustment: F1 score ~0.85
Visualizations show how seasonal adjustment improves anomaly detection.
💻 Future Work
Add more sophisticated models (e.g., LSTM or Prophet) for anomaly prediction.
Automate report generation in results/.
Add scripts in src/ to reproduce notebook analysis programmatically.
🔗 References
Scikit-learn Isolation Forest
Pandas rolling median documentation
Matplotlib documentation

---

This README is **professional, descriptive, and SOP-friendly**.  

It highlights:  

- Your **project story**  
- **Data & methodology**  
- **Results & improvements**  
- **Folder structure** (so reviewers see it’s organized)  
- **Future directions**  
