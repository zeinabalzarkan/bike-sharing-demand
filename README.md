🚴‍♀️ Bike Sharing Demand – Kaggle Competition
By Zeinab Alzarkan
This repository contains a complete solution to the Bike Sharing Demand Kaggle competition. The goal is to predict the number of bike rentals using historical weather and seasonal data. AutoGluon is used to automate training, feature engineering, and hyperparameter optimization.

📁 Project Structure
bash
Copy
Edit
bike-sharing-demand/
├── project.ipynb                  # Main notebook with full AutoGluon workflow
├── submission.csv                 # Initial Kaggle submission
├── submission_new_features.csv   # Submission after feature engineering
├── submission_new_hpo.csv        # Submission after hyperparameter tuning
├── images/                        # Visualizations (model scores, charts)
│   ├── model_train_score.png
│   └── model_test_score.png
├── report.md                      # Final project report
├── README.md                      # This file
🎯 Objective
Predict daily bike rental counts based on:

Date & time (seasonality)

Weather conditions (temperature, humidity, windspeed)

Holiday and working day information

This project follows an iterative ML process using AutoGluon's TabularPredictor to:

Train baseline models

Improve performance with feature engineering

Optimize results through hyperparameter tuning

🛠️ Tools and Libraries
Python 3.7+

AutoGluon

Pandas

Matplotlib / Seaborn

Kaggle API

📊 Results
Model Version	Description	Kaggle RMSE Score
Initial Model	Raw features only	0.70
+ Feature Engineering	Added hour, day, weekday, etc.	0.78
+ HPO	Tuned hyperparameters	0.80

📉 Visualizations
🔧 Model Training Score Progress
<img src="images/model_train_score.png" width="600"/>
🧪 Kaggle Submission Score Progress
<img src="images/model_test_score.png" width="600"/>
🚀 How to Reproduce
Clone the repository:

bash
Copy
Edit
git clone https://github.com/zeinabalzarkan/bike-sharing-demand.git
cd bike-sharing-demand
(Optional) Setup a virtual environment:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt
Run the notebook project.ipynb in Jupyter or SageMaker Studio.

Submit predictions to Kaggle using:

bash
Copy
Edit
kaggle competitions submit -c bike-sharing-demand -f submission.csv -m "Your message"
👤 Author
Zeinab Alzarkan

GitHub: @zeinabalzarkan

Kaggle: @zeinabalzarkan

📄 License
This project is licensed under the MIT License.
