# 🔤 What is Encoding?

## 1. Introduction

Encoding is the process of converting data from one format into another format so that it can be **easily stored, transmitted, or processed by different systems**.

Encoding is **not meant for security**. Its main purpose is **data compatibility and communication between systems**.

---

## 2. Real-Life Analogy

Imagine translating a sentence from **English to Morse code**.

Example:


HELLO

Encoded in Morse code:


.... . .-.. .-.. ---


The information is still the same, but it is represented in a **different format**.

---

## 3. Why Encoding is Used

Encoding helps computers and systems to:

- Transmit data safely over networks
- Store data in compatible formats
- Represent binary data in text form
- Ensure systems understand each other

Common uses of encoding include:

- email attachments
- web data transmission
- file storage
- multimedia formats

---

## 4. How Encoding Works

### Step 1: Original Data

Example:


Hello


---

### Step 2: Encoding Algorithm Applied

The data is converted into another format.

Example using Base64 encoding:


Hello → SGVsbG8=


---

### Step 3: Transmission or Storage

The encoded data can now be safely transmitted or stored.

---

### Step 4: Decoding

The receiver decodes the data back to the original form.

Example:


SGVsbG8= → Hello


---

## 5. Common Encoding Types

| Encoding Type | Purpose |
|---------------|---------|
| Base64 | Used to encode binary data into text |
| ASCII | Character encoding for computers |
| Unicode | Supports characters from many languages |
| URL Encoding | Used in web addresses |

---

## 6. Real-Life Example

### Email Attachments

When you send a file through email:

1. The file is **encoded into Base64**
2. The encoded data is sent through email
3. The receiver decodes it back to the original file

---

## 7. Encoding vs Encryption vs Hashing

| Method | Purpose | Reversible |
|------|---------|-----------|
| Encoding | Data format conversion | Yes |
| Encryption | Data security | Yes (with key) |
| Hashing | Data integrity and password storage | No |

---

## 8. Simple Summary

Encoding converts data into a different format so it can be **easily t
