🧱 The Internet: Full Floor Plan
From Physical Cables to Secure Logins

🟢 FLOOR 0: The Foundation (Physical)
1️⃣ What is the Internet? 🌐
The internet isn't "magic"—it is simply millions of computers connected together to share data.
Your Phone: A client computer.
Google's Office: A room full of server computers.
The Connection: Fiber optic cables, Satellites, or Wi-Fi.
2️⃣ Server vs. Client 📱↔️🖥️
The Client: The device that asks (Browser, Mobile App).
The Server: The computer that waits and answers (Always on, always listening).

🟢 FLOOR 1 & 2: Finding the Address
3️⃣ The URL & DNS 📞
Humans like names (google.com), but computers only understand numbers (IP Addresses).
DNS (Domain Name System): The "Phonebook" of the internet.
The Flow: Browser → DNS → "Give me the IP for google.com" → 142.250.190.14.

🟢 FLOOR 3 & 4: The Rules of Conversation
4️⃣ HTTP / HTTPS 🔒
The protocol (rules) for how the Client and Server speak.
HTTP: Talking in clear text (Dangerous ❌).
HTTPS: Talking in code/encryption (Secure ✅).
5️⃣ The Request & Response Lifecycle 🔄
Every interaction follows this loop:
Request: Client says "GET /index.html".
Response: Server sends back HTML, CSS, JS, and a Status Code.


🟢 FLOOR 5: The Brain (Backend)
6️⃣ Backend & Database 🧠
Backend: The logic. It receives the request, checks permissions, and runs code.
Database: The permanent memory. It stores users, passwords, and posts.
Rule: The Browser never talks directly to the Database. It must go through the Backend "gatekeeper."

🟢 FLOOR 6: The Big Picture (Full Lifecycle) 🔥
How it all connects:
You → Browser → DNS → Server → Backend → Database → Response → You

🟢 FLOOR 7 & 8: Remembering & Identity
7️⃣ Cookies vs. LocalStorage 🍪
Cookies: Small data sent automatically with every request. Great for Sessions.
LocalStorage: Data stored in the browser that is not sent to the server automatically. Great for UI preferences.
8️⃣ Authentication (Sessions vs. JWT) 🪪
Sessions: Server remembers you (Hotel Key 🔑).
JWT: You carry your own proof (Signed ID Card Card 🪪).
