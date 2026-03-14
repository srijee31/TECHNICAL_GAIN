# Ports in Computer Networking

## Introduction

A port is a **communication endpoint** used by computers to send and receive data over a network.

Ports allow multiple applications on the same device to communicate with the internet without interfering with each other.

A port works together with an **IP address** to identify a specific service or application.

Example:

IP Address → Identifies the device  
Port → Identifies the application on that device

---

## Why Ports Are Needed

A single computer can run many network services at the same time.

Examples:

- Web browser
- Email client
- Database server
- API server
- File transfer services

Ports help the operating system deliver incoming data to the **correct application**.

Without ports, the computer would not know which program should receive the data.

---

## Port Numbers

Port numbers range from:

0 – 65535

They are divided into three categories.

### Well-Known Ports (0–1023)

These ports are reserved for commonly used internet services.

Examples:

| Service | Port Number |
|-------|-------------|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 21 |
| SSH | 22 |
| DNS | 53 |

---

### Registered Ports (1024–49151)

These ports are assigned to specific applications or services.

Examples:

| Service | Port |
|------|------|
| MySQL | 3306 |
| PostgreSQL | 5432 |
| MongoDB | 27017 |

---

### Dynamic or Private Ports (49152–65535)

These ports are temporary ports used by client applications.

Example:

When a browser connects to a website, it may temporarily use a random port like:

52341

These ports are automatically assigned by the operating system.

---

## Example of Port Usage

When you open a website in a browser:

https://example.com

Behind the scenes:

IP Address → identifies the server  
Port → identifies the web service

Example:

Server IP: 93.184.216.34  
Port: 443 (HTTPS)

---

## Ports in Backend Development

When running a backend application locally, a port must be specified.

Example in Python:
app.run(port=5000)


The application will run on:


http://localhost:5000


Here:

- localhost → IP address (127.0.0.1)
- 5000 → Port where the application is listening

---

## Key Points

- A port is a communication endpoint used in networking.
- Ports help identify specific services on a device.
- Port numbers range from 0 to 65535.
- Well-known ports are reserved for common services like HTTP and HTTPS.
- Backend servers run on specific ports to handle requests.
