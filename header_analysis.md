📬 Header Analysis Report: Sample_email.eml

## 🗓️ Date
**Thu, 27 Jul 2023 07:40:03 +0000**

## 📩 From
**Microsoft account team <no-reply@access-accsecurity.com>**

## 🧭 To
**phishing@pot**

---

## 🔍 Authentication Results Breakdown

### 1. ✅ Message ID
`412928a2-0aad-4b27-959a-5df404e1f07d@VI1EUR06FT066.eop-eur06.prod.protection.outlook.com`

### 2. 🔐 SPF: `none`
> **Sender Policy Framework (SPF)** checks if the email is from an authorized server for the domain.

- ❗ The domain `access-accsecurity.com` has **no SPF record**.
- 🧨 This allows any server to send emails pretending to be from that domain.
- ✅ Real domains like Microsoft will always have a valid SPF.

---

### 3. 🔐 DKIM: `none`
> **DomainKeys Identified Mail (DKIM)** checks if the message was signed and not altered.

- ❗ No DKIM signature found — no cryptographic proof of authenticity.
- 🧨 Anyone can forge the "From" field without DKIM.
- ✅ Real companies cryptographically sign messages to prevent tampering.

---

### 4. 🔐 DMARC: `permerror`
> **DMARC** tells recipients what to do when SPF/DKIM fail.

- ❗ A **permanent error** occurred — likely due to misconfigured or broken DMARC records.
- 🧨 Without DMARC, SPF/DKIM failures won’t trigger protective actions.
- ✅ Real domains enforce DMARC to reject spoofed emails.

---

## 🧠 Verdict Summary

| Security Check | Status       | Risk                         |
|----------------|--------------|------------------------------|
| SPF            | ❌ None       | High – domain can be spoofed |
| DKIM           | ❌ None       | High – no signature          |
| DMARC          | ❌ PermError  | High – no policy enforcement |

---

## 📌 Conclusion

This email is **unauthenticated and likely spoofed**. It failed all major email verification checks:

- No SPF record (easy spoofing)
- No DKIM signature (no integrity check)
- Broken DMARC (no enforcement policy)

This is a **clear phishing attempt** and should be reported and blocked immediately.
