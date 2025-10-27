# 🧠 Computer Security – September 2025 Assignment

**Assignment:** Cryptography Design and Application 

**Members:** 
* Muhammad Ikmal Iman Bin Mohd Najib
* Muhammad Haikal Zikry
* Muhammad Danish Awra

**Course:** Computer Security

**Date:** 26th October 2025

---

## 📘 Overview

This repository contains all the Python implementations and demonstrations for the **Cryptography Design and Application**.
Each section demonstrates a different encryption concept using **custom-designed algorithms** developed in Python and tested using **Google Colab**.

---

## 🧩 Components Summary

| Part    | Title                                        | Description                                                                                                   |
| ------- | -------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **A.1** |  **MangoTango (Stream Cipher)**            | Custom stream cipher using dual LFSRs and nonlinear keystream generation.                                     |
| **A.2** |  **WingsDings (Block Cipher)**             | 64-bit Feistel-based block cipher using SHA-256-derived subkeys.                                              |
| **B**   |  **Hybrid Secure Chat (RSA + WingsDings)** | Demonstrates hybrid cryptography combining asymmetric and symmetric encryption in a secure messaging context. |

---

## ⚙️ Environment Setup (Google Colab)

All source codes were developed and tested using **Google Colab**, so no complex setup is required.

### 🧾 Requirements

Before running the code, ensure you have:

* A Google account (to access Colab)
* Internet connection
* `pycryptodome` library (for RSA encryption)

### 🔧 Install Required Library

Run this cell first in your Colab notebook:

```python
!pip install pycryptodome
```

---

## 🥭 Running MangoTango (Stream Cipher)

**File:** `Stream_Cipher.ipynb`
**Concept:** Original stream cipher demonstrating keystream generation, encryption, and decryption.

### ▶️ Steps in Colab:

1. Upload or open the `Stream_Cipher.ipynb` file in Colab.
2. Run all cells in sequence.
3. Enter your plaintext when prompted.

### 💻 Example Output:

```
===== MangoTango Stream Cipher Demo =====
Enter plaintext to encrypt: Good morning
[+] Encryption complete!
Ciphertext (hex): 8a5e3a12bcd9f12f
Decrypted text:   Good morning
Success: Decryption matches original plaintext.
```

---

## 🦅 Running WingsDings (Block Cipher)

**File:** `Block_Cipher.ipynb`
**Concept:** Feistel-based block cipher that uses SHA-256 to generate round keys and PKCS#7 padding for multi-block messages.

### ▶️ Steps in Colab:

1. Upload or open the file `Block_Cipher.ipynb` in Colab.
2. Run each cell from top to bottom.
3. Input your message when prompted.

### 💻 Example Output:

```
===== WingsDings Block Cipher Demo =====
Enter plaintext to encrypt: Careful who is behind you..
[+] Encryption complete!
Ciphertext (hex): 94e84af08f37d2f1a81c7841
Decrypted text:   Careful who is behind you..
Success: Decryption matches original plaintext.
```

---

## 🔐 Running Hybrid Cryptography Demo (Secure Chat)

**File:** `Hybrid_Demo_Secure_Chat.ipynb`
**Concept:** Combines RSA (asymmetric) for key exchange with WingsDings (symmetric) for fast message encryption. Demonstrates hybrid cryptography for a secure chat application.

### ▶️ Steps in Colab:

1. Upload or open `Hybrid_Demo_Secure_Chat.ipynb` in Colab.
2. Run the notebook step-by-step.
3. Enter a message when prompted — it will be encrypted by “Alice” and decrypted by “Bob”.

### 💻 Example Output:

```
===== Hybrid Cryptography Demo – Secure Chat =====
[1] Generating RSA key pair for Bob...
[2] Alice enters message to send securely: There is someone in your house
[+] Message encrypted successfully.
[3] Bob decrypts the incoming message...
Decrypted message: There is someone in your house
Success: Message decrypted correctly.
```

---

## 📂 Repository Structure

```
.
├── Stream_Cipher.ipynb                                         # MangoTango stream cipher 
├── Block_Cipher.ipynb                                          # WingsDings block cipher
├── Hybrid_Demo_Secure_Chat.ipynb                               # Hybrid cryptography demo 
│
├── MangoTango.drawio.png                                       # Stream cipher design diagram
├── WingsDing.drawio.png                                        # Block cipher Feistel structure diagram
├── Hybrid Cryptography Workflow Diagram_Secure Chat.drawio.png  # Hybrid workflow diagram
│
└── README.md                                                   # Documentation and instructions

```

---

## 🧠 Learning Outcomes

By running these notebooks, you will:

* Understand the **difference between stream and block ciphers**.
* Learn how **keystreams, subkeys, and Feistel rounds** operate.
* Implement and visualize **hybrid cryptography** combining symmetric and asymmetric encryption.
* Gain hands-on experience in **secure communication design**.

---

## ⚠️ Security Disclaimer

All algorithms (MangoTango, WingsDings) are **custom and educational**.
They are **not secure for real-world use** and are implemented purely for learning cryptographic design principles.

---

✅ **End of README**

---
