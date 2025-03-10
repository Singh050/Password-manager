# 🔐 Password Manager

A secure and simple password manager built with Python. This application encrypts your passwords and stores them securely using a master password system.

## 📌 Features
- Securely stores and manages passwords
- Uses a master password for encryption
- Command-line interface with interactive menu
- Error handling for missing files and incorrect inputs
- Uses `pycryptodome` for encryption and `halo` for interactive loading indicators

## 🛠️ Installation
### Prerequisites
- Python 3.6+
- Pip package manager

### Install Dependencies
To install the required dependencies, run:
```sh
pip install -r requirements.txt
```

## 🚀 Usage
Run the application with:
```sh
python main.py
```

### First-time Setup
1. The program will ask you to create a master password.
2. This password is required every time you start the application.
3. Once set, your passwords will be stored securely in `db/`.

### Adding & Managing Passwords
- Once the master password is entered, the interactive menu allows you to:
  - Add new passwords
  - Retrieve stored passwords
  - Remove passwords
  - Exit the program securely

## 📂 Project Structure
```
📂 Project
│── main.py  # Entry point of the application
│── requirements.txt  # Required dependencies
│── modules/
│   ├── encryption.py  # Encryption and decryption logic
│   ├── exceptions.py  # Custom exception handling
│   ├── menu.py  # Menu manager for user interactions
│── db/
    ├── masterpassword.json  # Stores encrypted master password
    ├── passwords.json  # Encrypted storage of passwords
```

## 🛡️ Security Considerations
- The master password is hashed using SHA-256 and stored securely.
- Ensure you **never lose your master password**, as it is unrecoverable.
- Always keep your password database (`db/`) secure and private.

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).

## 🤝 Contributing
Feel free to submit issues or pull requests to enhance this project.

## 🏆 Acknowledgments
Built using Python with `halo`, `termcolor`, and `pycryptodome` for encryption.

