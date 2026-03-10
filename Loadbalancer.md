# Technical Deep Dive: Load Balancing ⚖️

## 📌 Overview
In a distributed system, a **Load Balancer** acts as a "traffic cop" sitting in front of your servers and routing client requests across all servers capable of fulfilling those requests. It ensures that no single server bears too much demand.



---

## ☕ Real-Life Scenario: The "Viral" Coffee Shop
To understand how this works in production, let's look at a scaling coffee shop:

1.  **The Solo Barista (Single Server):** You open a shop with one barista. They take the order, brew the coffee, and serve it. It works great for 5 customers an hour.
2.  **The "Viral" Moment (Traffic Spike):** Suddenly, a food blogger posts about your shop. 500 people show up. The single barista crashes (burnout/downtime), and customers leave.
3.  **The Expansion (Horizontal Scaling):** You hire four more baristas.
4.  **The Greeter (The Load Balancer):** You place a staff member at the door. Their *only* job is to look at the baristas and point the next customer to the one who is currently free.

**The Result:** The workload is spread evenly, and if one barista needs a break (server maintenance), the shop continues to function perfectly.

---

## 🛠 Load Balancing Algorithms

| Strategy | Logic | Best For
