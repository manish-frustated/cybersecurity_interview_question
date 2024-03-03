# Cybersecurity Interview question




## Vulnerability Assessment vs. Penetration Testing:

```bash
  Vulnerability Assessment: Identifies and quantifies vulnerabilities in a system. It involves scanning the system for known vulnerabilities.
  Example: Using tools like Nessus to scan a network for known vulnerabilities in software

  Penetration Testing: Simulates real-world attacks to exploit vulnerabilities. It aims to determine the extent to which an attacker can gain unauthorized access.
  Example: Ethical hackers attempting to exploit vulnerabilities in a web application to gain access to sensitive data.
```

## DNS (Domain Name System) and DNS Enumeration:

```bash
  DNS: Translates domain names into IP addresses, allowing users to access websites using human-readable names.
  
  DNS Enumeration: Involves querying DNS servers to gather information about a target network. Attackers use this to map out network infrastructure, identify servers, and plan attacks.
  Example: Using tools like dnsenum to discover subdomains of a target domain.
```

## SSL and TLS:

```bash
  SSL (Secure Sockets Layer) and TLS (Transport Layer Security): Protocols that ensure secure communication over a network by encrypting data transmission.
```

## Shodan:

```bash
  Shodan: A search engine for internet-connected devices. It allows users to find specific types of computers, routers, servers, and other devices connected to the internet.
  Example: Finding all webcams connected to the internet with default passwords using Shodan.
```

## GitHub and GitHub Dorking:

```bash
  GitHub: A platform for hosting and sharing code repositories.
  
  GitHub Dorking: Searching GitHub repositories using advanced search techniques to find sensitive information such as passwords, API keys, or proprietary code.
  Example: Searching for passwords in code repositories using specific search queries like password filetype:yaml.
```

## Subdomain Enumeration:

```bash
  Subdomain: A subdivision of a domain. For example, "mail.example.com" is a subdomain of "example.com".
  
  Subdomain Enumeration: Involves finding subdomains associated with a domain, which can reveal additional attack surfaces for exploitation.
  Example: Using tools like Sublist3r to discover subdomains of a target domain.
```

## Google Dorking:

```bash
  Google Dorking: Using advanced search operators to find sensitive information indexed by Google, such as login pages, exposed databases, or confidential documents.
  Example: Searching for publicly accessible documents containing confidential information using specific search queries like filetype:pdf "confidential".
```

## SMB:

```bash
 SMB (Server Message Block): It's a network protocol used by computers mainly for sharing files, printers, and other resources.
 
 How Attackers Use SMB Enumeration: Attackers can use SMB enumeration to gather information about a network, like finding out what devices are connected, what shares are available, or even usernames and passwords. This helps them plan a targeted attack. For example, if they find a share with sensitive information, they might try to gain access to it using the information they gathered through enumeration.

```

## SNMP (Simple Network Management Protocol):

```bash
SNMP is a protocol used to manage and monitor network devices like routers, switches, and servers.

Attackers can use SNMP for enumeration, which means gathering information about the network. For example, they might use SNMP to find out what devices are connected to the network, their configurations, and potentially sensitive information like passwords if it's configured insecurely.
```

## SMTP (Simple Mail Transfer Protocol):

```bash
SMTP is a protocol used for sending and receiving email.

Attackers can use SMTP for enumeration by trying to gather information about email addresses, server configurations, and potentially exploiting vulnerabilities in email servers. For example, they might use SMTP commands to query a mail server for a list of valid email addresses or to test for open relays that could be used for spamming or sending malicious emails.
```

