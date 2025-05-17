# 🚗 Car Price Prediction Web App

This is a machine learning-based web application that predicts the selling price of a car based on various features such as manufacturing year, showroom price, kilometers driven, fuel type, and more. The app uses a Random Forest Regression model to make predictions.



## 🔧 Project Structure

```
car-price-prediction/
│
├── app.py                        # Flask backend application
├── index.html                   # Frontend template (in 'templates' folder)
├── random_forest_regression_model.pkl  # Trained ML model
├── requirements.txt             # Python dependencies
├── car data (1).csv             # Dataset used for training
├── templates/
│   └── index.html               # Main HTML page
└── static/
    └── images/
        └── downlaod.jpeg        # Background image used in UI
```

---

## 📌 Features

- Predicts the **resale value** of used cars.
- Built using **Flask**, a lightweight Python web framework.
- Beautiful and responsive frontend using HTML + CSS.
- Uses a **Random Forest Regression** model trained on real-world data.
- Input features:
  - Year of Purchase
  - Showroom Price (in Lakhs)
  - Kilometers Driven
  - Number of Previous Owners
  - Fuel Type (Petrol / Diesel / CNG)
  - Seller Type (Dealer / Individual)
  - Transmission Type (Manual / Automatic)

---

## 🧠 Machine Learning Model

- **Algorithm**: Random Forest Regressor
- **Preprocessing**: Log transformation on kilometers driven
- **Training Data**: Taken from `car data (1).csv`
- **Saved Model**: `random_forest_regression_model.pkl`

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/car-price-prediction.git
cd car-price-prediction
```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Flask App

```bash
python app.py
```

The application will be available at: `http://127.0.0.1:5000/`

---

## 🖥️ UI Preview

The user interface is clean and intuitive, with fields for each input variable and a **predict** button. Results are displayed dynamically.

![App Preview](static/images/downlaod.jpeg)

---

## 📂 Data Sample

The dataset (`car data (1).csv`) includes fields like:

- `Year`
- `Selling_Price`
- `Present_Price`
- `Kms_Driven`
- `Fuel_Type`
- `Seller_Type`
- `Transmission`
- `Owner`

---

## ✍️ Author

**Shreyas Sangalad**  

---

## 📃 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 💡 Future Enhancements

- Add model comparison (Linear Regression, XGBoost, etc.)
- Store predictions in a database
- Deploy the app on Heroku or Render
- Add user authentication and history tracking
