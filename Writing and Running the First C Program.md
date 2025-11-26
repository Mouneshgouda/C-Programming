# 🌐 Application Layer Topics

This document provides a concise overview of key **Application Layer protocols and services**.

---

## **Domain Name Space (DNS)**

The **Domain Name System (DNS)** is a hierarchical and decentralized naming system used to translate human-readable domain names (like `google.com`) into machine-readable IP addresses (like `142.250.191.46`).

### **Key Concepts**
- **Domain Name Space:**  
  The DNS structure is an inverted tree:
  - **Root**
  - **Top-Level Domains (TLDs):** `.com`, `.org`, `.net`
  - **Second-Level Domains:** e.g., `google`, `amazon`
  - Each node represents a domain.

- **Resolution:**  
  When a user types a URL, a **DNS Resolver** queries DNS servers to find the correct IP address.

- **DNS Records:**  
  - **A Record:** Maps domain to IPv4 address  
  - **MX Record:** Mail exchange server information  
  - **CNAME Record:** Canonical name/alias for a domain

---

## 📧 **Electronic Mail (Email)**

Email allows sending and receiving electronic messages.

### **Key Protocols**
- **SMTP (Simple Mail Transfer Protocol):** Sends emails from client to server and between servers.
- **POP3 (Post Office Protocol v3):** Retrieves email from a server (often downloads and deletes emails).
- **IMAP (Internet Message Access Protocol):** Manages emails on the server, allowing synchronized access across devices.

---

## 📁 **File Transfer Protocols**

### **FTP (File Transfer Protocol)**
Used to transfer files between a client and server.

#### **Key Features**
- **Two Connections:**
  - **Control Connection:** Sends commands, stays open during session.
  - **Data Connection:** Transfers files, created per transfer.
- **Authentication:** Usually requires a username/password; **anonymous FTP** is also supported.

---

## 💻 **World Wide Web (WWW) and HTTP**

### **WWW**
A system of interlinked documents and resources, accessed via URLs.

### **HTTP (Hypertext Transfer Protocol)**
- **Purpose:** Defines communication between web clients and servers.
- **Client-Server Model:** Browser sends a request → Server returns a response.
- **Stateless:** Each request is independent; **cookies** maintain session info.

---

## 🛠️ **Network Management**

### **SNMP (Simple Network Management Protocol)**
Used to manage and monitor network devices.

#### **Components**
- **Manager:** Central monitoring system.
- **Agent:** Software on device collecting data.
- **Managed Device:** Router, switch, server, etc.

#### **Function**
- Poll agents for data (e.g., traffic, status)  
- Receive **traps** (alerts) for critical events

---

## 🔒 **Security Protocols**

### **PGP (Pretty Good Privacy)**
Provides encryption and authentication for secure communication.

#### **Functions**
- **Signing:** Ensures integrity and sender identity.
- **Encryption:** Ensures only the intended recipient can read the message.

Uses:
- **Public-key cryptography** for key exchange  
- **Symmetric-key cryptography** for message encryption

---
<img width="3999" height="1748" alt="image" src="https://github.com/user-attachments/assets/22005584-99e7-4975-bd7e-1dd62202c0f7" />


## 🔐 **SSH (Secure Shell)**

SSH is a secure protocol for remote access and command execution.

### **Purpose**
- Replaces insecure protocols like Telnet  
- Encrypts all transmitted data

### **Security**
- Host authentication via **public-key cryptography**  
- User authentication via password or key

### **Applications**
- Remote command-line login  
- Secure file transfer (SFTP/SCP)  
- Running remote applications
