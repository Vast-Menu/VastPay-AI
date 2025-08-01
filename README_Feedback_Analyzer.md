# Customer Feedback Analyzer with Smart Notifications

## 📌 Overview
This Python script analyzes customer ratings and reviews using OpenAI's GPT intelligence. It detects the customer's sentiment and automatically responds with a smart, empathetic message. It also sends a Telegram alert to the store owner when a low rating is received.

## 🧠 Features
- Detects and analyzes customer sentiment from textual reviews (Arabic/English).
- Sends auto-responses based on customer emotion (apology, improvement promise, etc.).
- Alerts the store owner on Telegram if a rating is negative.
- Uses AI-generated messages to maintain professional tone.

## 🗃️ Data Sources
- Customer star ratings (1–5) and text comments.
- Stored in MySQL database.

## 🧹 Preprocessing
- Text cleaning (punctuation removal, language normalization).
- Filtering out empty reviews or invalid star ratings.
- Language handling (Arabic/English mixed input).

## 🛠️ Tech Stack
- **Language**: Python
- **AI Model**: OpenAI GPT API
- **Database**: MySQL
- **Messaging**: Telegram Bot API
- **Libraries**: `pymysql`, `requests`, `openai`, `python-telegram-bot`

## 🚀 How to Run
1. Install dependencies:
   ```bash
   pip install openai pymysql python-telegram-bot
   ```
2. Configure environment variables or insert your keys directly:
   - OpenAI API Key
   - MySQL credentials
   - Telegram Bot Token & Chat ID
3. Run the script:
   ```bash
   python feedback_analyzer.py
   ```

## 📈 Output
- AI-generated customer response
- Telegram alert to store owner