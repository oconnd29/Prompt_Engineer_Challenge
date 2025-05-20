# Prompt_Engineer_Challenge
Test out your ability as an AI prompt engineer to implemnt wind turbine fault monitoring!

## Instructions

1. Download the provided `.zip` dataset.
2. Unpack the training and testing sets.
3. Upload the datasets to your chosen AI tool.
4. Ask AI to evaluate turbine health, with or without training context.
5. Inpsect results and present then like - See ExampleResults_GPT_vs_LR-NBM.ipynb

## 📁 Files

- `ExampleResults_GPT_vs_LR-NBM.ipynb`  : Interactive version with plots and explanations
- `DS2_data.zip`                 : Compressed File containing...
- 'DS2_train_data.pkl'           : 3 month training period of SCADA data
- 'DS2_test_data.pkl'            : Followed by a ~1 month test period where a Bearing Failure occured
- `DS2_results.csv`: CSV file with anomaly scores, and labels
  
## Results (draft)
### Basic:
1. Does the AI detect the fault in time with the installed system?
2. Does the AI detect the fault BEFORE the installed system?
3. What AI tool did you use?
4. What method did AI use to detect the fault?
### Technical:
1. Would you, as a technician/engineer trust the results the AI gave you?
2. Would you, as a technician/engineer trust the results shown by the method NBM method? (NBM-based: Model which estimates healthy behaviour, then measure of fault is difference between true and estaimted) 

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


## ▶️ How to Run results example

```bash
pip install -r requirements.txt
jupyter notebook
