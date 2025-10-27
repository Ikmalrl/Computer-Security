# 🧠 Computer Security – September 2025 Assignment

**Assignment:** Cryptography Design and Application 

**Members:** 
* Muhammad Ikmal Iman 
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
| **A.1** |  **LunarBlaze (Stream Cipher)**            | Custom stream cipher using dual LFSRs and nonlinear keystream generation.                                     |
| **A.2** |  **CyberStone (Block Cipher)**             | 64-bit Feistel-based block cipher using SHA-256-derived subkeys.                                              |
| **B**   |  **hybrid cryptography**                   | Demonstrates hybrid cryptography combining asymmetric and symmetric encryption in a secure messaging context. |

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

## 🥭 Running LunarBlaze (Stream Cipher)

**File:** `LunarBlaze.ipynb`
**Concept:** Original stream cipher demonstrating keystream generation, encryption, and decryption.

### ▶️ Steps in Colab:

1. Upload or open the `LunarBlaze.ipynb` file in Colab.
2. Run all cells in sequence.
3. Enter your plaintext when prompted.

### 💻 Example Output:

```
===== LunarBlaze Stream Cipher =====
Enter plaintext: computer security

Status          : Encryption complete!
Ciphertext (hex): 9c3a37508e0b7b3fd17c0a888799bddbb2
Decrypted text  : computer security

Success: Decryption matches with the plaintext.
```

---

## 🦅 Running WingsDings (Block Cipher)

**File:** `CyberStone.ipynb`
**Concept:** Feistel-based block cipher that uses SHA-256 to generate round keys and PKCS#7 padding for multi-block messages.

### ▶️ Steps in Colab:

1. Upload or open the file `CyberStone.ipynb` in Colab.
2. Run each cell from top to bottom.
3. Input your message when prompted.

### 💻 Example Output:

```
===== CyberStone Block Cipher =====
Enter plaintext: computer security

Status          : Encryption complete!
Ciphertext (hex): e632b890ddfb198283f70679847424c4d7d37c84b7bb3892
Decrypted text  : computer security

Success: Decryption matches with the plaintext
```

---

## 🔐 Running Hybrid Cryptography Demo (Secure Chat)

**File:** `Hybrid_cryptography.ipynb`
**Concept:** Combines RSA (asymmetric) for key exchange with CyberStone (symmetric) for fast message encryption. Demonstrates hybrid cryptography for a secure chat application.

### ▶️ Steps in Colab:

1. Upload or open `Hybrid_Demo_Secure_Chat.ipynb` in Colab.
2. Run the notebook step-by-step.
3. Enter a message when prompted — it will be encrypted by “Alice” and decrypted by “Bob”.

### 💻 Example Output:

```
===== Hybrid Cryptography Demo =====
[1] Generating RSA key pair for Bob...
[2] Alice enters message to send securely: Hi Bob!

Encryption complete!
Encrypted session key length: 256 bytes
Encrypted message (hex): e2c84ce0e5e76f59

[3] Bob decrypts the incoming message...

Decryption complete!
Decrypted message: Hi Bob!

Success: Message decrypted correctly.
```

---

## 📂 Repository Structure

```
.
├── LunarBlaze.ipynb                                         # Stream cipher 
├── CyberStone.ipynb                                          # Block cipher
├── Hybrid_Demo_Secure_Chat.ipynb                               # Hybrid cryptography 
│
├── LunarBlaze.drawio.png                                       # Stream cipher design diagram
├── CyberStone.drawio.png                                        # Block cipher Feistel structure diagram
├── Hybrid Cryptography.drawio.png                              # Hybrid workflow diagram
│
└── README.md                                                   # Documentation and instructions

```

