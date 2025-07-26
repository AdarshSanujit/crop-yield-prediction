# 🌾 Crop Yield Prediction Web App

This is a Flask-based web application that predicts crop yield using machine learning. It utilizes a pre-trained Decision Tree Regressor (`dtr.pkl`) along with a data preprocessing pipeline (`preprocessor.pkl`) to provide real-time yield predictions based on agricultural input parameters.

---

## 🚀 Features

- Predicts crop yield based on:
  - Year
  - Average Rainfall (mm/year)
  - Pesticide Usage (tonnes)
  - Average Temperature (°C)
  - Area (Region)
  - Item (Crop)
- User-friendly web interface built with HTML & Flask.
- Integrates `scikit-learn` preprocessor and trained model.

---

## 🛠️ Tech Stack

- **Backend:** Python, Flask
- **Model:** Scikit-learn (`DecisionTreeRegressor`)
- **Preprocessing:** `ColumnTransformer`, Label Encoding/OneHotEncoding
- **Frontend:** HTML (Jinja2 templates)

---

## 📁 Project Structure

```
.
├── app.py                   # Main Flask application
├── dtr.pkl                  # Trained Decision Tree Regressor model
├── preprocessor.pkl         # Preprocessing pipeline
├── templates/
│   └── index.html           # Frontend HTML form
└── README.md
```

---

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/crop-yield-predictor.git
cd crop-yield-predictor
```

### 2. Install dependencies

It is recommended to use a virtual environment:

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

**Sample `requirements.txt`** (add this file):

```
Flask
numpy
scikit-learn
```

### 3. Run the application

```bash
python app.py
```

Visit [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.

---

## 🧠 Model Training (Optional)

The `dtr.pkl` and `preprocessor.pkl` should be created using your dataset with appropriate preprocessing (e.g., label encoding, scaling). If you want help training this model or exporting these files, feel free to ask.

---

## 📸 Screenshots

*(Include screenshots of the input form and output prediction, if available.)*

---

## 🙌 Contribution

Feel free to fork this repository and submit pull requests if you’d like to improve the project!

---

## 📄 License

MIT License – feel free to use, modify, and share.
