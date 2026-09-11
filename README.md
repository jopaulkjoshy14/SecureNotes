# 🔐 SecureNotes

A privacy-focused, client-side notes application that allows users to create, edit, and manage personal notes securely in their browser.

SecureNotes uses the Web Crypto API to protect stored notes with password-based encryption. No backend server or database is required, and note data remains stored locally in the user's browser.

## 🌐 Live Demo

[Open SecureNotes](https://securenotes-kmpl.onrender.com)

## ✨ Features

- Create and manage personal notes
- Add, edit, and delete notes
- Password-based access
- Client-side encryption using the Web Crypto API
- AES-GCM encryption for stored note data
- PBKDF2-based password key derivation
- Encrypted persistence using browser LocalStorage
- Offline-capable after the application is loaded
- Responsive interface for desktop and mobile devices
- Dedicated About page
- No backend server or external database required

## 🔒 Security and Privacy

SecureNotes is designed around a client-side privacy model.

The application performs encryption and decryption directly in the browser. Notes are encrypted before being stored in LocalStorage, and the application does not send note content to a backend server.

The project uses:

- **AES-GCM** for authenticated encryption
- **PBKDF2** for deriving an encryption key from the user's password
- **Web Crypto API** for browser-based cryptographic operations
- **LocalStorage** for encrypted local persistence

### Important Security Note

SecureNotes is intended as an educational and personal privacy project. It does not replace a professionally audited password manager or enterprise-grade secure storage system.

The security of the application also depends on:

- Choosing a strong password
- Keeping the browser and operating system secure
- Avoiding malicious browser extensions
- Protecting access to the user's device
- Understanding that clearing browser storage may permanently remove stored notes

## 🛠️ Technology Stack

- HTML5
- CSS3
- JavaScript
- Bootstrap
- Web Crypto API
- LocalStorage
- GitHub
- Render

## 📁 Project Structure

```text
SecureNotes/
├── css/
│   └── styles.css
├── js/
│   ├── crypto.js
│   ├── login.js
│   ├── notes.js
│   └── storage.js
├── index.html
├── notes.html
├── about.html
└── README.md
```

## 🚀 How to Run Locally

Because SecureNotes is a static web application, no backend server or package installation is required.

### Option 1: Open Directly

1. Download or clone the repository.
2. Open the project folder.
3. Open `index.html` in a modern browser.

### Option 2: Use a Local Development Server

Clone the repository:

```bash
git clone https://github.com/jopaulkjoshy14/SecureNotes.git
```

Move into the project directory:

```bash
cd SecureNotes
```

Then serve the project using any local static server or an editor extension such as Live Server.

## 🧭 Application Flow

1. Open the application.
2. Create a password during the first visit.
3. Sign in using the configured password.
4. Create, edit, or delete notes.
5. Notes are encrypted before being stored locally.
6. Sign out when finished.
7. Sign in again to access the stored notes.

## 💾 Data Storage

SecureNotes stores encrypted application data in the browser's LocalStorage.

The application does not use:

- A backend API
- A cloud database
- A user account system
- External note synchronization
- Server-side note processing

Because the data is stored locally, notes are specific to the browser and device where they were created.

Clearing browser storage, changing browsers, or using a different device may make previously stored notes unavailable.

## 📱 Responsive Design

The interface is designed to work across:

- Desktop computers
- Laptops
- Tablets
- Mobile devices

The layout adapts to different screen sizes while maintaining a simple and accessible note-management experience.

## 🎯 Project Objective

The objective of SecureNotes is to demonstrate how modern browser technologies can be used to build a lightweight privacy-focused application without relying on a backend server.

The project focuses on:

- Client-side cryptography
- Password-based key derivation
- Encrypted browser storage
- Secure application flow
- Responsive frontend design
- Privacy-conscious software development

## ⚠️ Limitations

- Notes are stored only in the current browser's LocalStorage.
- There is no cloud synchronization.
- Password recovery is not available.
- Losing the password may prevent access to stored notes.
- Clearing browser storage may permanently delete notes.
- The application has not undergone a formal security audit.
- The application should not be used as a replacement for professionally audited secure-storage software.


## 👨‍💻 Author

Developed by [Jopaul K Joshy](https://github.com/jopaulkjoshy14).

## ⭐ Support

If you find this project useful or interesting, consider starring the repository on GitHub.
