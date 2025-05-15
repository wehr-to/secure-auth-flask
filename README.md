# Secure Flask Authentication System 

This project is a **hardened user authentication system** built with Flask, focused on teaching and implementing real-world web security best practices. It was created as part of a personal app hardening initiative to go beyond “it works” and dive into **how to secure a web app properly**.

---

## 🚀 Features

- User registration & login
- Bcrypt password hashing (no plaintext storage)
- CSRF protection with Flask-WTF
- Session management with login tracking
- Session timeout logic
- Mock 2FA integration (via TOTP)
- .env-based secret management
- Routes protected with `@login_required`
- Realistic vulnerabilities (XSS, CSRF, IDOR) identified, injected, and mitigated

---

## Project Structure


---

## Getting Started

These steps will get the app running locally on your machine.

```bash
# 1. Clone the Repository
git clone https://github.com/yourusername/secure-flask-auth.git
cd secure-flask-auth

# 2. Create and Activate the Virtual Environment

# On macOS/Linux:
python3 -m venv venv
source venv/bin/activate

# On Windows:
python -m venv venv
venv\Scripts\activate

# 3. Install Dependencies
pip install -r requirements.txt

# 4. Set Up Environment Variables
cp .env.example .env

# Then open the .env file and set:
SECRET_KEY=your-secure-key-here

# 5. Initialize the Database
python

# Inside the Python shell, run:
from app import db
db.create_all()
exit()

# 6. Run the Application
flask run

# Visit in browser:
http://127.0.0.1:5000







