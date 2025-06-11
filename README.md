# 🧱 VexChain - Java Blockchain Implementation

[![Java](https://img.shields.io/badge/Language-Java-red.svg)](https://www.java.com/)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> A lightweight blockchain built in pure Java.  
> Perfect for understanding the **Usage** of blockchain technology.

---

## 📌 Features

- 🔐 **SHA-256 Hashing** for block integrity
- 🛠️ **Proof-of-Work** (mining) with adjustable difficulty
- 🔗 **Chained Hash Linking** between blocks
- ✅ **Self-Validation** for blockchain integrity
- 🧱 **Modular Design** for extensibility

---

## 🧠 Core Concepts

- **Immutability** – Each block contains a hash of the previous block
- **Proof of Work** – Blocks are mined using a nonce until a valid hash is found
- **Integrity Check** – The blockchain verifies itself to detect tampering

---

## 📁 Project Structure

### 📦 VexChain
- 📄 Block.java → Defines a single block (data, hash, nonce, etc.)
- 📄 StringUtil.java → Utility for SHA-256 hashing
- 📄 VexChain.java → Main blockchain runner

---

## 🚀 Getting Started

### 🧾 1. Clone the Repository

```bash
git clone https://github.com/vexyenv/vexchain.git
cd vexchain
```

### ⚙️ 2. Compile the Project

```bash
javac *.java
```

### ▶️ 3. Run the Blockchain

#### Example Output:

```bash
Mining Block 1... 
Block Mined: 0000096a6632e82cadf6cc5b28aa2abe30df590390f260a8f6daf21bf705aa88
Mining Block 2... 
Block Mined: 00000e5fae0d6a0ae831345eb22ba763706dc5e215455e65309cc76bab5f4ae0
Mining Block 3... 
Block Mined: 00000d48f2ebee2fe770a7577f0e153707d8007dfe863dd0d44625dac9f73ebe

Blockchain is Valid: true

The block chain: 
[
  {
    "hash": "0000096a6632e82cadf6cc5b28aa2abe30df590390f260a8f6daf21bf705aa88",
    "previousHash": "0",
    "data": "First Block",
    "timeStamp": 1749636051377,
    "nonce": 1654347
  },
  {
    "hash": "00000e5fae0d6a0ae831345eb22ba763706dc5e215455e65309cc76bab5f4ae0",
    "previousHash": "0000096a6632e82cadf6cc5b28aa2abe30df590390f260a8f6daf21bf705aa88",
    "data": "Second Block",
    "timeStamp": 1749636053548,
    "nonce": 898784
  },
  {
    "hash": "00000d48f2ebee2fe770a7577f0e153707d8007dfe863dd0d44625dac9f73ebe",
    "previousHash": "00000e5fae0d6a0ae831345eb22ba763706dc5e215455e65309cc76bab5f4ae0",
    "data": "Third Block",
    "timeStamp": 1749636054771,
    "nonce": 103372
  }
]
```

---
> Made with 💻 + ☕ by [Vexyenv](https://github.com/vexyenv) — Keep building!
