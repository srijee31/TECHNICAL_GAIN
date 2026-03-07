# Authentication

## Definition
Authentication is the process of **verifying the identity of a user**.

In simple words:

> Authentication answers the question:  
> **"Are you really who you say you are?"**

If the system confirms your identity → you are authenticated.

---

## Simple Example

When you log into an app:

1. You enter **email and password**
2. The request goes to the **server**
3. The server checks the **database**
4. If details match → Login successful
5. If not → Login failed

Flow:
# Authentication

## Definition
Authentication is the process of **verifying the identity of a user**.

In simple words:

> Authentication answers the question:  
> **"Are you really who you say you are?"**

If the system confirms your identity → you are authenticated.

---

## Simple Example

When you log into an app:

1. You enter **email and password**
2. The request goes to the **server**
3. The server checks the **database**
4. If details match → Login successful
5. If not → Login failed

Flow:
User → Login Request → Server → Database Check → Access Granted




---

# Real Life Analogy

Imagine entering an **office building**.

Security asks for your **ID card**.

- If the ID is valid → You can enter
- If the ID is invalid → Entry denied

Your **ID card acts as authentication proof**.

---

# Authentication vs Authorization

These two concepts are often confused.

| Concept | Meaning |
|--------|--------|
| Authentication | Verifying **who the user is** |
| Authorization | Verifying **what the user is allowed to access** |

Example (Instagram):

- Authentication → Logging into the account
- Authorization → Accessing profile settings, messages, etc.

---

# Types of Authentication

## 1. Password-Based Authentication

This is the most common method.

Users provide:

- Username or Email
- Password

Example:
Email: srijee@gmail.com

Password: ********



The server checks the credentials against the stored data.

---

## 2. OTP Authentication

OTP stands for **One-Time Password**.

A temporary password is sent to:

- Mobile number
- Email

Example:
Enter OTP: 493821


OTP works only once and expires after a short time.

Commonly used in:

- Banking applications
- Payment apps
- WhatsApp login verification

---

## 3. Token-Based Authentication

Instead of verifying credentials every time, the server generates a **token**.

A token acts as proof that the user has already logged in.

Example: **JWT (JSON Web Token)**

Flow:

Login → Server verifies credentials → Token generated → Client stores token


For future requests, the client sends the token.

Example request header:


Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6...


The server validates the token and allows access.

---

# Authentication Flow in Modern Web Applications

Typical authentication workflow:

1. User enters email and password
2. Client sends request to server
3. Server checks credentials in the database
4. If correct → Server generates authentication token
5. Token is sent to the client
6. Client stores token (cookie or local storage)
7. Token is used for future requests

---

# Where User Credentials are Stored

User data is stored in a **database**.

Example table:

| id | email | password_hash |
|----|------|---------------|
| 1 | srijee@gmail.com | hashed_password |

Important security rule:

> Passwords should **never be stored as plain text**

Instead, they are stored as **hashed values**.

Common hashing algorithms:

- bcrypt
- Argon2
- SHA

---

# Why Authentication is Important

Without authentication:

- Anyone could access accounts
- Sensitive data could be stolen
- Systems would become insecure

Authentication protects:

- User accounts
- Personal data
- Financial information
- Application security

---

# Simple Python Authentication Example

```python
username = input("Enter username: ")
password = input("Enter password: ")

if username == "admin" and password == "1234":
    print("Login successful")
else:
    print("Invalid credentials")

In real-world applications, the backend checks credentials using a database instead of hardcoded values.

Applications That Use Authentication

Almost every modern application uses authentication.

Examples:

Gmail

Instagram

Netflix

Amazon

Banking applications

Authentication ensures that only verified users can access their accounts.

Summary

Authentication is a core part of backend development.

Key points:

It verifies the identity of users

It protects user accounts and data

It can be implemented using passwords, OTP, or tokens

Modern systems often use JWT tokens and secure hashing
