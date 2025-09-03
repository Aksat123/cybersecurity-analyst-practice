# Incident Report - Scenario 1: Suspicious Login

**Date:** 2025-09-03  
**Analyst:** Akshat P

---

## 📝 Summary
Multiple failed login attempts were detected followed by a successful login from a foreign IP address.

---

## 🔍 Investigation Steps
1. Checked SIEM logs for username `jdoe_admin`.
2. Identified IP address 101.123.171.5 as source of attack.
3. Reviewed GeoIP data – location traced to Russia.
4. Found brute force pattern (15 failed logins → 1 success).

---

## 🛡 Containment
- Locked user account `jdoe_admin`.
- Blocked source IP on firewall.

---

## 📊 Tools Used
- Simulated SIEM (ChatGPT SOC Lab)
- Basic log review techniques

---

## ✅ Outcome
Attack successfully contained. Next steps include password reset and company-wide MFA enforcement.
