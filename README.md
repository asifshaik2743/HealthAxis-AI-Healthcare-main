---
💊 Smart Healthcare Assistant with Sentiment Analysis & Gemini AI

A powerful, full-stack AI-based healthcare assistant that integrates:

- Google Gemini API for AI-powered chatbot and sentiment analysis  
- ReactJS frontend  
- Python Flask backend  
- NodeJS auxiliary server  
- MySQL database powered by XAMPP

This system helps users with disease prediction, medical search, chatbot assistance, and review sentiment analysis — all in one platform.

---

## Project Structure

```

.
├── reactjs/              React frontend
├── backend/              Python backend (Flask + Gemini)
│   ├── app.py            Flask app
│   ├── chat.py           Gemini API integration
│   ├── disped.py         Disease prediction
│   ├── search.py         MySQL connection script
│   └── \*.csv             Medical datasets
├── nodejs/               NodeJS server
│   └── server.js
├── README.md             Project documentation

````

---

## Prerequisites

Make sure the following are installed:

- Node.js and npm
- Python 3.8 or higher
- XAMPP (Apache and MySQL)
- Python dependencies from `requirements.txt`

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/healthcare-assistant.git
cd healthcare-assistant
````

---

### 2. Start the Frontend (ReactJS)

```bash
cd reactjs
npm install
npm start
```

Frontend will run at: [http://localhost:3000](http://localhost:3000)

---

### 3. Set Up the Python Backend

```bash
cd backend
pip install -r requirements.txt
```

**Add your Gemini API key:**

* Get a key from [Google Gemini Studio](https://aistudio.google.com/app)
* Paste it in both `chat.py` and `app.py`

**Run backend scripts in separate terminals:**

```bash
python chat.py
python app.py
python disped.py
```

---

### 4. Configure MySQL with XAMPP

1. Open XAMPP and start **Apache** and **MySQL**
2. Go to phpMyAdmin and create a database named `Healthcare`
3. Run the following:

```bash
python search.py
```

---

### 5. Start the NodeJS Server

```bash
cd nodejs
npm install
node server.js
```

---

## Access the Application

Once everything is running, open:

```
http://localhost:3000
```

You can interact with the AI-powered healthcare assistant, perform searches, and analyze sentiments.

---

## Features

* Disease prediction from symptom input
* ChatBot powered by Google Gemini
* Sentiment analysis on reviews
* Medicine search from MySQL database
* Optional map view of nearby hospitals

---

## Technology Stack

| Component | Technology                 |
| --------- | -------------------------- |
| Frontend  | ReactJS, JavaScript        |
| Backend   | Flask (Python), Gemini API |
| Database  | MySQL (via XAMPP)          |
| Server    | Node.js                    |
| NLP & ML  | spaCy, nltk, scikit-learn  |

---

## Security Tip

Do not expose your Gemini API key in public repos. Use `.env` or secret managers in production.

---

## License

This project is open-source and intended for academic and educational use.

```
