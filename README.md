# 🔒 Securing an Apache Web Server  

A hands-on security hardening project for Apache running on Ubuntu. This guide outlines how to strengthen server defenses, protect sensitive data, and prevent common attack vectors — ensuring a stable and secure web hosting environment.

---

## 📖 Table of Contents

- [🎯 Objective](#-objective)
- [🛠️ Tools Used](#-tools-used)
- [🧠 Skills Learned](#-skills-learned)
- [🚀 Project Workflow](#-project-workflow)
- [📊 Summary](#-summary)
- [📚 References](#-references)

## 🎯 Objective  

To proactively secure an Apache web server by applying proven security best practices, from firewall setup and directory restrictions to HTTPS implementation and log monitoring — building a reliable, attack-resilient environment for web services.

---

## 🛠️ Tools & Technologies  

- **Apache2** — Web server installation and configuration  
- **UFW (Uncomplicated Firewall)** — Server firewall configuration  
- **Certbot (Let’s Encrypt)** — Free SSL/TLS certificate issuance  
- **ModSecurity** — Web Application Firewall (WAF)  
- **Fail2Ban** — Protection against brute-force login attempts  
- **Ubuntu Server** — Linux distribution hosting the Apache service  

---

## 📚 Skills Learned  

- **Linux Server Administration**  
- **Web Server Security Configuration**  
- **Firewall Rule Management (UFW)**  
- **SSL/TLS Implementation with Let's Encrypt**  
- **Web Application Firewall (WAF) Setup**  
- **Attack Surface Reduction**  
- **Log Monitoring & Incident Detection**  
- **Best Practices for Apache Hardening**

---

## 🚀 Project Workflow  

### 📌 Step 1: Install Apache2  

Installed Apache2 web server via package manager.  

![Apache Installation](https://github.com/user-attachments/assets/94988259-0461-44de-b7ad-c5a0027821a9)

---

### 📌 Step 2: Configure UFW Firewall  

Configured UFW to allow necessary web traffic and block unauthorized access.

![UFW Configuration](https://github.com/user-attachments/assets/2917daef-2796-48d2-a045-b58855549541)

---

### 📌 Step 3: Disable Directory Listing  

Prevented file and folder listings via browser by setting:

![image](https://github.com/user-attachments/assets/e1b96fff-1598-41f8-b91a-426d9881e459)

---

### 📌 Step 4: Hide Apache Version and OS Info
Hid sensitive server information by setting:

ServerTokens Prod
ServerSignature Off

---

### 📌 Step 5: Install & Enable ModSecurity
Added a Web Application Firewall to block common web attacks like SQL injection.

![image](https://github.com/user-attachments/assets/a05bd0f1-d659-4318-be4b-e71f338755b6)

![image](https://github.com/user-attachments/assets/6773cccf-0af0-45ce-878c-48f7197bd7fc)

---

### 📌 Step 6: Enable HTTPS with SSL/TLS
Installed Certbot and obtained SSL certificates via Let’s Encrypt.

![image](https://github.com/user-attachments/assets/3ff8c9a4-bad5-4d3f-8fb0-c93525bcc1bf)

![image](https://github.com/user-attachments/assets/47044fd5-5e92-444d-9b4a-2dee319dfb63)

---

### 📌 Step 7: Regularly Monitor Server Logs
Reviewed Apache access and error logs to detect anomalies.

![image](https://github.com/user-attachments/assets/13c5a6d0-5a4d-4ed1-b62c-cd94978dbf3b)

---

## 📊 Summary
This project demonstrates proactive server hardening techniques for a public-facing web service, safeguarding against unauthorized access, data breaches, and common attacks. Essential for any cybersecurity analyst or system administrator looking to secure their Linux web infrastructure.


## 📚 References

- Apache Security Best Practices
- UFW Documentation
- Certbot for Let's Encrypt
- ModSecurity Handbook



🚀 Author: Manoj Mothukuru

