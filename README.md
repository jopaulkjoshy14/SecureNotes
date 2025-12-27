# 🔐 SecureNotes

SecureNotes is a privacy-focused notes application that uses **client-side encryption** to protect user data.  
All notes are encrypted in the browser before being stored, ensuring that sensitive data never leaves the client unencrypted.

---

## 🌍 Live Demo

🔗 App: https://securenotes-kmpl.onrender.com  
🔗 Repository: https://github.com/jopaulkjoshy14/SecureNotes  

---

## 🚀 Features

- 🔒 Client-side encryption using **AES-GCM** via the Web Crypto API  
- 🔑 Password-based access (encryption key derived from user password)  
- 📝 Create, edit, and delete notes securely  
- 💾 Encrypted persistence using LocalStorage  
- 🌐 Fully offline-capable (works without internet after loading)  
- 🧩 No backend required — pure HTML, CSS, and JavaScript  
- 🛡 Clean separation of cryptography, storage, and UI logic  

---

## 📁 Project Structure

SecureNotes/ 
│ 
├── index.html            # Login page
├── notes.html            # Notes interface 
│ 
├── css/ 
│   
└── styles.css        # UI styling 
│ 
├── js/ 
│   
├── crypto.js         # Encryption & decryption logic 
│   
├── storage.js        # Encrypted LocalStorage handling 
│   
├── login.js          # Password handling & key derivation 
│   
└── notes.js          # Notes CRUD functionality 
│ 
└── assets/               # Images / icons

---

## 🛠️ Tech Stack

- HTML5  
- CSS3  
- Vanilla JavaScript (ES6)  
- Web Crypto API  
- LocalStorage API  

---

## 🔐 Encryption Details

SecureNotes uses modern browser cryptography features to protect data:

- **PBKDF2** for deriving encryption keys from the user password  
- **AES-GCM (256-bit)** for authenticated encryption  
- Random salt for each key derivation  
- Random IV for every encryption operation  

> All encryption and decryption happens locally in the browser.

---

## 🚀 Deployment

This is a static web application with no backend.

- Hosted on **Render**
- No build step required
- Render serves the app directly from the repository root

Live URL:  
👉 https://securenotes-kmpl.onrender.com

---

## 📸 Screenshots

![Login Page](assets/login.png)
![Notes Interface](assets/notes.png)

---

## 🧭 Roadmap

Export / Import encrypted notes
Search functionality inside notes
UI and accessibility improvements

---

## 📄 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it with attribution.

---

## 👤 Author

Jopaul K Joshy
🔗 Portfolio: https://portfolio-kuf9.onrender.com
🔗 LinkedIn: https://www.linkedin.com/in/jopaul-k-joshy-75a7a6299
