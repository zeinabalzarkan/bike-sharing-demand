
---

## 🎯 Project Goal

The objective is to build a regression model that predicts the number of bike rentals based on:

- Date and time
- Weather data (temperature, humidity, windspeed)
- Holiday and working day information
- Season and hour features

---

## 🛠️ Tools Used

- Python 3.7+
- AutoGluon
- Pandas
- Matplotlib / Seaborn
- Kaggle API

---

## 📊 Model Results

| Model Version        | Description                     | Kaggle RMSE Score |
|----------------------|----------------------------------|-------------------|
| Initial Model        | Raw features only                | -53               |
| + Feature Engineering| Added time-based features        | -30               |
| + HPO                | Hyperparameter optimization      | -35               |

---

## 📈 Visualizations

### Model Training Scores
![Training Score](images/model_train_score.png)

### Kaggle Submission Scores
![Test Score](images/model_test_score.png)

---

## 🚀 Getting Started

To reproduce this project:

```bash
 # Clone this repository
   git clone https://github.com/zeinabalzarkan/bike-sharing-demand.git
   cd bike-sharing-demand

 # (Optional) Create a virtual environment
   python -m venv venv
   source venv/bin/activate  # On Windows use: .\venv\Scripts\activate

 # Install required packages
   pip install -r requirements.txt

 # Run the notebook
   jupyter notebook project.ipynb

---

## 👤 About Me
GitHub: @zeinabalzarkan
Kaggle: @zeinabalzarkan
