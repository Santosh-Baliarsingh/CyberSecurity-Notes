<!-- markdownlint-disable MD033 -->
# Penetration Tester

## Table of Content

| No | Section                                     | Sub-Section |
|----|---------------------------------------------|-------------|
| 1  | [**Penetration Testing Fundamentals**](#penetration-testing-fundamentals) |  a. [**What is Penetration Testing?**](#what-is-penetration-testing)<br> b. [**Penetration Testing Ethics**](#penetration-testing-ethics)<br> c. [**Key Ethical Principles**](#key-ethical-principles) |
| 2  | [**Penetration Testing Methodologies**](#penetration-testing-methodologies) |  |
| 4  | [**Types of Penetration Testing**](#types-of-penetration-testing) | a. [**Penetration Testing Scenarios Table**](#penetration-testing-scenarios-table) |
| 5  | [**Popular Tools Used in Pentesting**](#popular-tools-used-in-pentesting) |  a. [**Summary**](#summary) |

## Penetration Testing Fundamentals

## What is Penetration Testing?

- **`Penetration Testing` (also known as `Ethical Hacking`)** is a **`controlled and authorized attack`** simulation performed by **`cybersecurity professionals`** to **`identify vulnerabilities in systems, networks, or applications`** before malicious hackers can exploit them.

  - It is part of a broader security assessment strategy and provides practical insight into **`how secure a system really is`**.

  - The goal is not just to **`find vulnerabilities`**, but to **`assess the impact, prioritize risks, and recommend remediation`** steps.

- **`Real-life analogy`:** Imagine a company hires a professional burglar to break into their building — not to steal anything, but to check if their doors, windows, cameras, and alarms are secure enough.

## Penetration Testing Ethics

- Penetration Testing is performed **`legally and ethically`** with strict guidelines and moral responsibilities. Here's what ethical behavior in pentesting looks like:

### Key Ethical Principles

| **Principle**                 | **Description**                                                                                                                         |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| **`Authorization`**           | Always obtain **`written permission` (`scope of work`)** from the system owner before performing any tests.                             |
| **`Confidentiality`**         | All findings and sensitive data during the test must be kept **`confidential`**. No data should be leaked, shared, or reused elsewhere. |
| **`Non-Destructive Testing`** | The test must not cause **`system downtime`, `data loss`, or `service disruptions`** unless explicitly allowed.                         |
| **`Integrity in Reporting`**  | Reports should be **`accurate`, `honest`, and `objective`,** regardless of how the test went.                                           |
| **`No Personal Gain`**        | An ethical hacker should **`never exploit`** a vulnerability for personal benefit.                                                      |

- **Without a signed agreement or contract, any testing is considered `illegal hacking` (`a criminal offense`)**.

## Penetration Testing Methodologies

- Penetration Testing isn't done randomly — professionals follow **`established methodologies`** to ensure thoroughness, structure, and reliability.

- **`Common Methodologies`:**
  
1. **`PTES` (`Penetration Testing Execution Standard`)**

   - Full process from **`pre-engagement` to `post-exploitation`** and reporting.

2. **`OSSTMM` (`Open Source Security Testing Methodology Manual`)**

   - Focuses on **`operational security`** and legal clarity.

3. **`OWASP` Testing Guide**

   - Ideal for **`web applications`**. Follows the top 10 web vulnerabilities.

4. **`NIST SP800-115`**

   - U.S. government standard for security assessments.

## Typical Phases of a Penetration Test

| **Phase**                                         | **Description**                                                                                                       |
|---------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| **1. `Pre-engagement` (`Planning`)**              | **`Define scope`, `goals`, `legal agreements`, `tools`, `timeline`, `team roles`**.                                   |
| **2. `Reconnaissance` (`Information Gathering`)** | **`Passive and active scanning`, `DNS lookup`, `WHOIS, Google hacking`,** etc.                                        |
| **3. `Scanning` & `Enumeration`**                 | **Use tools like `Nmap to scan ports`, `detect OS`, `services`, and `gather internal details`.**                      |
| **4. `Vulnerability Analysis`**                   | **Identify known `vulnerabilities using scanners` (`Nessus`, `Nikto`, `OpenVAS`, etc.)**.                             |
| **5. `Exploitation`**                             | **Try to `gain access` using `exploits`, `misconfigurations`, and `weak credentials`**.                               |
| **6. `Post-Exploitation`**                        | **Assess the `impact`, `extract data`, `escalate privileges`, and `maintain access`**.                                |
| **7. `Reporting`**                                | **Deliver a `comprehensive report` that includes `findings`, `screenshots`, `risk levels`, and `recommended fixes`**. |

## Types of Penetration Testing

- **`Penetration tests`** are divided based on how much information the tester is given. There are **`three primary types`:**

- **`Black Box Testing`(`No Knowledge`)**

  - **`No prior knowledge`** of the target system.

  - Tester acts like an external hacker.

  - Time-consuming and realistic.

  - Used to simulate real-world attacks from outsiders.

- **`Example`:** A company asks you to test their e-commerce website without telling you anything about its structure, technologies, or credentials.

- **`Grey Box Testing`(`Partial Knowledge`)**

  - Partial knowledge of the system.

  - You may receive user-level credentials or some internal documentation.

  - Mimics an insider threat (e.g., an employee or partner).

- **`Example`:** A company gives you a standard user account and asks you to try accessing admin-level data or perform privilege escalation.

- **`White Box Testing`(`Full Knowledge`)**

  - Full access to the internal system: source code, infrastructure, architecture, credentials.

  - Deep and thorough testing.

  - Used to test **`logic flaws`, `code-level bugs`, and `internal misconfigurations`**.

- **`Example`:** A bank gives you full access to their internal system, including admin credentials and source code, to find deep security holes before launching it publicly.

### Real-World Scenarios

### Penetration Testing Scenarios Table

| **Test Type**      | **Scenario**                                                                                                                                                                            |
|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **`BlackBox`**     | You're hired to test a university website. You only know the URL. You perform recon, look for login pages, try SQL injection, brute-force, and enumerate users.                         |
| **`GreyBox`**      | A startup provides a regular user account for their SaaS app. You explore session manipulation, broken access controls, and insecure API endpoints to try accessing admin data.         |
| **`WhiteBox`**     | A hospital gives you full backend access to their patient management app. You analyze the source code and identify hardcoded passwords, API token leaks, and insecure session handling. |

## Popular Tools Used in Pentesting

### Tools Used in Penetration Testing

| **Phase**                      | **Tools**                                            |
|--------------------------------|------------------------------------------------------|
| **`Reconnaissance`**           | **`Google Dorking`, `Maltego`, `Recon-ng`**          |
| **`Scanning` & `Enumeration`** | **`Nmap`, `Nessus`, `Nikto`, `Dirb`, `Gobuster`**    |
| **`Exploitation`**             | **`Metasploit`, `SQLmap`, `Burp Suite`, `Hydra`**    |
| **`Post Exploitation`**        | **`Mimikatz`, `Empire`, `PowerSploit`**              |
| **`Web App Testing`**          | **`OWASP ZAP`, `Burp Suite`, `Wfuzz`**               |
| **`Reporting`**                | **`Dradis`, `Serpico`, `CherryTree`**                |

## Summary

- Penetration Testing helps secure systems by identifying weaknesses **`before attackers do`**.

- It requires **`ethical behavior`, `methodical approaches`, and `realistic testing scenarios`**.

- Understanding the **`types of testing` (`Black`, `White`, `Grey`)** helps define your role and scope.

- Tools and methodologies bring structure and efficiency to the entire process.
