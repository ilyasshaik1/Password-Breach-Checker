
# 🔐 Password Breach Checker (Flask Web App)

A Flask-based web application to check if a password has appeared in known data breaches, using the **Have I Been Pwned** API.  
It uses the k-Anonymity model to protect your privacy — your full password is **never** sent over the internet.

---

## 🚀 Features
- 🔍 Check if a password has been compromised in data breaches.
- ✅ Uses secure k-Anonymity method (only first 5 hash characters sent).
- 💻 Simple and responsive UI built with Bootstrap.
- ⚡ Fast and lightweight — runs locally.

---

## 📸 Demo Screenshot
<img width="1156" height="659" alt="Screenshot 2025-08-14 164138" src="https://github.com/user-attachments/assets/c3e6326b-a095-444f-a382-2c74c0e55609" />
<img width="1851" height="677" alt="Screenshot 2025-08-14 164152" src="https://github.com/user-attachments/assets/0a894ad1-adee-4282-9822-8400d81c48c6" />
<img width="1889" height="582" alt="Screenshot 2025-08-14 164207" src="https://github.com/user-attachments/assets/1314513a-c287-4e48-b839-53b86eafc750" />



---

## 📂 Project Structure
```

password\_checker/
│
├── app.py                # Flask backend
├── static/
│   └── style.css         # Custom styling
└── templates/
└── index.html        # Frontend template

````

---

## 🛠 Installation

### 1. Clone the Repository
```bash
git clone [https://github.com/ilyasshaik1/Password-Breach-Checker](https://github.com/ilyasshaik1/Password-Breach-Checker.git)
cd password-checker
````

### 2. Install Dependencies

```bash
pip install flask requests
```

### 3. Run the Application

```bash
python app.py
```

### 4. Open in Browser

```
http://127.0.0.1:5000
```

---

## ⚙️ How It Works

1. User enters a password into the form.
2. The password is converted into a SHA-1 hash locally.
3. Only the **first 5 characters** of the hash are sent to the Have I Been Pwned API.
4. API returns possible matching hashes; the app checks locally if the password exists in the list.
5. Result is displayed without exposing the password.

---

## 📜 Example

**Input:**

```
mypassword123
```

**Output:**

```
⚠️ This password was found 120394 times. Change it!
```

---

## 🔒 Privacy Note

Your password is **never sent** in plain text or in full hash form — this ensures maximum privacy and security.

---

## 📄 License

This project is licensed under the MIT License.
Feel free to modify and use it in your own projects.
