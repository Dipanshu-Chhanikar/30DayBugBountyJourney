# 🐞 Bug Bounty Journey – Day 2 

---

## 🎯 Objective
Begin mastering **Cross-Site Scripting (XSS)** vulnerabilities by learning the theory, watching real-world demos, and solving hands-on labs from PortSwigger Academy.

---

## 🎥 Learning Summary

- Watched [**XSS Vulnerabilities – NahamSec**](https://www.youtube.com/watch?v=u8zKkQ1VTMI), which explained:
  - Different types of XSS (Reflected, Stored, DOM-based)
  - Real-world exploitation techniques
  - Common HTML/JS injection points

- Watched [**DOM XSS Explained – InsiderPhD**](https://www.youtube.com/watch?v=-6uPHcLj4oU), which covered:
  - What DOM XSS is and how it differs from reflected XSS
  - The concept of sources and sinks
  - How JavaScript handles and processes user-controlled input

- Watched [**Live Bug Bounty Demo – XSS in Real Target**](https://www.youtube.com/watch?v=ecuiE83zvqY), which showed:
  - How to identify input points and test payloads
  - Tips for finding XSS in modern JS-heavy apps
  - Using Burp Suite effectively to test for XSS

---

## 🧪 Labs Explored

### ✅ PortSwigger Web Security Academy
- [Reflected XSS in HTML context with nothing encoded](https://portswigger.net/web-security/cross-site-scripting/reflected/lab-html-context-nothing-encoded)
- [Bypassing CSP to exploit XSS](https://portswigger.net/web-security/cross-site-scripting/content-security-policy/lab-csp-bypass)
- [DOM-based XSS in a JavaScript framework](https://portswigger.net/web-security/cross-site-scripting/dom-based/lab-dom-xss-reflected)
- [Reflected XSS overview](https://portswigger.net/web-security/cross-site-scripting/reflected)

### ✅ Additional Resource
- [Using Burp Suite to manually test for reflected XSS](https://portswigger.net/support/using-burp-to-manually-test-for-reflected-xss)

---

## 🧰 Tools Used and Practiced

| Tool / Extension     | Purpose                                          |
|----------------------|--------------------------------------------------|
| **Burp Suite**       | Intercept and modify requests for XSS testing    |
| **Google Chrome**    | Inspect DOM and observe JavaScript behavior      |
| **HackTools**        | Quickly inject XSS payloads                      |
| **FoxyProxy**        | Switch proxy modes while browsing                |

---

## 🧠 What I Learned

- The **difference between Reflected, Stored, and DOM-based XSS**.
- How **HTML injection context** impacts whether a payload executes.
- DOM-based XSS occurs when **JavaScript processes user input directly**, without proper sanitization.
- CSP (Content Security Policy) is a security layer that can be bypassed if misconfigured — learned how to test those bypasses.
- How to **identify JavaScript sources (e.g., `location`, `document.referrer`) and sinks (e.g., `innerHTML`, `eval`)** in web applications.
- How to manually test XSS using **Burp Suite**, inspect server responses, and inject payloads to trigger JavaScript execution.
