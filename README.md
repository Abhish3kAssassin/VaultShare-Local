# 🔐 VaultShare — Secure File Transfer Web Application

A secure file transfer web application built to demonstrate real-world cybersecurity concepts including **encryption, integrity verification, access control, and secure communication**.

---

## 🚀 Features

- 🔑 User Authentication (Login / Register)
- 📤 Secure File Upload & Download
- 🔐 AES-256-GCM Encryption (before storage)
- 🧾 SHA-256 Integrity Verification
- 👥 Access Control (owner + shared users)
- ⏳ File Expiry System
- 📜 Activity & Transfer Logs
- 🌐 Multi-device access (same network)
- 💾 No database (JSON-based storage)

---

## 🧱 Tech Stack

| Layer       | Technology |
|------------|------------|
| Frontend   | HTML, CSS, JavaScript |
| Backend    | Node.js, Express |
| Security   | Crypto (AES-256-GCM, SHA-256, PBKDF2) |
| Storage    | Local filesystem + JSON |

---

## ⚙️ How It Works

1. User logs in or registers  
2. File is uploaded via web interface  
3. File is encrypted using **AES-256-GCM**  
4. SHA-256 hash is generated for integrity  
5. File + metadata stored locally  
6. Only authorized users can access/download  
7. Integrity is verified before use  

---

## 🔐 Security Implementation

- 🔒 **Password Hashing:** PBKDF2 with salt  
- 🔑 **Session Management:** HMAC-signed tokens  
- 🛡️ **Encryption:** AES-256-GCM (confidentiality + authenticity)  
- 🧾 **Integrity:** SHA-256 hashing  
- 🚫 **Rate Limiting:** Prevent brute-force attacks  
- 🔐 **Access Control:** Owner + allowed users  

---

## 🖥️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/Abhish3kAssassin/VaultShare-Local.git
```

### 2. Install dependencies
```bash
npm install
```

### 3. Run the server
```bash
npm start
```

### 4. Open in browser
```
http://localhost:3000
```

---

## 🌐 Access from Other Devices

1. Find your local IP:
```bash
ipconfig
```

2. Open on another device (same Wi-Fi):
```
http://YOUR_IP:3000
```

3. Ensure:
- Firewall allows port `3000`
- Network is set to **Private**

---

## 📂 Project Structure

```
vaultshare/
│
├── server.js
├── package.json
├── storage/
│   ├── uploads/
│   ├── meta/
│   ├── logs/
│   ├── users.json
│   └── files.json
│
├── public/
│   ├── index.html
│   ├── style.css
│   └── app.js
│
└── README.md
```

---

## 📊 Example Use Case

- Upload a file from your PC  
- Share access with another user  
- Access the app from your phone  
- Download securely with integrity verification  

---

## ⚠️ Limitations

- ❌ Not production-ready  
- ❌ No HTTPS/TLS  
- ❌ No database (uses JSON files)  
- ❌ Basic authentication (no OAuth/JWT yet)  

---

## 🚀 Future Improvements

- 🔵 WebSockets (real-time updates)  
- 🔴 JWT-based authentication  
- 🟢 Database (PostgreSQL / MongoDB)  
- 🟡 File sharing via secure links  
- 🟣 Download tracking UI  
- ⚡ Drag & drop file upload  
- 🔐 TLS (HTTPS support)  

---

## 🏆 Resume Description

> Developed a secure file transfer web application using Node.js and Express, implementing AES-256 encryption, SHA-256 integrity verification, and role-based access control for secure file sharing across local networks.

---

## 💡 Why This Project Stands Out

- Combines **cybersecurity + full-stack development**
- Implements **real encryption (not just theory)**
- Demonstrates **secure system design**
- Works across **multiple devices on a network**

---

## 📜 License

MIT License (or choose your own)

---

## 👨‍💻 Author

Your Name  
Cybersecurity Enthusiast
