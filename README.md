
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
