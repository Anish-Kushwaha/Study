# 🔐 Security Policy

This document outlines the security practices, reporting process, and responsibilities related to the **FocusRoom – CISCE Boards 2026 Study Platform**.

FocusRoom is a **client-side, browser-based application** with no backend services. Even so, security and responsible disclosure are taken seriously.

---

## 📌 Scope

This security policy applies to:

- The FocusRoom web application
- The public repository hosted on GitHub
- The live deployment at:
  https://anish-kushwaha.github.io/Study

It does **not** apply to:
- Third-party libraries or CDNs used (Font Awesome, Google Fonts)
- User devices or browsers
- GitHub infrastructure itself

---

## 🧠 Architecture Overview (Security Context)

FocusRoom is designed with a **minimal attack surface**:

- Single-file application (`index.html`)
- No backend server
- No databases
- No authentication system
- No user accounts
- No cookies
- No external APIs (except static assets)

All logic executes **locally in the user’s browser**.

---

## 🔒 Data Handling & Privacy

FocusRoom prioritizes user privacy by design.

### ✅ What the app DOES
- Stores study data locally using `localStorage`
- Keeps all timer, goal, and session data on the user’s device

### ❌ What the app DOES NOT do
- Collect personal information
- Transmit data to servers
- Track users
- Use analytics or telemetry
- Store passwords or credentials

All stored data is:
- Non-sensitive
- Local-only
- Fully controllable by the user

---

## 🛡 Security Measures Implemented

- No remote code execution
- No form submissions
- No user input sent over the network
- No authentication logic (eliminates auth-related vulnerabilities)
- No dynamic script injection from user input
- Static asset loading from trusted CDNs only

The simplicity of the architecture significantly reduces common web vulnerabilities such as:
- SQL Injection
- Authentication bypass
- Server-side request forgery (SSRF)
- Data breaches

---

## ⚠️ Known Limitations

Because FocusRoom is a **client-only application**:

- Data stored in `localStorage` can be cleared by the user
- Data is not encrypted (non-sensitive by design)
- Security depends partially on the user’s browser environment

These limitations are **intentional trade-offs** for simplicity and privacy.

---

## 🐞 Reporting a Vulnerability

If you discover a security vulnerability, please report it responsibly.

### 📧 How to Report
Send an email with details to:

**Anish-Kushwaha@zohomail.in**

### 📝 Include the following:
- Description of the vulnerability
- Steps to reproduce
- Affected file or section (if known)
- Potential impact
- Screenshots or proof-of-concept (if available)

Please **do not** disclose vulnerabilities publicly before they are reviewed.

---

## ⏳ Response Timeline

- Initial acknowledgment: within **48 hours**
- Investigation and validation: **as soon as possible**
- Fix or mitigation: based on severity

Since this is a personal/educational project, response times may vary, but all valid reports are taken seriously.

---

## 🚫 Out-of-Scope Issues

The following are **not considered security vulnerabilities**:

- UI/UX issues
- Feature requests
- Performance optimizations
- Browser-specific rendering issues
- Vulnerabilities in third-party services outside this repository

---

## 📜 Responsible Disclosure

Security researchers are encouraged to follow responsible disclosure practices.

Please:
- Avoid exploiting vulnerabilities
- Avoid accessing or modifying user data
- Allow time for fixes before public disclosure

---

## 📅 Policy Updates

This security policy may be updated as the project evolves.

Last updated: **2025**

---

## 👤 Maintainer

**Anish Kushwaha**  
Student • Developer • Cybersecurity Enthusiast  

Email: Anish-Kushwaha@zohomail.in  
GitHub: https://github.com/Anish-Kushwaha

---

## ⚖️ Disclaimer

This project is provided **“as is”**, without warranty of any kind.

The author is not responsible for misuse, data loss, or damages arising from the use of this software.
