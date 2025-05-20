# Prompt_Engineer_Challenge
Test out your ability as an AI prompt engineer in fault monitoring!

# Anomaly Detection Visualization

This project demonstrates how to visualize anomaly detection results from:
- A Linear Regression (LR) model
- A GPT-based Isolation Forest

The notebook highlights:
- Detected anomalies
- The failure alarm time
- Training and test periods

## 📊 Example Output

![example-plot](results_comparison.png)

## 📁 Files

- `Results_GPT_vs_LR-NBM.ipynb`: Interactive version with plots and explanations
- `DS2_data.zip`:
-     DS2_train_data.pkl: 3 month training period of SCADA data
-     DS2_test_data.pkl:  Followed by a ~1 month test period where a Bearing Failure occured
- `results_DS2.csv`: CSV file with anomaly scores, and labels

## ▶️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
