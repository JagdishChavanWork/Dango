# 🚀 Django + AI Project (Local Conda Environment – Python 3.12)

This project is set up for **production-grade AI software development using Django and Python 3.12**.  
It uses a **project-level Conda environment (Anaconda)** to ensure dependency isolation, compatibility, and smooth deployment.

All tools, libraries, and versions used here are **mutually compatible** and aligned with industry standards.

---

## 📌 Prerequisites
- **Anaconda (latest version)**
- Git
- Windows OS
- Command Prompt (CMD)

> ⚠️ Python is managed **only via Conda (Anaconda)**  
> Do NOT use system Python or virtualenv.

---

## 📂 Project Structure
```
django_ai_product/
│
├── env/                # Local Conda environment (DO NOT COMMIT)
├── config/             # Django project settings
├── manage.py
├── requirements.txt
├── .env                # Environment variables (ignored by git)
└── README.md
```

---

## 🧱 Step 1: Create Project Directory
```cmd
mkdir django_ai_product
cd django_ai_product
```

---

## 🧪 Step 2: Create Local Conda Environment (Python 3.12)
```cmd
conda create --prefix .\env python=3.12 -y
```

---

## ▶️ Step 3: Activate the Environment (CMD)
```cmd
conda activate .\env
```

Verify:
```cmd
python --version
```

---

## 🔧 Step 4: Upgrade Core Packaging Tools
```cmd
pip install --upgrade pip setuptools wheel
```

---

## 🌐 Step 5: Install Django
```cmd
pip install "django>=5.0,<6.0"
```

---

## 🔌 Step 6: Install Backend & API Stack
```cmd
pip install djangorestframework python-dotenv django-cors-headers gunicorn whitenoise
```

---

## 🧠 Step 7: Install AI / Data Stack
```cmd
pip install numpy pandas scikit-learn
```

---

## 🏗️ Step 8: Create Django Project
```cmd
django-admin startproject config .
```

Run server:
```cmd
python manage.py runserver
```

---

## 📦 Step 9: Freeze Dependencies
```cmd
pip freeze > requirements.txt
```

---

## 🔐 Step 10: Environment Variables
Create `.env` file:
```
SECRET_KEY=your-secret-key
DEBUG=True
```

---

## 🗃️ Step 11: Git Setup
```cmd
git init
```

`.gitignore`
```
env/
.env
__pycache__/
*.pyc
```

---

## 🎯 Purpose
Build deployable AI-backed Django applications ready for production, Docker, and cloud.

