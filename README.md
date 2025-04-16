<!-- markdownlint-disable MD033 -->
# Cyber Security Notes

**Welcome to My personal CyberSecurity Notes! This repository is a curated collection of `concepts`, `explanations`, `real-world examples`, and `best practices` related to `cybersecurity`.**

## Table of Content

| No | Section                                     | Sub-Section |
|----|---------------------------------------------|-------------|
| 1  | [**Governance & Regulation in Cybersecurity**](#governance--regulation-in-cybersecurity) |  a. [**Important Terminologies**](#important-terminologies)<br> b. [**What is Cybersecurity Governance?**](#what-is-cybersecurity-governance)<br> c. [**Key Components of Cybersecurity Governance**](#key-components-of-cybersecurity-governance)<br> d. [**Cybersecurity Regulations & Laws**](#cybersecurity-regulations--laws)<br> e. [**Real-World Example of Governance & Regulation**](#real-world-example-of-governance--regulation)<br> f. [**Tools & Frameworks for Governance**](#tools--frameworks-for-governance)<br> g. [**Summary Notes**](#summary-notes) |
| 2  | [**Cyber Kill Chain**](#cyber-kill-chain)   |  a. [**Reconnaissance**](#1-reconnaissance-target-identification)<br> b. [**Weaponization**](#2-weaponization-creating-payload)<br> c. [**Delivery**](#3-delivery-delivering-the-payload)<br> d. [**Exploitation**](#4-exploitation-triggering-the-exploit)<br> e. [**Installation**](#5-installation-installing-malware)<br> f. [**Command and Control**](#6-command-and-control-c2)<br> g. [**Actions on Objectives**](#7-actions-on-objectives-final-goal-achieved)<br> h. [**Kill Chain Summary Table**](#kill-chain-summary-table)<br> i. [**Realistic Scenario in Flow**](#realistic-scenario-in-flow) |
| 3  | [**Cybersecurity Principles**](#cybersecurity-principles) |  a. [**CIA Triad**](#1-cia-triad-core-security-principles)<br> b. [**DAD Triad**](#2-dad-triad-attackers-goals)<br> c. [**Defense-in-Depth**](#3-defense-in-depth)<br> d. [**Fundamental Concepts of Security Models**](#4-fundamental-concepts-of-security-models)<br> e. [**ISO/IEC 19249**](#5-isoiec-19249)<br> f. [**Zero Trust vs Trust but Verify**](#6-zero-trust-vs-trust-but-verify)<br> g. [**Threat vs Risk**](#7-threat-vs-risk)<br> h. [**Summary Notes (Quick Reference Table)**](#summary-notes-quick-reference-table) |

## Governance & Regulation in Cybersecurity

### Important Terminologies

- **`Governance`:**
  
  - Managing and directing an organisation or system to achieve its objectives and ensure compliance with laws, regulations, and standards.

- **`Regulation`:**
  
  - A rule or law enforced by a governing body to ensure compliance and protect against harm.

- **`Compliance`:**
  
  - The state of adhering to laws, regulations, and standards that apply to an organisation or system.

### What is Cybersecurity Governance?

- Cybersecurity governance is the `framework` used by organizations to manage and direct their security efforts. It ensures that:

  - Cybersecurity aligns with business goals

  - Risks are identified and managed

  - Policies, roles, and responsibilities are clearly defined

  - Legal and regulatory compliance is maintained

## Key Components of Cybersecurity Governance

| **Component**          | **Description**                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| **`Policies` & `Standards`**   | Define how the organization protects data and systems (e.g., password policies, encryption standards). |
| **`Risk Management`**        | Identifies, assesses, and prioritizes cybersecurity risks.                 |
| **`Roles` & `Responsibilities`** | Assigns responsibilities (CISO, IT Admin, Security Analyst, etc.).       |
| **`Monitoring` & `Reporting`** | Ensures continuous oversight and improvement of security controls.         |
| **`Incident Response Plan`** | Guides how to respond to cyber incidents effectively.                      |

## Cybersecurity Regulations & Laws

### Global Regulations

| **Law/Framework**   | **Purpose**                                                                                     |
|-----------------------|---------------------------------------------------------------------------------------------|
| **`GDPR` (`EU`)**             | General Data Protection Regulation: Protects personal data and privacy of EU citizens. Heavy fines for data breaches. |
| **`HIPAA` (`USA`)**           | Protects health information in the healthcare sector.                                      |
| **`PCI-DSS`**               | For organizations handling credit card data (banks, payment processors).                   |
| **`NIST Framework` (`USA`)**  | National Institute of Standards and Technology: A security guideline followed by government and private companies. |

### Indian Cybersecurity Regulations

| **Law/Policy**            | **Description**                                                                 |
|---------------------------|---------------------------------------------------------------------------------|
| **`IT Act 2000`**               | Main cyber law in India. Covers hacking, identity theft, cyber terrorism, etc.  |
| **`CERT-In Guidelines` (`2022`)** | Indian Computer Emergency Response Team mandates breach reporting within 6 hours.|
| **`Data Protection Act` (`2023`)**| Aims to safeguard personal data and privacy of Indian citizens (inspired by GDPR).|
| **`Digital India Initiatives`** | Promotes cybersecurity in e-Governance, digital banking, and Aadhaar systems.   |

## Real-World Example of Governance & Regulation

- Let’s say **`"SecureBank Ltd."`** is a digital bank in India.

- 👨‍💼 **`Governance`:**

  - The **`CISO`** sets a policy: All customer data must be encrypted and stored in India.

  - A risk assessment shows their mobile app backend is vulnerable.

  - Security team is assigned responsibility to fix it within 30 days.

- 📜 **`Regulation`:**

  - They follow **`CERT-In rules`** and must report any data breach within **`6 hours`**.

  - They must comply with **`Data Protection Act 2023`** ensuring customers can delete or correct their data.

  - Their credit card processing must meet **`PCI-DSS standards`**.

## Tools & Frameworks for Governance

| **Tool/Framework**     | **Usage**                                                                                   |
|-------------------------|---------------------------------------------------------------------------------------------|
| **`ISO/IEC 27001`**          | International standard for managing information security                                     |
| **`NIST CSF`**               | Risk management and cybersecurity best practices                                            |
| **`COBIT`**                  | Governance framework for IT management                                                      |
| **`SOC 2`**                  | Audit standard for service providers handling data                                          |

### Summary Notes

- **`Cybersecurity governance`** = Strategy + policies + roles for secure operations.

- **`Regulation`** = Laws enforced by governments to protect user data and systems.

- Real-world organizations must follow both internal policies (governance) and external laws (regulation).

- Non-compliance can result in **`hefty fines`**, **`loss of reputation`**, or even **`legal action`**.

## Cyber Kill Chain

- The **`Cyber Kill Chain`** — a concept developed by **`Lockheed Martin`** in `2011`.

- The **`Cyber Kill Chain`** is a **`framework`** that outlines the steps adversaries follow to launch and execute a `cyberattack`. It helps defenders identify and stop attackers at various stages.

### **1. `Reconnaissance` (`Target Identification`)**

- **`What happens`:**

  - The attacker gathers information about the target organization (**`OSINT`**, **`social media`**, **`employee info`**, **`tech stack`**)

- **`Real-World Example`:**

  - Attacker searches for examplecorp.com on:

  - LinkedIn (employee names, job titles)

  - Shodan (open servers and devices)

  - Google Dork:
  
    ```bash
    site:examplecorp.com filetype:pdf
    ```

  - Finds exposed `PDF documents` with `employee emails` and `internal IPs`.

- **`Defender Tip`:** Monitor for unauthorized scanning and public exposure of internal docs.

### **2. `Weaponization` (`Creating Payload`)**

- **`What happens`:**

  - The attacker crafts a **`weaponized payload`** using an exploit + a backdoor or malware.

- **`Real-World Example`:**

  - Attacker creates a malicious **`PDF file`** that uses an old Adobe Reader vulnerability to run a reverse shell.

- **`Defender Tip`:** Use `sandboxing` and `antivirus` to detect crafted payloads before they execute.

### **3. `Delivery` (`Delivering the Payload`)**

- **`What happens`:**
  
- The attacker delivers the payload via:

  - Email (phishing)

  - USB drops

  - Malicious websites

  - Drive-by downloads

- **`Real-World Example`:**

  - A **`phishing email`** is sent to an employee pretending to be HR with a subject: **`"Salary Hike Details - March 2025"`**

  - Attached **`PDF`** has the exploit from **`Step 2`**.

- **`Defender Tip`:** Train employees to recognize phishing. Use email filters and spam protection.

### **4. `Exploitation` (`Triggering the Exploit`)**

- **`What happens`:**
  
  - Once the victim opens the payload, the exploit runs and executes the attacker's code.

- **`Real-World Example`:**

  - Employee opens the malicious `PDF`.

  - **`Exploit triggers`**, runs a **`reverse shell`**:

  - Attacker gets **`low-privileged access`** to the **`user’s system`**.

- **`Defender Tip`:** Keep software patched. Use **`endpoint detection` (`EDR`)**.

### **5. `Installation` (`Installing Malware`)**

- **`What happens`:**
  
  - Attacker installs **`malware` (`backdoor`, `keylogger`, `trojan`)** to maintain access.

- **`Real-World Example`:**

  - Attacker installs **`Cobalt Strike Beacon`** or **`Netcat listener`** for **`persistence`**:
  
  ```bash
  nc -nlvp 4444
  ```

- **`Defender Tip`:** Monitor `registry changes`, `startup scripts`, and use `behavior-based detection`.

### **6. `Command and Control` (`C2`)**

- **`What happens`:**
  
  - The attacker establishes communication with the victim's system to send commands and receive stolen data.

- **`Real-World Example`:**

  - Infected system pings a remote `C2` server every 10 seconds via HTTP.

  - Attacker sends command to **`escalate privileges`** or **`download more malware`**.

- **`Defender Tip`:** Monitor `outbound traffic` for connections to `unusual domains` or `IPs`.

### **7. `Actions on Objectives` (`Final Goal Achieved`)**

- **`What happens`:**
  
- Attacker performs the intended objective:

  - **`Data theft`**

  - **`Destroy systems`**

  - **`Ransomware attack`**

  - **`Lateral movement`**

- **`Real-World Example`:**

  - Attacker uses stolen credentials to access the `finance department server`.

  - `Exfiltrates` payroll data and sends to external server.

- **`Defender Tip`:** Use file `integrity monitoring`, `DLP systems`, and `role-based access control`.

### Kill Chain Summary Table

| **Stage**                      | **Attacker's Action**      | **Real-World Example**                   | **Defense**                          |
|--------------------------------|----------------------------|------------------------------------------|--------------------------------------|
| **`1. Reconnaissance`**        | **`Gather info`**          | **`Google`, `LinkedIn`, `Shodan`**       | **`OSINT monitoring`**               |
| **`2. Weaponization`**         | **`Create payload`**       | **`Malicious PDF with exploit`**         | **`Sandbox`, `signature detection`** |
| **`3. Delivery`**              | **`Send payload`**         | **`Phishing email`**                     | **`Email filters`, `training`**      |
| **`4. Exploitation`**          | **`Trigger exploit`**      | **`PDF opens reverse shell`**            | **`Patching`, `EDR`**                |
| **`5. Installation`**          | **`Install malware`**      | **`Cobalt Strike beacon`**               | **`Behavior detection`**             |
| **`6. Command & Control`**     | **`Remote control`**       | **`C2 via HTTP to attacker server`**     | **`Monitor outbound traffic`**       |
| **`7. Actions on Objectives`** | **`Final impact`**         | **`Data exfiltration`**                  | **`DLP`, `logging`, `SIEM`**         |

### Realistic Scenario in Flow

- Attacker identifies target `John@company.com` on LinkedIn (`Recon`).

- Crafts a PDF with an exploit and backdoor (`Weaponization`).

- Sends a phishing email (`Delivery`).

- John opens it, exploit runs (`Exploitation`).

- Malware installs, persists (`Installation`).

- Machine connects to attacker’s C2 server (`C2`).

- Attacker steals sensitive internal financial reports (`Objectives`).

## Cybersecurity Principles

### **1. `CIA Triad` (`Core Security Principles`)**

- **`What is it?`**
  
- A foundational model for ensuring information security. It stands for:

  - **`C`onfidentiality**
  
  - **`I`ntegrity**

  - **`A`vailability**

- **`Real-World Examples`:**

### CIA Triad Table

| **Principle**         | **Meaning**                                      | **Example**                                                                 |
|-----------------------|--------------------------------------------------|-----------------------------------------------------------------------------|
| **`Confidentiality`** | Only authorized people can access data           | Bank encrypts your account details; attacker cannot read your ATM PIN       |
| **`Integrity`**       | Data should not be tampered with                 | Tamper-proof logs in a healthcare system; no one can alter patient records  |
| **`Availability`**    | Systems/data should be accessible when needed    | Google services (Gmail, Drive) must be available 24/7; DDOS protection ensures this |

### **2. `DAD Triad` (`Attacker’s Goals`)**

- While **`CIA`** is from the **`defender’s side`**, **`DAD`** is from the **`attacker’s view`**:

  - **`D`isclosure (`breaking confidentiality`)**

  - **`A`lteration (`breaking integrity`)**

  - **`D`estruction/`D`enial (`breaking availability`)**

- **`Example`:**

  - Attacker `leaks passwords` → **`Disclosure`**

  - `Modifies` a company invoice → **`Alteration`**

  - Launches `DDoS` on a website → **`Denial`**

### **3. `Defense-in-Depth`**

- **`What is it?`**
  
- A layered security strategy where multiple controls are in place so if one fails, others still protect the system.

- **`Real-World Example`:**
  
  - Let’s say you're protecting a data center:

  - **`Physical Security`** – **`Security guards`, `keycards`**

  - **`Network Security`** – **`Firewalls`, `IDS`/`IPS`**

  - **`System Security`** – **`Antivirus`, `EDR tools`**

  - **`Access Control`** – **`Role-based access`**

  - **`Encryption`** – **`For stored and transmitted data`**

  - **`Monitoring`** – **`SIEM`, `alert systems`**

- Even if an attacker breaks in at one level, other levels still stop or detect the threat.

### **4. `Fundamental Concepts of Security Models`**

- Security models are theoretical frameworks used to design secure systems

### Security Models Table

| **Model**                            | **Focus**                     | **Real-Life Example**                                                      |
|--------------------------------------|-------------------------------|----------------------------------------------------------------------------|
| **`Bell-LaPadula`**                  | Confidentiality only          | Military systems where data classification matters (Top Secret, Secret, Confidential) |
| **`Biba Model`**                     | Integrity                     | Medical databases to prevent doctors from altering lab results             |
| **`Clark-Wilson`**                   | Commercial integrity          | Banking systems ensuring only approved transactions are allowed            |
| **`Brewer-Nash (Cinderella Model)`** | Prevent conflict of interest  | Legal firms can't let lawyers access two competing client cases            |

### **5. `ISO/IEC 19249`**

- **`What is it?`**
  
- This standard defines **`five architectural design principles`** for secure systems:

  1. Security Policy Enforcement

  2. Security Function Isolation

  3. Least Privilege

  4. Secure Defaults

  5. Open Design

- **`Example`:**
  
- A `banking app` following these principles:

  - Gives minimum access to each user role (e.g., teller vs manager)

  - Logs every transaction (Policy Enforcement)

  - Runs critical functions in isolated containers (Isolation)

### **6. `Zero Trust vs Trust but Verify`**

- **`Trust but Verify` (`Old Model`):**
  
  - Once you’re inside the network, you're `trusted`.

- **`Example`:**

  - **`Employee connects to company Wi-Fi`** → **`Gets access to file servers without re-authentication`**.

- **`Problem`:** If attacker gains internal access, they can move laterally without being stopped.

- **`Zero Trust` (`Modern Model`):**

- **`“Never trust, always verify.”`**
  
- Even inside the network, you must authenticate and authorize every time.

- **`Real-World Example`:**
  
  - **`Google`** uses **`BeyondCorp` (`Zero Trust model`)**.

- If you access `Gmail` on your work laptop, it checks:

  - **`Device health`**

  - **`User identity`**

  - **`Geo-location`**

  - **`Then allows access`**

- **`Zero Trust`** = **`Verification at every layer`**

### **7. `Threat vs Risk`**

### Threat vs Risk Table

| **Term**     | **Definition**                                      | **Real-Life Example**                                       |
|--------------|----------------------------------------------------|--------------------------------------------------------------|
| **`Threat`** | Potential danger (attacker or event)               | Phishing email, malware, disgruntled employee                |
| **`Risk`**   | The impact if a threat exploits a vulnerability    | If phishing succeeds, attacker gets access to finance system |

- **`Formula`:**
  
- **`Risk`** = **`Threat`** × **`Vulnerability`** × **`Impact`**

- **`So`:**

  - **`No vulnerability`** = **`No risk` (`even if threat exists`)**

  - **`No threat`** = **`No risk` (`even if you have a vulnerability`)**

### Summary Notes (Quick Reference Table)

| **Principle**           | **Description**                                                        | **Example**                                   |
|-------------------------|------------------------------------------------------------------------|-----------------------------------------------|
| **`CIA`**               | **`Core principles` (`Confidentiality`, `Integrity`, `Availability`)** | **`Bank account info`**                       |
| **`DAD`**               | **`Attacker goals` (`Disclosure`, `Alteration`, `Denial`)**            | **`Data leak`, `tampering`, `DDoS`**          |
| **`Defense-in-Depth`**  | **`Layered security model`**                                           | **`Physical` + `network` + `access control`** |
| **`Security Models`**   | **`Theoretical security designs`**                                     | **`Bell-LaPadula`, `Biba`, `Clark-Wilson`**   |
| **`ISO/IEC 19249`**     | **`Design principles for secure architecture`**                        | **`Least Privilege`, `Secure Defaults`**      |
| **`Zero Trust`**        | **`Never trust`, `always verify`**                                     | **`Google BeyondCorp`**                       |
| **`Threat vs Risk`**    | **`Threat = attacker/event`, `Risk` = `damage`**                       | **`Phishing email` vs `stolen credentials`**  |
