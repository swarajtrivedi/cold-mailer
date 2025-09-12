# ✉️ AutoMailer AI – Cold Email Outreach, Supercharged by GPT-4

Tired of writing cold emails manually while job hunting?  
**AutoMailer AI** is your personal assistant that **writes and sends personalized emails** to recruiters and companies — while you focus on the rest of your job search.

Built to help job seekers like me scale outreach without sacrificing quality. Just give it a contact list, and let it do the magic.

---

## 🚀 Features

✅ Takes a `.csv` file of companies and their websites  
✅ Uses **GPT-4** to generate **tailored email drafts**  
✅ Sends emails through **Gmail** with your **resume attached**  
✅ Adds **random delays (10–15 mins)** between sends to avoid flags  
✅ **Avoids duplicates** by tracking previously sent emails  
✅ **Backs up GPT responses** so nothing is lost on failure  
✅ Easy to plug in your own contacts, resume, and tweaks

---

## 📦 Folder Setup

Make sure your project root contains:

- `resources/contacts.csv` → Your list of companies (see format below)
- `attachments/your_resume.pdf` → Your resume file

---

## 🧾 contacts.csv Format

Your `contacts.csv` inside the `resources/` folder **must contain** the following columns:

| Column    | Description                             |
|-----------|-----------------------------------------|
| Email     | Email address of the company contact     |
| Company   | Name of the company                      |
| Website   | Official company website (used for GPT)  |

Example:

```csv
Email,Company,Website
hr@startupx.com,Startup X,https://startupx.com
careers@aiinc.io,AI Inc,https://aiinc.io
