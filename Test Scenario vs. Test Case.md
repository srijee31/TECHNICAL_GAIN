# 🧪 Test Scenario vs. Test Case
### The "What" vs. the "How" of professional testing.

---

## 🧠 The Core Mental Model
Before you even touch a device, you need a plan. Testing is divided into two layers: the **Goal** and the **Manual**.
**Requirement ➔ Test Scenario (The What) ➔ Test Case (The How)**



---

## 🎯 Test Scenario (The Big Picture)
A test scenario is a high-level description of a feature to be tested. It describes a **"Business Flow"** from the user's perspective.
* **No Steps:** Just the intent.
* **No Data:** No specific passwords or usernames yet.
* **Goal:** To ensure total **"Test Coverage"** (making sure we didn't forget a feature).

📝 **Example (Pixel Watch Sync):**
* Verify user can sync sleep data to the Fitbit app.
* Verify sync behavior when the phone Bluetooth is OFF.
* Verify sync behavior when the watch battery is below 5%.

---

## 🧪 Test Case (The Execution Level)
A test case is the detailed **"recipe"** used to execute one specific part of a scenario. It is what you actually follow when you are sitting with the device in your hand.

📦 **A Test Case must include:**
1.  **Preconditions:** (e.g., "Watch is paired with phone").
2.  **Steps:** (1. Open App, 2. Pull down to refresh...).
3.  **Test Data:** (Username: `test_user_01`, Password: `Password123`).
4.  **Expected Result:** (Sync icon rotates, data appears in 10 seconds).



---

## 🔥 Why this matters in Real Projects (The "Tea" ☕)
At companies like **HCLTech** or **Google**, you don't just start writing steps. 
* **Seniors start with Scenarios:** They map out the "Story" first to ensure every edge case is covered.
* **Juniors dive into Test Cases:** They often get stuck in the details and miss the "Big Picture" flows.
* **The Multiplier Effect:** One Scenario usually leads to multiple Test Cases (**Positive**, **Negative**, and **Edge cases**).

---

## 📊 Comparison at a Glance

| Feature | Test Scenario | Test Case |
| :--- | :--- | :--- |
| **Focus** | "What" to test (Goal) | "How" to test (Steps) |
| **Level** | High-level (Abstract) | Low-level (Detailed) |
| **Derivation** | Derived from Requirements | Derived from Scenarios |
| **Complexity** | One-line statement | Multi-step procedure |

---

## 🧪 The QA Brain Moment (Interview Check) 🧠
When an interviewer asks you to "Test a Pen," they are checking if you think in Scenarios:
* **Scenario 1:** Verify the pen writes on paper. (Positive)
* **Scenario 2:** Verify the pen doesn't leak at high altitudes. (Edge Case)
* **Scenario 3:** Verify the ink dries within 2 seconds. (Performance)

---

### 💡 One-Line Interview-Safe Answer:
**A Test Scenario defines the scope of what to test; a Test Case defines the steps to execute it.**

markdown
# 🧪 Test Scenario vs. Test Case
### The "What" vs. the "How" of professional testing.

---

## 🎯 Test Scenario (The Goal)
* **Definition:** A high-level description of what needs to be tested.
* **Format:** "Verify the [Feature] works under [Condition]."
* **Example:** "Verify the login works with valid credentials."

---

## 🧪 Test Case (The Steps)
* **Definition:** A detailed set of steps, data, and expected results.
* **Format:** Step-by-step instructions.
* **Example:** 1. Enter "admin@email.com" in the email field.
    2. Enter "12345" in the password field.
    3. Click "Login."
    4. Expected: User is redirected to the Dashboard.

---

## ⚔️ Comparison at a Glance
* **Scenario:** Broad and derived from requirements.
* **Test Case:** Specific and derived from scenarios.
* **Ratio:** 1 Scenario ➔ Many Test Cases (Positive, Negative, Edge).

---

### 💡 One-Line Lock-in:
**A Test Scenario defines the scope of what to test; a Test Case defines the steps to execute it.**
