# REST API Structure

## What is REST API?

REST (Representational State Transfer) is a standard way of designing APIs.

---

## Key Principles

### 1. Stateless
Each request is independent

---

### 2. Resource-Based
Everything is treated as a resource

Example:
/users
/products

---

### 3. Use HTTP Methods

- GET → fetch data
- POST → create data
- PUT → update data
- DELETE → remove data

---

## Example API

GET /users → get all users  
GET /users/1 → get one user  
POST /users → create user  
PUT /users/1 → update user  
DELETE /users/1 → delete user  

---

## Good API Design

❌ Bad:
getUsersData

✅ Good:
/users

---

## Key Points

- Use nouns, not verbs
- Keep URLs clean
- Follow standard HTTP methods
