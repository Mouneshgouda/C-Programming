# Application Layer Topics

---

🌐 **Domain Name Space (DNS)**  
The Domain Name System (DNS) is a hierarchical and decentralized naming system for computers, services, or any resource connected to the Internet or a private network. It translates human-readable domain names (like google.com) into machine-readable IP addresses (like 142.250.191.46).

### Key Concepts:
**Domain Name Space (DNS in Internet):** This is the structure of the naming system, forming an inverted tree. At the top is the root, followed by Top-Level Domains (TLDs) (e.g., .com, .org, .net), then Second-Level Domains (e.g., google), and so on. Every node in the tree is a domain.

**Resolution:** When a user types a URL, a DNS Resolver queries DNS servers to find the corresponding IP address. This process is called name resolution.

**Types of DNS Records:** These store information about the domain, such as A records (IP address mapping), MX records (mail exchange servers), and CNAME records (canonical names/aliases).

---

📧 **Electronic Mail (Email)**  
Electronic mail is one of the most widely used network services. It allows users to send and receive messages electronically.

### Key Protocols:
**SMTP (Simple Mail Transfer Protocol):** This is the standard protocol used for sending email across the internet. It handles the transfer of mail from the sender's mail client to the sender's mail server, and then from the sender's mail server to the recipient's mail server.

**POP3 (Post Office Protocol version 3):** Used by a local email client to retrieve email from a remote server. Historically, it often downloaded and deleted the mail from the server.

**IMAP (Internet Message Access Protocol):** A more modern protocol for retrieving mail, which allows users to manage and access their email on the server (folders, flags, etc.) without downloading it entirely.

---

📁 **File Transfer Protocols**

**FTP (File Transfer Protocol)**  
FTP is a standard network protocol used to transfer computer files between a client and a server on a computer network.

### Key Feature: FTP uses two separate connections:
**Control Connection:** For sending commands (e.g., login, change directory). This remains open for the entire session.

**Data Connection:** For transferring the actual file data. This connection is established every time a file is transferred.

**Authentication:** FTP typically requires a username and password, though anonymous FTP is also possible.

---

💻 **World Wide Web (WWW) and HTTP**

The World Wide Web (WWW) is an information system where documents and other web resources are identified by URLs, interconnected by hypertext links, and can be accessed via the Internet.

### HTTP (Hypertext Transfer Protocol)
**Purpose:** It defines how messages are formatted and transmitted, and what actions Web servers and browsers should take in response to various commands.

**Client-Server Model:** The client (usually a web browser) sends an HTTP request to a server, and the server returns an HTTP response.

**Stateless:** By default, HTTP is stateless, meaning each request is treated independently, and the server doesn't remember previous requests. Cookies are used to maintain state.

---

🛠️ **Network Management**

### SNMP (Simple Network Management Protocol)
SNMP is a protocol used for managing and monitoring network devices and their functions on an IP network.

### Components:
**Manager:** The central station used by an administrator to monitor the network.

**Agent:** Software running on the managed device (router, server, switch) that collects information and communicates it to the manager.

**Managed Device:** The actual device being monitored.

**Function:** SNMP allows managers to poll agents for information (e.g., interface status, traffic statistics) or receive traps (alerts) from agents when a critical event occurs.

---

🔒 **Security Protocols**

### PGP (Pretty Good Privacy)
PGP is an encryption program that provides cryptographic privacy and authentication for data communication. It is often used for:

**Signing:** Verifying the integrity of the message and the identity of the sender.

**Encryption:** Ensuring only the intended recipient can read the message.

PGP uses a combination of public-key cryptography (for key exchange) and symmetric-key cryptography (for message encryption).

---
<img width="3999" height="1748" alt="image" src="https://github.com/user-attachments/assets/74658c00-b79e-4abf-b96c-f095f3b1595b" />


🔐 **SSH (Secure Shell)**
SSH is a cryptographic network protocol for operating network services securely over an unsecured network.

**Purpose:** It is primarily used for remote command-line login and remote command execution, replacing insecure protocols like Telnet.

**Security:** SSH uses public-key cryptography for authenticating the remote computer and optionally allows the user to be authenticated using a password or public-key. All communications are encrypted.

**Applications:** Secure file transfer (SFTP/SCP), running remote applications.
