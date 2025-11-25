# File-Encryptor-Decryptor

<img width="1301" height="641" alt="Screenshot 2025-11-25 210058" src="https://github.com/user-attachments/assets/9bb68dc3-4316-4cd1-98f4-2923074762ed" />
<img width="1242" height="702" alt="Screenshot 2025-08-16 183345" src="https://github.com/user-attachments/assets/8e4e8855-1522-471a-9ed9-3d3570d95165" />











A simple and secure Flask-based web application that allows users to upload files and encrypt or decrypt them using Fernet (AES-128 CBC + HMAC) encryption.
This tool ensures confidentiality by generating a unique key for every encryption session and securely handles files on the server.
🚀 Features

🔐 Encrypt any file using Python’s cryptography library.

🔓 Decrypt encrypted files using the stored key.

📁 Secure file upload handling with Werkzeug.

📦 Download encrypted/decrypted files directly.

⚠️ Handles invalid keys, missing files, and wrong decrypt attempts gracefully


| Component            | Technology Used         | Purpose                                         |
| -------------------- | ----------------------- | ----------------------------------------------- |
| **Frontend**         | HTML, CSS               | UI for file upload + encrypt/decrypt actions    |
| **Backend**          | Python, Flask           | Server-side processing of encryption/decryption |
| **Security**         | `cryptography` (Fernet) | AES-based file encryption/decryption            |
| **File Handling**    | `Werkzeug`, `os`        | Secure file saving + retrieval                  |
| **Templates Engine** | Jinja2 (Flask built-in) | Dynamic rendering of results                    |
| **Storage**          | Local file system       | Store uploads & encrypted outputs               |


/project-folder
│── app.py
│── Secret.key       (auto-generated)
│── /uploads         (auto-created for storing files)
│── /templates
│     └── index.html


How to run?

1. Install Required Dependencies
pip install flask cryptography werkzeug

4️⃣ Run the Application
python app.py

5️⃣ Open in Browser

Visit:

http://127.0.0.1:5000/
