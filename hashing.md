# 🔑 What is Hashing?

## 1. Introduction

Hashing is a process that converts data into a **fixed-length string of characters**, called a **hash value** or **hash code**.

The original data can be of any size, but the hash output is always a **fixed size**.

Hashing is mainly used for:

- Password storage
- Data integrity verification
- Digital signatures
- Blockchain technology

---

## 2. Real-Life Analogy

Think of hashing like a **fingerprint for data**.

Just like every person has a unique fingerprint, every piece of data produces a unique hash value.

Example:
Hello → 185f8db32271fe25f561a6fc938b2e264306ec304eda518007d1764826381969


Even a small change in the input will produce a **completely different hash**.

Example:


Hello → 185f8db32271fe25f561a6fc938b2e264306ec304eda518007d1764826381969
hello → 2cf24dba5fb0a030e...


Notice that just changing **H → h** creates a totally different hash.

---

## 3. Why Hashing is Important

Hashing is used to:

- Secure passwords
- Detect data tampering
- Verify file integrity
- Protect sensitive information

It ensures that data has **not been modified**.

---

## 4. How Hashing Works

### Step 1: Input Data

Example:


mypassword


---

### Step 2: Hash Function Applied

A mathematical algorithm converts the input into a hash.

Example:


mypassword → 91dfd9ddb4198affc5c194cd8ce6d338fde470e2


---

### Step 3: Store the Hash

Instead of storing the password, the system stores the **hash value**.

Example database record:


User: Srijee
Password Hash: 91dfd9ddb4198affc5c194cd8ce6d338fde470e2


---

### Step 4: Login Verification

When the user logs in:

1. User enters password
2. System hashes the entered password
3. System compares it with the stored hash

If both hashes match, access is granted.

Example flow:


User Input → Hash Function → Compare with Stored Hash → Login Success


---

## 5. Characteristics of Hashing

A good hashing algorithm has these properties:

| Property | Description |
|--------|-------------|
| Deterministic | Same input always produces same hash |
| Fixed Length Output | Hash output size is constant |
| Fast Computation | Hash generation is quick |
| Collision Resistant | Difficult for two inputs to produce same hash |
| One-way Function | Original data cannot be easily retrieved |

---

## 6. Popular Hashing Algorithms

Common hashing algorithms include:

- MD5
- SHA-1
- SHA-256
- SHA-3

Modern systems commonly use **SHA-256** because it is more secure.

---

## 7. Real-Life Example

When you create an account on a website:

1. You enter a password
2. The system hashes the password
3. Only the hash is stored in the database

Even if hackers steal the database, they **cannot easily recover the original password**.

---

## 8. Simple Summary

Hashing is a process that converts data into a unique fixed-length value used for **secure storage and data verification**.
