# 🛡️ SOC Analyst Portfolio — Tiago Krysiaki

Hands-on SOC scenarios focused on **Monitoring, Detection, Investigation, and Response** in Linux environments.

---

## 🎯 Detection Use Cases

### 🔐 SSH Brute Force Detection (MITRE T1110)

**Monitoring**
- Wazuh alerts for multiple failed SSH login attempts  

**Detection**
- High volume of authentication failures from a single IP  
- Pattern of sequential username attempts  

**Investigation**
- Analysis of `/var/log/auth.log`  
- Identification of source IP and targeted accounts  
- Timeline reconstruction of attack attempts  

**Classification**
- Brute Force Attack (T1110)  

**Response**
- Source IP blocking (Fail2ban / firewall)  
- Review of compromised or targeted accounts  

---

### 📊 Suspicious Authentication Activity

**Monitoring**
- Authentication logs via Wazuh and system logs  

**Detection**
- Logins at unusual hours  
- Access from unknown or inconsistent IP addresses  

**Investigation**
- Correlation of login events across logs  
- Validation of user behavior patterns  

**Classification**
- Potential Account Misuse / Unauthorized Access  

**Response**
- Session review and access validation  
- Credential reset if necessary  

---

### 🧾 Log Analysis & Event Correlation

**Monitoring**
- Continuous log ingestion (auth.log, auditd)  

**Detection**
- Anomalous patterns in authentication and system activity  

**Investigation**
- Cross-log correlation (auth.log + auditd)  
- IOC extraction (IP, user, timestamp)  

**Classification**
- Suspicious Activity / Security Event  

**Response**
- Escalation or containment based on severity  

---

## 🧠 Methodology

**Monitoring → Detection → Investigation → Classification → Response**

Aligned with:
- MITRE ATT&CK  
- NIST Incident Response  
- CIS Controls  

---

## 📎 Repository

👉 https://github.com/TKrysiaki/lab-soc-linux

---

## 📫 Contact

- LinkedIn: https://www.linkedin.com/in/tiago-krysiaki-b3322ba7  
- Email: t.krysiaki91@gmail.com  
