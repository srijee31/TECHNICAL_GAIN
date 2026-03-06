🎯 Technical Concept: HTTP Status Codes
The server’s way of talking back with numbers.

🤔 What are Status Codes?
Whenever your app talks to a server, the server always replies with a 3-digit number. This number tells the app the final result of the request.
It’s like a delivery app giving you an instant status update.
It helps the app decide whether to show your "Home Screen" or an "Error Message."

✅ The "Big Five" You Need to Know
These are the most common codes you will encounter in QA and Backend development.
🟢 200 – OK
Meaning: Everything worked perfectly.
Analogy: "Order delivered successfully." 📦
Result: The app loads your data and the user is happy.
🟡 400 – Bad Request
Meaning: The server didn't understand you because you sent something wrong.
Analogy: "You entered a delivery address that doesn't exist." 📍
Result: Usually happens if you miss a required field in a form.
🔒 401 – Unauthorized
Meaning: You aren't logged in, or your Token is invalid/expired.
Analogy: "Show your ID card before entering." 🪪
Result: The app kicks you back to the login screen.
🚫 403 – Forbidden
Meaning: The server knows who you are, but you aren't allowed to do that.
Analogy: "Staff Only. You don't have the keys to this room." 🔑
Result: Example: A regular user trying to delete another user's post.
❓ 404 – Not Found
Meaning: The URL or data you asked for does not exist.
Analogy: "We drove to the address, but there is no house there." 🏠
Result: A broken link or a deleted post.
💥 500 – Internal Server Error
Meaning: You did everything right, but the server crashed or had a bug.
Analogy: "The kitchen caught fire while cooking your meal." 🔥
Result: This is a Backend Bug. The developer needs to check the logs.

🧠 The "Golden Rule" of Grouping
If you forget the specific numbers, just remember the first digit:
2xx: Success! (Everything is fine) ✅
4xx: Your Mistake (The Client/App sent bad data) 🙋‍♂️
5xx: Server's Mistake (The Backend/Code crashed) 🧑‍💻

🧪 QA Brain Shortcut 🧠
When you are testing the Fitbit or Pixel Watch app and an error pops up, check the network log:
See a 4xx? Check if you entered the wrong password or if the watch is disconnected.
See a 5xx? Don't waste time on the app—go tell the Backend developers their server is down.

💡 One-Line Takeaway:
Status codes are just numbers with attitude—they tell you exactly who to blame for a bug.


