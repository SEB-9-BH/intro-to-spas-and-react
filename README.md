# Intro to SPAs and React
![](https://i.imgur.com/uoJvBRK.jpg)
Here’s a fully formed **Markdown** lesson you can use to teach SPAs and React fundamentals before introducing Vite.
It integrates the topics from your content outline and uses the provided diagram to explain how SPAs work in practice.

---

# **Introduction to SPAs and React**

Before we dive into building a React app with **Vite**, it’s important to understand **what React is**, how **Single Page Applications (SPAs)** work, and how React fits into the bigger picture of modern web development.

---

## **1. What is a SPA?**

**SPA** stands for **Single Page Application**.
Instead of the server sending a brand new HTML page for every request, the app loads **one main HTML file** and dynamically updates the content as the user interacts with it.

**Key Points:**

* The browser **does not reload** the entire page when you navigate.
* Content updates via **JavaScript** using **AJAX/HTTP** calls to get new data.
* Provides a **faster, app-like experience**.
* Common examples: Gmail, Twitter, Facebook.

**Benefits:**

* Faster navigation
* Better user experience
* Reduces server load

**Drawbacks:**

* Larger initial load time
* SEO challenges (but can be fixed with SSR/Pre-rendering)
* Requires JavaScript enabled

---

## **2. Core Technologies of SPAs**

SPAs rely on a combination of:

* **HTML** → Structure
* **CSS** → Styling
* **JavaScript** → Interactivity and data handling
* **AJAX / Fetch API** → Communicating with the server without page reloads
* **Routing libraries** → Manage URL changes without reloading the page

---

## **3. SPAs vs MPAs**

| Feature              | SPA (Single Page App) | MPA (Multi Page App)  |
| -------------------- | --------------------- | --------------------- |
| Page Reloads         | No                    | Yes                   |
| Speed                | Fast after first load | Slower                |
| SEO                  | Needs extra setup     | Better out of the box |
| Server Communication | Mostly via APIs       | Full page reloads     |
| Example              | Gmail                 | Amazon product pages  |

---

## **4. What is React?**

React is a **JavaScript library** for building **user interfaces**.
It is especially popular for SPAs because it efficiently updates only the parts of the page that change.

---

## **5. React Concepts**

* **Components**: Reusable, independent UI blocks (e.g., a button, a navbar).
* **JSX**: A syntax that lets you write HTML-like code inside JavaScript.
* **State Management**: A way to store and manage data that changes over time.
* **Virtual DOM**: A lightweight copy of the real DOM that React uses to decide what needs to update.
* **React Ecosystem**: Includes tools like React Router, Redux, and hooks for extending functionality.

---

## **6. Connecting the Diagram to SPAs and React**

![React Node Diagram](e5669901-57b7-4f71-b73d-8bcf839d0480.png)

### **Step-by-Step Explanation**

1. **The Visitor** opens the app in their browser.
2. **React Client Side**:

   * **Components**: Handle UI pieces like buttons, forms, or entire sections.
   * **Routing Components**: Let you change the "page" without refreshing the browser.
   * **Services (Fetch API)**: Used to request or send data to the backend via **AJAX/HTTP**.
3. **Node.js with Express Server**:

   * **Routes**: Define endpoints like `/api/users` or `/api/products`.
   * **Express**: Manages the server and handles incoming API requests.
4. **Database (MongoDB)**:

   * Stores and retrieves data requested by the client.
5. **Flow**:

   * React sends a request to Node.js (via AJAX/HTTP).
   * Node.js queries MongoDB and sends data back.
   * React updates the UI without reloading the page.

---

## **7. Why React + SPA Architecture Works Well**

* React’s **component model** keeps UI modular and maintainable.
* **Virtual DOM** makes updates faster.
* SPAs reduce unnecessary reloads, improving performance.
* Combined with **Node.js + Express + MongoDB**, you get a **full-stack JS application**.

---

## **8. Summary**

By the end of this section, you should:

* Understand **what SPAs are** and how they work.
* Know the **core technologies** behind SPAs.
* Be able to **compare SPAs vs MPAs**.
* Understand how **React fits** into the SPA architecture.
* Recognize how **frontend (React)** and **backend (Node/Express)** communicate with a database.

---

✅ **Next Step:** We will use **Vite** to quickly scaffold a new React SPA and begin building components.

