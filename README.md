# 🔐 Secure Login System

A full-stack secure web login system built with **Flask** featuring bcrypt password hashing, SQL injection protection, session management, and optional TOTP-based Two-Factor Authentication.

---

## 🛡️ Security Features

| Feature | Implementation |
|---|---|
| Password Hashing | bcrypt with cost factor 12 |
| SQL Injection Protection | Parameterized queries (SQLite) |
| Session Management | Flask sessions with 30-min timeout, HttpOnly cookies |
| Brute-force Protection | 5 attempts → 5-minute IP lockout |
| Input Validation | Regex: username, email, password strength |
| 2FA (Optional) | TOTP via pyotp — Google Authenticator / Authy compatible |
| Login Audit Log | Every login attempt logged with IP and timestamp |

---

## 📁 Project Structure

---

## ▶️ How to Run

**1. Install dependencies**
```bash
pip install -r requirements.txt
```

**2. Start the server**
```bash
python app.py
```

**3. Open in browser**

---

## 🔑 Password Requirements

- Minimum 8 characters
- At least one uppercase letter
- At least one number
- At least one special character

---

## 📱 2FA Setup (Optional)

1. Register and log in
2. Go to Dashboard → Enable 2FA
3. Scan the QR code with Google Authenticator or Authy
4. Enter the 6-digit code to activate
5. Future logins will require the code after password

---

## 📦 Dependencies

- Python 3.8+
- Flask
- bcrypt
- pyotp
- qrcode
- Pillow

---

## 👤 Author

Built as part of a Web Security project submission.
