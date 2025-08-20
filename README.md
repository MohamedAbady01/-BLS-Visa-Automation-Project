# 🛂 BLS Visa Appointment Automation

This project automates the process of booking visa appointments on the **BLS Spain Morocco** website using **Python + Selenium**.  
It also integrates with **Gmail (IMAP)** for OTP verification and provides a **Tkinter GUI** for MySQL data handling.

---

## 🚀 Features
- 🌐 Automated navigation & form filling on BLS website  
- ✅ Handles checkboxes inside iframes  
- 📩 Reads **OTP Confirmation** emails from Gmail (IMAP)  
- 🔑 Automates OTP link submission for login  
- 🗄️ Connects to MySQL to fetch user/passport data  
- 🖥️ Simple Tkinter GUI for database access  

---

## 📂 Project Structure
bls_visa.ipynb # Main Jupyter Notebook
chromedriver.exe # Selenium Chrome WebDriver (update path)
README.md # Documentation


---

## ⚙️ Requirements
Install dependencies:
```bash
pip install selenium mysql-connector-python
```
Additional built-in libraries used:

imaplib

email

tkinter

datetime

time

re
▶️ Usage
1. Configure Chrome & WebDriver

Update in the code:

options.binary_location = "C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe"
driver = webdriver.Chrome(executable_path="C:\\path\\to\\chromedriver.exe")

Mail="yourmail@gmail.com"
Pass="your_app_password"   # Use Gmail App Password
jupyter notebook bls_visa.ipynb
4. Booking Flow

Script opens BLS → navigates to login

Waits for OTP email → extracts confirmation link

Submits OTP automatically

Opens appointment page & selects options (type, members, center, category)

5. Database GUI

The Tkinter app allows:

Entering DB credentials (host, user, password, db)

Fetching records from MySQL

(Extendable for auto form filling from DB)

⚠️ Notes

Gmail requires App Password (not normal password) when using IMAP.

Website structure (XPaths) may change → update locators if needed.

Intended for educational & personal use only.

🔮 Future Improvements

Add undetected-chromedriver to bypass bot detection

Integrate 2Captcha API for solving captchas

Extend MySQL integration for bulk booking automation

Add logging & error handling for better stability

👨‍💻 Author

Developed by Mohamed Abady
⭐ Upwork Freelancer – 100% Job Success | Multiple 5-star projects
