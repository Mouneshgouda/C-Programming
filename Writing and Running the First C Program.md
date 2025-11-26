# 🌐 Domain Name System (DNS)

The **Domain Name System (DNS)** is a hierarchical and decentralized naming system used to identify computers, services, and other resources connected to the Internet or private networks. It converts human-readable domain names (e.g., `google.com`) into machine-readable IP addresses (e.g., `142.250.191.46`).

---

## 🔑 Key Concepts

### **Domain Name Space**
DNS follows an **inverted-tree structure**, where each node is a domain.

- **Root (`.`)** – top of the hierarchy  
- **TLDs (Top-Level Domains)** – e.g., `.com`, `.org`, `.net`  
- **Second-Level Domains** – e.g., `google` in `google.com`  
- **Subdomains** – e.g., `mail.google.com`

### **DNS Resolution**
When a user enters a URL, a **DNS resolver** queries DNS servers to determine the matching IP address. This process is known as **name resolution**.

### **Types of DNS Records**
Common DNS records include:

- **A Record** – Maps a domain to an IPv4 address  
- **AAAA Record** – Maps a domain to an IPv6 address  
- **MX Record** – Specifies mail exchange servers for email  
- **CNAME Record** – Provides canonical names (aliases)

---

# 📧 Electronic Mail (Email)

Email is one of the most widely used Internet services, enabling users to exchange digital messages across networks.

---

## 📡 Key Email Protocols

### **SMTP (Simple Mail Transfer Protocol)**
- Used for **sending** email.
- Handles the transfer of mail from:
  - Sender’s email client → Sender’s mail server  
  - Sender’s mail server → Recipient’s mail server

### **POP3 (Post Office Protocol v3)**
- Used for **retrieving** email.
- Traditionally downloads messages and may **remove them from the server** after retrieval.

### **IMAP (Internet Message Access Protocol)**
- A more advanced protocol for mail retrieval.
- Allows email management **directly on the server**:
  - Folders  
  - Flags  
  - Partial or full message retrieval  
- Ideal for multi-device access.

---

# 📁 File Transfer Protocols

## **FTP (File Transfer Protocol)**
FTP is a standard network protocol used for transferring files between a client and a server on a network.

### 🔑 Key Features
- **Two Separate Connections**
  - **Control Connection**  
    Handles commands such as login, directory changes, etc.  
    Stays open for the duration of the FTP session.
  - **Data Connection**  
    Used for actual file transfers.  
    A new data connection is created each time a file is sent or received.

- **Authentication**  
  Usually requires a **username and password**, though **anonymous FTP** is also supported for public file sharing.

---

# 💻 World Wide Web (WWW) & HTTP

The **World Wide Web (WWW)** is an information system where resources are identified by **URLs**, connected by **hyperlinks**, and accessed via the Internet.

## **HTTP (Hypertext Transfer Protocol)**
HTTP is the underlying protocol for data communication on the web.

### 🔑 Key Concepts
- **Purpose**  
  Defines how messages are **formatted**, **transmitted**, and how servers and browsers respond to commands.

- **Client–Server Model**  
  A client (usually a browser) sends an **HTTP request**, and the server replies with an **HTTP response**.

- **Stateless Protocol**  
  Each request is treated independently.  
  Servers do not retain session information unless **cookies**, **sessions**, or **tokens** are used.

---

# 🛠️ Network Management

## **SNMP (Simple Network Management Protocol)**
SNMP is used for monitoring and managing devices on an IP network.

### 🔧 Components
- **Manager**  
  Central system used by administrators to oversee the network.

- **Agent**  
  Software running on each managed device that gathers information and responds to the manager.

- **Managed Device**  
  Routers, switches, servers, or other networked equipment being monitored.

### 📊 Function
SNMP enables:
- **Polling**: Managers request data from agents (e.g., interface status, bandwidth usage).  
- **Traps**: Agents send alerts to managers when critical events occur.

---

# 🔒 Security Protocols

## **PGP (Pretty Good Privacy)**
PGP is a widely used encryption system providing privacy and authentication for digital communications.

### 🔑 Capabilities
- **Signing**  
  Ensures message integrity and verifies the sender's identity.

- **Encryption**  
  Protects message contents, ensuring only the intended recipient can read them.

### 🔐 How It Works
PGP combines:
- **Public-key cryptography** → for secure key exchange  
- **Symmetric-key cryptography** → for efficient message encryption  

---
<img width="3999" height="1748" alt="image" src="https://github.com/user-attachments/assets/6f5fc14a-72f2-47b0-aa93-d4eb93c2f437" />

# 🔐 SSH (Secure Shell)

**SSH (Secure Shell)** is a cryptographic network protocol used to securely operate network services over an unsecured network.

## 🎯 Purpose
SSH is primarily used for:
- **Remote command-line login**
- **Remote command execution**
It replaces older insecure protocols like **Telnet** by providing strong encryption and authentication.

## 🔒 Security
SSH ensures secure communication through:
- **Public-key cryptography** for authenticating the remote machine.
- **User authentication** via:
  - Password  
  - Public/private key pair  
- **Encrypted communication**, protecting data from eavesdropping and tampering.

## 🧰 Applications
SSH can be used for:
- **Secure file transfer**:  
  - **SFTP (SSH File Transfer Protocol)**  
  - **SCP (Secure Copy Protocol)**
- **Running remote applications** safely
- **Tunneling and port forwarding**
- **Secure remote administration** of servers and network devices

---


