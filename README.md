# 🏠 Bangalore House Price Prediction

This data science project series walks through the **step-by-step process** of how to build a real estate price prediction website.

---

## 📌 Project Overview
We aim to predict house prices in Bangalore using various machine learning techniques. The project is divided into three main parts:

1. **Model Building**  
   - Using **sklearn** and **linear regression** on the Bangalore home prices dataset from [Kaggle](https://www.kaggle.com/).  
   - Covers data cleaning, feature engineering, dimensionality reduction, and hyperparameter tuning.
   
2. **Flask Server**  
   - A **Python Flask server** serves HTTP requests using the saved ML model.
   
3. **Frontend Website**  
   - Built with **HTML, CSS, and JavaScript**.  
   - Allows users to enter details like square footage, number of bedrooms, etc.  
   - Calls the Flask server to retrieve predicted price.

---

## 🚀 Technologies & Tools

- Python
- Numpy & Pandas → Data cleaning & preprocessing
- Matplotlib → Data visualization
- Scikit-learn (sklearn) → Model building & evaluation
- Jupyter Notebook → For experimentation
- PyCharm / VS Code → Development IDE
- Flask → Backend server
- HTML, CSS, JavaScript → Frontend UI
- Nginx → Web server

---

## 📂 Project Structure
```bash
BHP/
│── client/                # Frontend (HTML, CSS, JS)
│── model/                 # Trained ML model files
│── server/                # Flask backend (server.py)
│── bhp.pem / bhp.ppk      # Keys (if using cloud deployment)
│── README.md              # Project documentation
````

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Chilliflex/Bangalore-House-Price-Prediction.git
cd Bangalore-House-Price-Prediction
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate   # On Windows
source venv/bin/activate  # On Linux/Mac
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run Flask Server

```bash
cd server
python server.py
```

Server will start at 👉 `http://127.0.0.1:5000`

### 5️⃣ Run Frontend

* Open `client/index.html` in a browser.
* Enter details (square feet, BHK, etc.), and the site will display predicted prices.

---

## 🔧 Running with Nginx

1. Install **Nginx** on your machine.
2. Replace the `nginx.conf` file inside `nginx/conf/` with the provided config.
3. Run `nginx.exe`.
4. Start Flask server with PyCharm:

   ```bash
   python server.py
   ```
5. Access the website via browser.

---

## 📊 Concepts Covered

This project demonstrates many important data science concepts:

* Data loading & cleaning
* Outlier detection & removal
* Feature engineering
* Dimensionality reduction
* GridSearchCV for hyperparameter tuning
* K-Fold cross-validation
* Model deployment with Flask & Nginx

---

## ✨ Demo Flow

1. User enters inputs in web UI.
2. Frontend sends request to Flask backend.
3. Flask backend loads trained ML model.
4. Model predicts house price and returns result.
5. UI displays the predicted price.

---

```


