# 📧 AI Email Reply Assistant

An intelligent email assistant that reads incoming emails, analyzes their content, and generates high-quality reply drafts using AI.

---

## 🚀 Overview

This project connects to your email inbox (via Gmail API), extracts email content, and uses AI to generate context-aware replies. Instead of auto-sending messages, it safely saves suggested responses as drafts for you to review.

---

## ✨ Features

* 📥 Read emails from Gmail
* 🧠 Analyze email intent and tone
* ✍️ Generate professional reply drafts using AI
* 📝 Save replies as Gmail drafts (no auto-send)
* 🔒 Secure handling of API keys with environment variables

---

## 🛠️ Tech Stack

* Node.js
* Gmail API
* OpenAI API
* Git & GitHub

---

## 📁 Project Structure

```
email-reply-ai/
├─ README.md
├─ package.json
├─ .env.example
├─ .gitignore
└─ src/
   ├─ index.js
   ├─ gmail.js
   ├─ aiReply.js
   └─ prompts.js
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/YOUR_USERNAME/email-reply-ai.git
cd email-reply-ai
```

---

### 2. Install dependencies

```
npm install
```

---

### 3. Configure environment variables

Create a `.env` file in the root directory:

```
OPENAI_API_KEY=your_openai_api_key
GMAIL_CLIENT_ID=your_client_id
GMAIL_CLIENT_SECRET=your_client_secret
GMAIL_REFRESH_TOKEN=your_refresh_token
```

---

### 4. Run the application

```
node src/index.js
```

---

## 🧠 How It Works

1. Fetch unread or selected emails via Gmail API
2. Extract subject, sender, and body content
3. Send email content to the AI model
4. Generate a suggested reply
5. Save the reply as a draft in Gmail

---

## 📝 Example Prompt

```
You are helping write a professional email reply.

Email:
{{email_body}}

Write a concise and helpful response.
Do not invent information.
If details are missing, ask a clarifying question.
```

---

## 🔐 Security Notes

* Never commit your `.env` file
* Use `.env.example` to share required variables
* Keep API keys private

---

## 📌 Future Improvements

* Web interface for reviewing drafts
* Support for multiple email providers
* Tone customization (formal, friendly, etc.)
* Auto-labeling and prioritization of emails

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

MIT License

---

## ⚠️ Disclaimer

This tool generates AI-based suggestions. Always review responses before sending to ensure accuracy and appropriateness.
