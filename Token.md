🪪 Technical Concept: What is a Token?
How apps remember you without asking for a password every 5 seconds.
🤔 The Core Problem
Imagine if every time you liked a photo on Instagram, a popup appeared saying: "Please enter your password to confirm it's you." * It would be torture 😵‍💫

It would be incredibly slow 🐌

It would be a massive security risk to send your password over the wire constantly.

How do we prove it’s "still us" after the first login?

🎟️ Enter: The Token
In simple words, a Token is a digital "ID Card" or "Entry Pass" that your app carries after you log in for the first time.

🔄 The Step-by-Step Login Flow
The Handshake: You enter your username + password.

The Verification: The App sends them to the API. The Server checks the database.

The Reward: The Server says, "You're legit! Here is a unique Token."

The Memory: Your app (frontend) saves this token in its memory (LocalStorage or Cookies).

The Proof: For every future request (viewing a profile, posting a comment), the app sends that Token instead of your password.

🎬 The "Movie Theater" Analogy
Buying the Ticket: This is your Login. You show your ID and pay.

The Hand Stamp: Once they check your ticket, they give you a UV Stamp on your hand.

Re-entry: When you go out for popcorn and come back, you don't show your ID again. You just show the Stamp.

The Stamp = The Token. It proves you already "logged in" at the front gate.

🔐 Why Tokens are Smarter than Passwords
Limited Life ⏳: Tokens can be set to expire (e.g., after 24 hours). A password stays the same forever until you change it.

Easy Revocation ❌: If you lose your phone, you can "Log out of all devices." The server simply deletes those tokens, making them useless.

Scope: A token can be restricted. For example, a token might allow you to "Read Posts" but not "Delete Account."

🧪 What happens when a Token Expires?
Your app sends the old token to the API.

The Server checks its "expiration date" and says: "Nope. This pass is too old."

The API sends back a 401 Unauthorized error.

The App sees this and automatically kicks you back to the Login Screen.

🧾 What is a JWT? (The name you'll see everywhere)
JWT stands for JSON Web Token.
Think of a JWT as a "Smart Token." It doesn't just say "I'm a user"; it carries encoded data inside it, like:

Your User ID

Your Role (Admin vs. User)

Exactly when the token expires

💡 One Killer Line to Remember:
A Password proves who you are ONCE. A Token proves who you are EVERY TIME after.
