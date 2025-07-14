# 📬 AI-Powered Email Automation Tool

This Python project automates the process of sending **personalized job outreach emails** using the **OpenAI GPT-4 API**. It reads company contact info from a CSV file, generates tailored emails based on each company’s website, attaches your resume, and sends the email through Gmail. It also prevents duplicate emails and includes randomized delays to avoid spam filters or rate limits.

---

## 🚀 Features

- 🤖 Auto-generates customized emails for each company using GPT-4
- 📎 Attaches your resume to every outgoing email
- 🧠 Caches GPT results in a backup file to avoid redundant API calls
- ✅ Prevents duplicate emails with persistent email tracking
- ⏱️ Adds random wait time (2–5 mins) between sends to stay under Gmail limits
- 🔌 Modular structure for better maintainability

---

## ⚙️ Setup Instructions

### 1. 🔐 Add a `.env` File

Create a `.env` file in the project root directory with the following variables:

OPENAI_API_KEY=your_openai_api_key
SENDER_EMAIL=your_email@gmail.com
EMAIL_APP_PASSWORD=your_gmail_app_password
RESUME_FILENAME=Swaraj_Resume.pdf

Alternatively, you can set the env vars from the CLI.

### 2. Installing Deps

pip install openai python-dotenv pandas

### 3. File structure 

Create a resources and an attachments folder.
Put the contacts.csv file in the resources folder.
The structure of the contacts.csv file => Email, Company, Website are the mandatory fields.
Put the resume to be attached in the attachments folder.

## Run the script

To run the script do: python mail_script.py or simply run the mail_script.py file.

Happy mailing!


