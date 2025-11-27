# 🔐 SecureNotes

SecureNotes is a lightweight, privacy-focused notes application that runs entirely in the browser.  
All notes are **encrypted client-side** using the Web Crypto API, ensuring that your data never leaves your device.

Perfect for secure personal note-taking, journaling, or storing sensitive information without relying on any server.

---

## 🚀 Features

- 🔒 **Client-side encryption** (AES-GCM via Web Crypto API)
- 🔑 **Password-protected login**
- 📝 **Create, edit, delete notes securely**
- 💾 **Encrypted LocalStorage persistence**
- 🌐 **Fully offline – works without internet**
- 🧩 **No backend required – pure HTML/CSS/JS**
- 🛡 **Clean separation of crypto, storage, and UI logic**

---

## 📁 Project Structure

SecureNotes/
│
├── index.html # Login page
├── notes.html # Notes UI
│
├── css/
│ └── styles.css
│
├── js/
  ├── crypto.js # Encryption/decryption logic
  ├── storage.js # Secure LocalStorage management
  ├── login.js # Handles login + password flow
  └── notes.js # Notes creation/edit/delete


yaml
Copy code

---

## 🛠️ Tech Stack

- **HTML5**
- **CSS3**
- **Vanilla JavaScript**
- **Web Crypto API**
- **LocalStorage**

---

## 🔐 How Encryption Works

SecureNotes uses the Web Crypto API to derive a key from the user's password using:

- `PBKDF2` → Key derivation  
- `AES-GCM` → Encryption & decryption  
- Random salts + IVs for every encryption  
- Everything is stored as encrypted strings in LocalStorage  

No data is ever sent to a server or external service.

---

## 📦 Installation & Usage

### **Option 1: Clone via GitHub**

```bash
git clone https://github.com/your-username/SecureNotes.git
cd SecureNotes
