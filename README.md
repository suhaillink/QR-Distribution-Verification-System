<div align="center">

# 📱 QR Distribution Verification System

### Prevent duplicate distribution • Verify instantly • Manage beneficiaries in real-time


![GitHub stars](https://img.shields.io/github/stars/YOUR_USERNAME/YOUR_REPO?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/YOUR_USERNAME/YOUR_REPO?style=for-the-badge)
![License](https://img.shields.io/github/license/YOUR_USERNAME/YOUR_REPO?style=for-the-badge)
![Firebase](https://img.shields.io/badge/Firebase-Firestore-orange?style=for-the-badge\&logo=firebase)

</div>

---

## 🧠 Overview

The **QR Distribution Verification System** is a mobile-friendly web application that allows organizers to register and verify beneficiaries using QR codes.

It eliminates manual registers, token slips, and confusion during public distribution programs.

A simple smartphone becomes a **real-time verification device**.

---

## ❗ The Problem

Distribution programs often rely on manual tracking.

This creates serious issues:

* 🧾 Paper lists get messy
* 🔁 Same person collects multiple times
* 😠 Arguments at the counter
* 🧍 Genuine people miss their turn
* ⏱ Slow queues

We needed a solution that was:

* simple
* fast
* usable by volunteers
* fair

---

## 💡 The Idea

Every card already contains a QR code.

So instead of giving people tokens…

➡ Use the QR as a **unique digital identity**.

Scan once → register
Scan again → verify
Give item → mark collected

No duplicates. No confusion.

---

## ⚙️ How It Works

```
Scan QR → Check database → Eligible → Give item → Mark collected
```

| Action        | Result                        |
| ------------- | ----------------------------- |
| First scan    | Registers beneficiary         |
| Second scan   | Checks eligibility            |
| After marking | Prevents duplicate collection |

---

## ✨ Features

* 📷 QR code scanning
* ☁ Cloud database
* 🚫 Duplicate prevention
* 🕒 Date & time tracking
* 👨‍💼 Admin dashboard
* 📱 Mobile-only operation
* 🌐 Works from any location
* 👥 Multiple volunteers supported

---

## 🖥 Admin Dashboard

The admin panel displays:

* all registered QR IDs
* collection status
* timestamps
* duplicate detection

✔ = Collected
❌ = Not collected

---

## 🧰 Tech Stack

| Technology         | Purpose        |
| ------------------ | -------------- |
| HTML / CSS / JS    | Frontend       |
| Firebase Hosting   | Deployment     |
| Firebase Firestore | Database       |
| html5-qrcode       | Scanner engine |

---

## 🚀 Installation Guide

### 1️⃣ Create Firebase Project

Go to:

https://console.firebase.google.com

Create a new project.

---

### 2️⃣ Enable Database

```
Build → Firestore Database → Create Database → Test Mode
```

---

### 3️⃣ Enable Hosting

```
Build → Hosting → Get Started
```

---

### 4️⃣ Install Tools

Install NodeJS first:

https://nodejs.org

Then install Firebase CLI:

```
npm install -g firebase-tools
firebase login
```

---

### 5️⃣ Clone Repository

```
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

---

### 6️⃣ Initialize Firebase

```
firebase init
```

Select:

* Firestore
* Hosting

Public directory:

```
public
```

Single Page App → YES

---

### 7️⃣ Add Your Firebase Config

Go to:

Firebase Console → Project Settings → Web App → SDK configuration

Copy:

```
const firebaseConfig = { ... }
```

Open:

```
public/index.html
```

Replace the existing firebaseConfig with yours.

---

### 8️⃣ Deploy

```
firebase deploy
```

You will receive:

```
https://your-project.web.app
```

Open on phone → start scanning 🎉

---

## 🔐 Admin Login

Default password:

```
123456
```

Change inside `index.html`:

```
if(pass!=="123456")
```

---

## 📁 Database Structure

Collection:

```
families
```

Document stores:

* registered_date
* collected_date
* status

---

## 🌍 Use Cases

* Food distribution
* Relief camps
* Event check-in
* Token redemption
* Coupon validation
* Attendance tracking

---

## 🎨 Customization

You can modify:

* colors & theme
* language
* password
* UI text
* layout

Everything is in:

```
public/index.html
```

---

## 🤝 Contributing

Pull requests are welcome.

Ideas:

* Offline support
* Multi-event support
* Export to Excel
* Native Android wrapper

---

## 📜 License

Free to use for community and non-commercial purposes.

---

## ❤️ Final Note

This project was created to solve a real-world operational problem.

Not as a tutorial.

Not as a demo.

But to make distribution **fair, transparent, and respectful**.

If it helps your community, the project achieved its purpose.
