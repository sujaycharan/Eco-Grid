# ⚡ Eco-Grid – Smart Energy Management & Prediction System

Eco-Grid is an AI-powered web platform designed to promote sustainable energy usage through intelligent predictions, user insights, and real-time communication.  
It combines **Flask**, **MongoDB**, and **Machine Learning (XGBoost)** to help users monitor, manage, and optimize electricity consumption efficiently.

---

## 🚀 Features

- 🔐 **User Authentication** – Secure login and registration using hashed passwords.  
- 📊 **Electricity Consumption Prediction** – Predicts power usage patterns using an XGBoost model.  
- 💬 **Twilio SMS Integration** – Sends instant alerts or updates to users’ registered phone numbers.  
- 🧾 **QR Code Generation** – Generates unique QR codes for user verification or quick access.  
- 💾 **MongoDB Database** – Efficient NoSQL storage for user and consumption data.  
- 🌐 **CORS Enabled API** – Seamless integration with any frontend client (React, Angular, etc.).  
- 🧠 **AI-Driven Insights** – Built using an ML model trained on electricity usage data.

---

## 🧰 Tech Stack

| Category | Technologies Used |
|-----------|-------------------|
| **Frontend** | (Can be integrated with React.js / HTML / JS) |
| **Backend** | Flask (Python) |
| **Database** | MongoDB |
| **ML Model** | XGBoost, Scikit-learn, Pandas |
| **Other Tools** | Twilio API, QRCode, Flask-CORS, Werkzeug Security |

---

## 📂 Project Structure

```
Eco-Grid/
│
├── app.py                         # Main Flask application
├── xgboost_electricity_model.pkl  # Pre-trained ML model
├── requirements.txt               # Python dependencies
├── README.md                      # Project documentation
├── .gitignore
└── templates/ or static/ (optional for UI)
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Eco-Grid.git
cd Eco-Grid
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables  
Create a `.env` file or edit directly in `app.py`:
```
TWILIO_ACCOUNT_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_token
TWILIO_PHONE_NUMBER=your_twilio_phone
MONGO_URI=mongodb://127.0.0.1:27017/
SECRET_KEY=your_secret_key
```

### 5. Run the application
```bash
python app.py
```

Your app will run on:  
👉 http://127.0.0.1:5000/

---

## 🧠 Machine Learning Model

The `xgboost_electricity_model.pkl` file is a pre-trained **XGBoost regression model** used to predict electricity usage patterns.  
You can replace it with your own trained model using the following libraries:
```python
import xgboost as xgb
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error
```

---

## 🚀 Future Enhancements

- Add interactive frontend using **React.js**
- Integrate **real-time IoT meter data**
- Include **carbon footprint tracking**
- Add **email notifications** and **usage analytics dashboard**

---

## 👨‍💻 Author

**Sujay Charan**  
📧 [sujaycharanlearning2005@gmail.com]  
💼 [https://www.linkedin.com/in/sujay-charan/]  

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---


