# ⚡ SVG Attack Lab

> A fully client-side browser tool for demonstrating, injecting, and analyzing SVG-based attack vectors — built for authorized security research, CTF competitions, and controlled lab environments.

🔗 **Live Tool:** [https://giriaryan694-a11y.github.io/SVG-Attack-Lab/](https://giriaryan694-a11y.github.io/SVG-Attack-Lab/)

---

## ⚠️ Ethical Use Disclaimer

**READ THIS BEFORE USING THE TOOL.**

SVG Attack Lab is designed **exclusively** for:

- Authorized penetration testing engagements (with written permission)
- Bug bounty programs within defined scope
- CTF (Capture The Flag) competitions
- Academic and security research in isolated/controlled lab environments
- Security awareness training and demonstrations

**This tool must never be used against systems, applications, or infrastructure that you do not own or do not have explicit written authorization to test.**

Unauthorized use of this tool against real-world systems is **illegal** and constitutes a criminal offense under multiple national and international laws. The authors, contributors, and maintainers of SVG Attack Lab accept **zero liability** for any misuse, damage, or legal consequences arising from improper use.

By accessing and using this tool, you agree to:
1. Use it only on systems you own or have explicit written authorization to test
2. Comply with all applicable local, national, and international laws
3. Follow responsible disclosure guidelines if vulnerabilities are discovered
4. Not use this tool for surveillance, stalking, data theft, sabotage, or any malicious purpose

---

## 🎯 Features

- **6 Attack Techniques** with full descriptions and severity ratings
- **Upload your own SVG** or start from a built-in template
- **Payload parameter customization** — callback URL, file path, custom JS
- **Syntax-highlighted output** with one-click download
- **Sandboxed visual preview** (scripts safely blocked)
- **Forensic analysis panel** — lists detected vectors and mitigations
- **Three UI themes** — Dark, Light, Eye-Save (warm yellowish)
- **100% client-side** — no server, no data sent anywhere

---

## 🔬 Techniques Covered

| # | Technique | Class | Severity |
|---|-----------|-------|----------|
| 1 | Inline `onload` XSS | XSS | Critical |
| 2 | `<script>` Tag Injection | XSS | Critical |
| 3 | Image-based Data Exfiltration | Exfil | High |
| 4 | `<foreignObject>` DOM Injection | DOM XSS | Critical |
| 5 | XML External Entity (XXE) | XXE / LFI | Critical+ |
| 6 | Cookie Exfiltration via Fetch | Cookie Theft | Critical+ |

---

## ⚖️ Legal Framework — Abuse Laws

Using this tool without authorization is a criminal offense. The following laws apply depending on your jurisdiction.

---

### 🇮🇳 Indian Laws

#### Information Technology Act, 2000 (IT Act)

| Section | Title | Relevance | Punishment |
|---------|-------|-----------|------------|
| **Section 43** | Penalty for damage to computer systems | Unauthorized access, downloading data, introducing malware | Civil liability — compensation up to ₹1 crore |
| **Section 43A** | Failure to protect sensitive data | Negligent handling of personal data | Compensation to affected persons |
| **Section 66** | Computer-related offences | Unauthorized access, data theft, system disruption | Up to 3 years imprisonment and/or ₹5 lakh fine |
| **Section 66B** | Receiving stolen computer resources | Possessing data obtained via unauthorized access | Up to 3 years imprisonment and/or ₹1 lakh fine |
| **Section 66C** | Identity theft | Using another person's digital signature, password, or unique identifier | Up to 3 years imprisonment and ₹1 lakh fine |
| **Section 66D** | Cheating by personation using computer resource | Impersonation using computers or communication devices | Up to 3 years imprisonment and ₹1 lakh fine |
| **Section 66E** | Violation of privacy | Capturing, publishing, or transmitting private images without consent | Up to 3 years imprisonment and/or ₹2 lakh fine |
| **Section 66F** | Cyber terrorism | Attacks on critical infrastructure, government systems | Life imprisonment |
| **Section 72** | Breach of confidentiality and privacy | Disclosing information obtained in breach of a lawful contract | Up to 2 years imprisonment and/or ₹1 lakh fine |

#### Indian Penal Code (IPC) / Bharatiya Nyaya Sanhita (BNS), 2023

- **Section 420 IPC / Section 318 BNS** — Cheating and dishonestly inducing delivery of property (applies to phishing and fraud using injected payloads)
- **Section 379 IPC / Section 303 BNS** — Theft (applies to stealing digital credentials or data)
- **Section 463 IPC / Section 336 BNS** — Forgery (applicable where SVG payloads are used to forge or fabricate digital documents)

#### Key Points Under Indian Law
- The IT Act is enforced by the **Cyber Crime cells** under state police and the **Indian Computer Emergency Response Team (CERT-In)**
- **CERT-In** mandates incident reporting for cybersecurity breaches under the CERT-In Directions, 2022
- Courts have increasingly awarded significant compensatory damages in cyber offense cases
- Cybercrime is cognizable and non-bailable under most sections of the IT Act

---

### 🌍 International Laws

#### 🇺🇸 United States

| Law | Key Provisions | Punishment |
|-----|---------------|------------|
| **Computer Fraud and Abuse Act (CFAA), 18 U.S.C. § 1030** | Unauthorized access to computer systems, exceeding authorized access, causing damage or loss | Up to 10–20 years imprisonment (repeat offense); civil liability |
| **Electronic Communications Privacy Act (ECPA)** | Unauthorized interception of electronic communications | Up to 5 years imprisonment |
| **Identity Theft Enforcement and Restitution Act** | Computer-facilitated identity theft | Restitution + imprisonment |
| **CAN-SPAM Act** | Fraudulent headers, spoofing in email-based attacks | Fines up to $43,792 per violation |

> **Note:** The CFAA has been used aggressively to prosecute security researchers. Even "exceeding authorized access" on a system you are allowed to use can trigger prosecution. Always get written authorization.

#### 🇬🇧 United Kingdom

| Law | Key Provisions | Punishment |
|-----|---------------|------------|
| **Computer Misuse Act 1990 (CMA)** | Unauthorized access (Section 1), unauthorized access with intent (Section 2), unauthorized modification (Section 3), impairing systems (Section 3ZA) | Section 1: Up to 2 years; Section 3: Up to 10 years; Section 3ZA: Life imprisonment |
| **Police and Justice Act 2006** | Amendments to CMA; criminalizes making/supplying tools for unauthorized access | Up to 2 years |
| **Investigatory Powers Act 2016** | Governs lawful interception; unauthorized interception is a criminal offense | Imprisonment + unlimited fines |

#### 🇪🇺 European Union

| Law | Key Provisions |
|-----|---------------|
| **Directive on Attacks Against Information Systems (2013/40/EU)** | Criminalizes illegal access, illegal system interference, illegal data interference, and tool production for attacks — harmonized across all EU member states |
| **General Data Protection Regulation (GDPR)** | Using attack tools to extract personal data can trigger GDPR violations — fines up to €20 million or 4% of global annual turnover |
| **NIS2 Directive (2022/0383)** | Mandatory cybersecurity requirements for critical infrastructure operators; unauthorized probing of such systems carries severe penalties |

#### 🇦🇺 Australia

| Law | Key Provisions | Punishment |
|-----|---------------|------------|
| **Criminal Code Act 1995 — Part 10.7** | Unauthorized access/modification/impairment of computer data | Up to 10 years imprisonment |
| **Privacy Act 1988** | Data exfiltration affecting personal information of Australians | Civil penalties up to AUD 50 million |

#### 🇨🇦 Canada

| Law | Key Provisions | Punishment |
|-----|---------------|------------|
| **Criminal Code, Section 342.1** | Unauthorized use of a computer | Up to 10 years imprisonment |
| **Criminal Code, Section 430(1.1)** | Mischief in relation to computer data | Up to 10 years imprisonment |

#### 🇸🇬 Singapore

| Law | Key Provisions | Punishment |
|-----|---------------|------------|
| **Computer Misuse Act (Cap. 50A)** | Unauthorized access, unauthorized modification, unauthorized use for wrongful gain | Up to 3–10 years depending on severity; fines up to SGD 50,000 |

---

### 🌐 International Treaties & Frameworks

- **Budapest Convention on Cybercrime (Council of Europe, 2001)** — The primary international treaty on cybercrime, ratified by 60+ countries including the US, UK, EU members, Canada, and Japan. Defines computer intrusion, data interference, and misuse of devices as criminal offenses requiring harmonized prosecution.

- **UN Group of Governmental Experts (UNGGE)** — Establishes norms of responsible state behavior in cyberspace; attacks on critical infrastructure are considered violations of international law.

- **Tallinn Manual 2.0** — Non-binding but widely referenced NATO framework on how international law applies to cyber operations, including offensive security activities.

---

## 🛡️ Responsible Disclosure

If you discover a real vulnerability during authorized testing:

1. **Do not exploit it further** beyond what is needed to confirm the issue
2. **Document the finding** with a clear proof-of-concept and impact assessment
3. **Notify the vendor or organization** privately via their security disclosure channel
4. **Allow reasonable remediation time** (typically 90 days — Google Project Zero standard)
5. **Coordinate public disclosure** with the affected party

Frameworks: [CVE Program](https://cve.mitre.org/) | [HackerOne Disclosure Guidelines](https://www.hackerone.com/disclosure-guidelines) | [CERT/CC Vulnerability Disclosure Policy](https://www.kb.cert.org/vuls/disclosure/)

---

## 🔒 Mitigations Reference

For defenders — what SVG Attack Lab tests against:

| Vector | Mitigation |
|--------|-----------|
| Inline XSS (onload, script) | DOMPurify with SVG namespace; strip `on*` attributes |
| foreignObject injection | Remove `<foreignObject>` from allowed SVG tags |
| External resource exfil | CSP: `img-src 'self'`; block external references |
| XXE (server-side) | Disable external entity resolution; use `defusedxml` (Python), `FEATURE_SECURE_PROCESSING` (Java) |
| Cookie theft | Set `HttpOnly` and `Secure` flags; enforce `SameSite=Strict` |
| General SVG upload | Convert to PNG server-side; serve with `Content-Type: image/png` + `X-Content-Type-Options: nosniff` |

---

## 🧰 Tech Stack

- Pure HTML5, CSS3, Vanilla JavaScript
- Zero external dependencies
- Zero server-side code
- Zero data collection

---

## 📜 License

This project is licensed for **educational and authorized security research use only**.

Redistribution or use for malicious purposes is strictly prohibited and may constitute a criminal offense under the laws listed above.

---

<p align="center">Made with ❤️ by <strong>Aryan Giri</strong> &nbsp;|&nbsp; SVG Attack Lab &nbsp;|&nbsp; For authorized security research only</p>
