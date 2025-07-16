---

# 💊 Smart Healthcare Assistant with Sentiment Analysis & Gemini AI

A powerful, full-stack AI-based healthcare assistant that integrates:

* 🔮 **Google Gemini API** for AI-powered chatbot & sentiment analysis
* 💻 **ReactJS** frontend
* 🧠 **Python Flask** backend
* ⚙️ **NodeJS** auxiliary server
* 🛢️ **MySQL** database powered by **XAMPP**

This system helps users with disease prediction, medical search, chatbot assistance, and review sentiment analysis — all in one platform.

---

## 📁 Project Structure

```
.
├── reactjs/              # React frontend
├── backend/              # Python backend (Flask + Gemini)
│   ├── app.py            # Flask app
│   ├── chat.py           # Gemini API integration
│   ├── disped.py         # Disease prediction
│   ├── search.py         # MySQL connection script
│   └── data.csv             # Medical datasets
├── nodejs/               # NodeJS server
│   └── server.js
├── README.md             # Project documentation
```

---

## ✅ Prerequisites

Install the following before running the project:

* [Node.js & npm](https://nodejs.org/)
* [Python 3.8+](https://www.python.org/)
* [XAMPP](https://www.apachefriends.org/index.html) (for Apache & MySQL)
* Python packages listed in `requirements.txt`

---

## ⚙️ Step-by-Step Setup Instructions

### 🔹 1. Clone the Repository

```bash
git clone https://github.com/your-username/healthcare-assistant.git
cd healthcare-assistant
```

---

### 🔹 2. Start the Frontend (ReactJS)

```bash
cd reactjs
npm install       # First-time setup
npm start         # Runs on http://localhost:3000
```

---

### 🔹 3. Set Up the Python Backend

```bash
cd backend
pip install -r requirements.txt
```

#### 🔑 Google Gemini API Key

* Get your API key from [Google Gemini Studio](https://aistudio.google.com/app).
* Paste your key into `chat.py` and `app.py`.

#### ▶️ Run Backend Services (in separate terminals):

```bash
python chat.py
python app.py
python disped.py
```

---

### 🔹 4. Configure MySQL with XAMPP

1. Open **XAMPP**.
2. Start **Apache** and **MySQL**.
3. Open **phpMyAdmin** and create a database named:

```
Healthcare
```

4. Run:

```bash
python search.py
```

This connects your backend to the MySQL database.

---

### 🔹 5. Start the NodeJS Server

```bash
cd nodejs
npm install   # If needed
node server.js
```

---

## 🌐 Access the Application

Once all components are running, go to:

```
http://localhost:3000
```

You'll be able to interact with the healthcare assistant, use the chatbot, and search for diseases and medicines.

---

## 💡 Features

* 🔍 **Disease Prediction** using symptom-based logic
* 🧠 **ChatBot** powered by Google Gemini
* 💊 **Medical Search** via database connection
* 😊 **Sentiment Analysis** on medical reviews
* 📍 **Map View** of hospitals (optional JSON data)

---

## 📦 Technologies Used

| Component    | Tech Stack                |
| ------------ | ------------------------- |
| Frontend     | ReactJS, CSS, JavaScript  |
| Backend      | Python, Flask, Gemini API |
| Database     | MySQL, XAMPP              |
| Extra Server | Node.js                   |
| ML/NLP       | nltk, scikit-learn, spaCy |

---

## 🔐 Security Note

⚠️ **Never share your Gemini API key publicly.**
Use environment variables or a `.env` file in production.

---

## 📚 License

This project is for academic and educational purposes only.
Feel free to fork, customize, and extend it.

---
