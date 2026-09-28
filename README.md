### `requirements.txt`

```txt
numpy
pandas
scikit-learn
xgboost
streamlit
joblib
feature-engine
```

### `README.md`

````markdown
# ✈️ Flight Price Prediction

A machine learning web application built with **Python, Streamlit, Scikit-learn, XGBoost, Pandas, NumPy, and Feature-engine** to predict flight ticket prices.

The application provides an interactive interface where users enter airline, journey date, source, destination, departure time, arrival time, duration, number of stops, and additional information. The trained XGBoost model predicts the estimated flight price in INR.

## 🚀 Features

- Interactive Streamlit web interface
- Flight price prediction in INR
- XGBoost regression model
- Random Forest based feature selection
- Scikit-learn preprocessing pipelines
- Missing-value handling
- Rare-category encoding
- One-hot and mean encoding
- Date and time feature extraction
- Flight-duration feature engineering
- Outlier handling using Winsorization
- Feature scaling and transformation
- Joblib preprocessing pipeline
- Pickle-based XGBoost model

## 🧠 Input Features

| Feature | Description |
|---|---|
| Airline | Airline operating the flight |
| Date of Journey | Date of journey |
| Source | Departure city |
| Destination | Arrival city |
| Departure Time | Flight departure time |
| Arrival Time | Flight arrival time |
| Duration | Flight duration in minutes |
| Total Stops | Number of stops |
| Additional Info | Additional flight information |

## 🔧 Machine Learning Pipeline

The project performs the following preprocessing:

1. Missing-value imputation
2. Rare-label encoding
3. One-hot encoding
4. Mean encoding
5. Date feature extraction
6. Time feature extraction
7. Part-of-day feature engineering
8. Flight-duration categorization
9. RBF similarity features
10. Outlier treatment using Winsorization
11. Power transformation
12. Feature scaling
13. Feature selection
14. XGBoost regression prediction

## 📁 Project Structure

```text
Flight-prices-prediction/
│
├── app.py
├── train.csv
├── preprocessor.joblib
├── xgboost-model
├── requirements.txt
└── README.md
````

## 💻 Requirements

* Python 3.9 or newer
* pip
* Streamlit
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Feature-engine
* Joblib

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Flight-prices-prediction.git
```

### 2. Open the project directory

```bash
cd Flight-prices-prediction
```

### 3. Create a virtual environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

## ▶️ Run the Streamlit Application

Run the following command:

```bash
streamlit run app.py
```

Streamlit will normally open the application at:

```text
http://localhost:8501
```

If it does not open automatically, copy the URL from the terminal and open it in your browser.

## 🧪 How to Use

1. Select the **Airline**.
2. Select the **Date of Journey**.
3. Select the **Source** city.
4. Select the **Destination** city.
5. Select the **Departure Time**.
6. Select the **Arrival Time**.
7. Enter the **Duration** in minutes.
8. Enter the **Total Stops**.
9. Select **Additional Info**.
10. Click **Predict**.
11. The estimated flight price will be displayed in INR.

## 📦 Install Dependencies Manually

If you do not want to use `requirements.txt`, install the packages with:

```bash
pip install numpy pandas scikit-learn xgboost streamlit joblib feature-engine
```

## 🛠️ Technologies Used

* **Python**
* **Streamlit**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **XGBoost**
* **Feature-engine**
* **Joblib**
* **Pickle**

## 📊 Prediction

The application displays the predicted price in Indian Rupees:

```text
The predicted price is XXXXX INR
```

## ⚠️ Important Notes

The application expects the following files:

```text
train.csv
preprocessor.joblib
xgboost-model
```

`app.py` reads `train.csv` during startup and loads the preprocessing pipeline and trained XGBoost model for prediction.

Keep these files in the same project directory unless you modify the paths in `app.py`.

## 🐛 Troubleshooting

### Streamlit command not found

Try:

```bash
python -m streamlit run app.py
```

### Missing module error

Install the required packages:

```bash
pip install -r requirements.txt
```

### XGBoost or model loading error

Make sure the installed XGBoost version is compatible with the version used to train and save the model.

### Port already in use

Run Streamlit on another port:

```bash
streamlit run app.py --server.port 8502
```

## 👨‍💻 Author

Developed as a machine learning project for flight price prediction using an interactive Streamlit application.

## 📄 License

You can add your preferred open-source license, such as the MIT License.

---

⭐ If you find this project useful, consider giving the repository a star!


