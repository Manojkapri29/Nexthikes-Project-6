# Nexthikes-Project-6
🧪 Sales Forecasting for Rossmann Pharmaceuticals

Welcome to the Sales Forecasting Project for Rossmann Pharmaceuticals!
This project helps predict daily sales for pharmaceutical stores using machine learning and deep learning techniques. We also built web apps to make the predictions easy to use and tracked everything using modern MLOps tools.

---

 📌 What’s This Project About?

Rossmann sells medical products across various stores, and like any retail business, they need to predict how much they’ll sell. Our goal is to help them do just that—using historical data (like past sales, promotions, holidays, etc.) and turning it into smart, data-driven forecasts.

---

 🗂️ What's Inside the Project?

Here's a quick overview of the folders and files you'll find:

```
data/               --> All sales data (raw, processed, external)
notebooks/          --> Jupyter notebooks for each stage: cleaning, modeling, etc.
models/             --> Saved machine learning and deep learning models
src/                --> Python scripts for data, features, models, and deployment
deployment/         --> Flask and Streamlit app code for web deployment
mlruns/             --> MLflow tracking folder
dvc.yaml            --> DVC file for tracking data versions
Dockerfile          --> For running the project in a container
requirements.txt    --> List of Python packages needed
README.md           --> This file!
```

---

🛠️ How to Get Started

 1. Clone the repository:

```bash
git clone https://github.com/<your-username>/rossmann-sales-forecasting.git
cd rossmann-sales-forecasting
```

 2. Set up your Python environment:

```bash
python -m venv venv
source venv/bin/activate   # or venv\\Scripts\\activate on Windows
pip install -r requirements.txt
```

 3. Get the data:

If you're using DVC:

  bash
dvc pull
```

## 🔍 What Did We Do?

### ✅ Data Cleaning & Exploration

* Fixed missing values
* Handled outliers
* Explored trends and patterns in sales

### ✅ Feature Engineering

* Created time-based features like day, week, holiday
* Added lag features (sales from previous days/weeks)
* Marked promotion days

 ✅ Model Building

* **ML Models:** Random Forest, XGBoost
* **DL Models:** LSTM and CNN-LSTM
* All models are evaluated using metrics like RMSE and MAE.

---

 🚀 Web App Deployment

We built two user interfaces:

 1. Flask App (API)

Runs as a backend server to serve predictions.

bash
flask run


 2. Streamlit App (Dashboard)

Nice interactive interface to visualize predictions.

```bash
streamlit run src/deployment/streamlit_app.py
```

---

 📊 MLOps Tools Used

* **MLFlow** – Tracks experiments, parameters, and results.
* DVC – Tracks versions of datasets and models.
* Docker – Package the app and run it anywhere.

 🎯 How to Use

1. Choose your preferred app (Flask for APIs, Streamlit for UI).
2. Launch it using the commands above.
3. Input your store and date information.
4. Get instant sales forecasts.

 📈 Results

We compared different models and found strong performance using XGBoost and LSTM. You can find results and charts in the `reports/` folder or in the Streamlit dashboard.

 🤝 Want to Contribute?

We’d love your help! Feel free to fork the repo, open an issue, or create a pull request.

 📬 Contact

**Project by:** Manoj Kapri 
📧 Email: (kaprimanoj88@gmail.com)

