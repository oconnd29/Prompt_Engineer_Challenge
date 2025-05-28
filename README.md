# Prompt_Engineer_Challenge
Test out your ability as an AI prompt engineer to implement wind turbine fault monitoring!

Using an example from a real wind turbine, where a failure of generator bearing occured, can we detect the damage before the instaleld system?

## Instructions

1. Download the training and test `.zip` files. 
2. Unpack the training and testing sets.
3. Upload the datasets to your chosen ChatBot.
4. Ask the AI to evaluate turbine health, with or without training context. 
5. Inpsect results and present then like - See ExampleResults_GPT_vs_LR-NBM.ipynb


Example Prompt:
'Using the training data, learn to detect the failure alarm that occurs during the test data. plot the test data detections.'

## 📁 Files

- `Visualise_Results_GPT_vs_LR-NBM.ipynb`  
  An interactive Jupyter notebook comparing anomaly detection results using GPT-based methods vs. Linear Regression based Normal Behavior Model (LR-NBM). Includes results, plots. 

- `DS2_data.zip`  
  Compressed archive containing sensor and alarm data from Dataset DS2, structured for training and testing a failure prediction model.*

  **Contents:**
  - `DS2_train_data.pkl`  
    SCADA sensor data and corresponding alarm events for a ~3-month training and validation period.  
    KEYS: 'train_sensor_data' and 'train_alarm_data'
  - `DS2_test_data.pkl`  
    SCADA sensor data and corresponding alarm events for a ~1-month test period during which a bearing failure occurred.  
    KEYS: 'test_sensor_data', 'test_alarm_data' and 'failure_alarm'

- `DS2_results.csv`  
  CSV file containing anomaly scores and ground-truth labels for the test period, used to evaluate model performance.*

  
## Feedback - Email me! oconnd29@tcd.ie
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
- An LR-NBM model
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
