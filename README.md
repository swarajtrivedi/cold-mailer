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

## 🧭 Setup
1) **Place your contacts file**
   - Create a folder named `resources/`
   - Put `contacts.csv` inside it (format shown below)

2) **Add your resume**
   - Create a folder named `attachments/`
   - Put your resume PDF inside it (e.g., `attachments/your_resume.pdf`)

3) **Set environment variables (macOS/Linux – bash/zsh)**
   ```bash
   export SENDER_EMAIL="your_email@gmail.com"
   export EMAIL_APP_PASSWORD="your_gmail_app_password"
   export RESUME_FILENAME="your_resume.pdf"
   ```
   
   - **How to generate a Gmail App Password:**
     1. Go to https://myaccount.google.com/security  
     2. Turn on **2-Step Verification** (if not already)
     3. Under **“Signing in to Google”**, open **App passwords**
     4. Choose **App: Mail**, **Device: Other** (e.g., “AutoMailer”), then **Generate**
     5. Copy the **16-character** password and use it as `EMAIL_APP_PASSWORD` in your `.env`
        
---

## 📄 `contacts.csv` (place in `resources/`)
Required columns (case-sensitive):

| Email | Company | Website |
|------|---------|---------|
| hr@startupx.com | Startup X | https://startupx.com |

Example:
```csv
Email,Company,Website
hr@startupx.com,Startup X,https://startupx.com
careers@aiinc.io,AI Inc,https://aiinc.io
