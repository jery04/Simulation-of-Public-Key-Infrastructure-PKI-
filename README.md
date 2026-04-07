# 🏢🤝🔒 Simulation of Digital Signature and Encryption between Company and Provider

This project is a **simulation** of a digital signature and message encryption process between a **company** and a **provider**, using Python's `cryptography` library. The goal is to demonstrate how documents and communications can be protected in a digital environment, ensuring **authenticity**, **integrity**, and **confidentiality**.

> ⚠️ **Note:** This work is primarily aimed at showing **how the solution and implementation are carried out**, rather than for practical execution. It's ideal for understanding the procedure and the cryptographic steps involved, not for production or automated use.

## 🚀 What this project does

- **Generates public and private keys** for both parties (company and provider).
- **Creates a digital contract** that can be signed by both parties.
- **Digitally signs** the contract using private keys and verifies the signatures using public keys.
- **Attaches simulated digital certificates** to each signature.
- **Encrypts and decrypts messages** between the company and the provider, including a timestamp for added security.
- **Exports the signed document** in JSON format, showing all signatures and certificates.

## 🛡️ Why it's secure

The project uses the `cryptography` library, which implements modern and robust cryptographic algorithms such as:

- **RSA** for key generation, digital signatures, and asymmetric encryption.
- **SHA-256** for secure hash generation.
- **OAEP and PSS padding** to protect against known cryptographic attacks.
- **Timestamps** to prevent replay attacks and ensure temporal validity of signatures and messages.

These tools allow simulating a real document and communication protection system similar to those used in **PKI (Public Key Infrastructure)** systems in real-world environments.

## 📦 Code structure

- **PKI.py**: Contains all the logic for key generation, signing, verification, encryption, decryption, and handling certificates and documents.
- **README.md**: This file, explaining the project.

## 📝 Usage example

When running the script you will see how:
1. A contract is created.
2. The company signs it digitally.
3. The provider verifies the signature and, if valid, also signs the contract.
4. The contract signed by both parties is exported.
5. An encrypted message is sent from the company to the provider that only the provider can decrypt.

## 📚 Requirements

- Python 3.8+
- Install the `cryptography` library

