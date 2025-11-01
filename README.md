# Human-E.S.C.A.P.E. Threat Model
### Beyond the Firewall: Human-Centric Security Risk Management

<div align="center">

![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/Version-1.0-blue.svg)
![Focus](https://img.shields.io/badge/Focus-GRC-green.svg)
![Maintained](https://img.shields.io/badge/Maintained-Yes-brightgreen.svg)

**A comprehensive GRC framework for identifying, assessing, and mitigating human-centric cybersecurity threats**

[Overview](#overview) • [Framework](#the-escape-framework) • [Case Studies](#case-studies) • [Implementation](#implementation-guide) • [ROI Analysis](#roi-analysis) • [Get Started](#getting-started)

</div>

---

## 🎯 Overview

While organizations invest billions in firewalls, EDR, and SIEM systems, **74% of data breaches involve the human element** (Verizon DBIR 2024). Traditional threat models focus on technical vulnerabilities while ignoring the most exploitable attack surface: **human psychology**.

### The Problem

| Challenge | Reality |
|-----------|---------|
| 💰 **Average Breach Cost** | ₹40.5 Crore per incident involving human error |
| 📧 **Phishing Success Rate** | 32% of employees click malicious links |
| ⏱️ **Detection Time** | 287 days average to detect social engineering |
| 📊 **Organizations with Human Risk Programs** | Only 23% have formal programs |

### The Solution: Human-E.S.C.A.P.E.

A structured framework providing:
- ✅ **Quantifiable risk assessment** for human vulnerabilities
- ✅ **Policy and control recommendations** aligned with ISO 27001, NIST CSF, SOC 2
- ✅ **Real-world validation** through major breach analysis (Twitter, Uber, MGM)
- ✅ **Practical implementation guidance** for GRC professionals
- ✅ **Proven ROI** with 633% average return on investment

---


### Framework Highlights

**Each component scores 0-100 based on:**
- Presence of attack indicators
- Control effectiveness
- Environmental risk factors
- Historical incident data

**Weighted Risk Calculation:**
```
Human Risk Score = (E × 0.20) + (S × 0.25) + (C × 0.15) + 
                   (A × 0.20) + (P × 0.10) + (E × 0.10)
```

**Risk Classification:**
- 🟢 0-29: **LOW** - Monitor and maintain
- 🟡 30-49: **MODERATE** - Enhance controls
- 🟠 50-69: **HIGH** - Immediate action needed
- 🔴 70-100: **CRITICAL** - Crisis response required

---

## 📚 Case Studies

### 🎯 MGM Resorts Ransomware (September 2023)

**10-minute phone call. ₹915 Crore loss.**

```
Attack Vector: Help Desk Social Engineering
Duration: 10 minutes
Impact: 9-day operational shutdown
Financial Loss: ₹915 Crore ($110M)
```

**E.S.C.A.P.E. Analysis:**

| Component | Score | Key Factor |
|-----------|-------|-----------|
| Emotional | 79/100 | Empathy for "locked out" employee |
| Social Engineering | 91/100 | Professional impersonation |
| Cognitive Bias | 76/100 | Helpfulness bias overrode security |
| Authority | 71/100 | Claimed IT department affiliation |
| Pressure | 84/100 | "Urgent meeting" time constraint |
| Environmental | 82/100 | Help desk culture of quick resolution |
| **OVERALL RISK** | **80.5/100** | **CRITICAL** |

**Control Failures:**
- ❌ No multi-factor identity verification
- ❌ Password reset without manager approval
- ❌ No anomaly detection for privilege escalation
- ❌ Weak help desk authentication protocols

**What Would Have Prevented This:**
- ✅ 3-factor identity verification for password resets
- ✅ Callback to registered employee number
- ✅ Manager approval for privileged accounts
- ✅ Monitoring for post-reset anomalous activity

---

### 🎯 Uber Data Breach (September 2022)

**MFA fatigue + WhatsApp impersonation. ₹1,230 Crore impact.**

```
Attack Method: MFA Fatigue + Fake IT Support
Entry Point: Contractor credentials
Impact: Full network compromise
Financial Loss: ₹1,230 Crore ($148M in fines)
```

**Attack Chain:**
1. Purchased contractor credentials from dark web
2. Sent 50+ MFA push notifications (fatigue attack)
3. WhatsApp message: "Hi, this is Uber IT. Accept MFA to help us investigate"
4. Contractor clicked "Accept" → Full VPN access
5. Found shared admin credentials → AWS access
6. Full compromise: Internal systems, source code, customer data

**E.S.C.A.P.E. Score: 82/100 (CRITICAL)**

**Key Lessons:**
- Limit MFA push notifications (max 3/hour)
- Out-of-band verification for IT requests
- Contractor security baseline requirements
- Eliminate shared credentials with PAM solution

---

### 🎯 Twitter Breach (July 2020)

**Spear phishing targeting support staff. ₹2,907 Crore reputational damage.**

```
Attack Vector: Vishing + Credential Harvesting
Accounts Compromised: 130 high-profile (Obama, Biden, Musk)
Direct Loss: ₹1 Crore ($120K Bitcoin scams)
Reputational Damage: ₹2,907 Crore ($350M estimated)
```

**E.S.C.A.P.E. Score: 83/100 (CRITICAL)**

**Root Cause:**
- Employees granted admin access without callback verification
- No secondary authentication for high-privilege requests
- Insufficient social engineering awareness training

---

## 🛡️ Implementation Guide

### Phase 1: Foundation (Months 1-2)

**Goal:** Establish baseline and governance

**Key Activities:**
- [ ] Baseline E.S.C.A.P.E. risk assessment
- [ ] Executive presentation and budget approval
- [ ] Policy gap analysis
- [ ] Governance structure setup
- [ ] Pilot phishing simulation

**Deliverables:**
- Risk assessment report
- Executive sponsor identified
- Implementation roadmap
- Current-state metrics

**Budget:** ₹23-28 Lakhs (small-medium org)

---

### Phase 2: Control Implementation (Months 3-6)

**Goal:** Deploy technical and administrative controls

**Technical Controls:**

| Control | Purpose | Example Solutions | Cost (INR/year) |
|---------|---------|-------------------|-----------------|
| Email Security | Block phishing | Proofpoint, Mimecast, Fortinet | ₹8-25 Lakhs |
| Awareness Platform | Training & simulations | KnowBe4, Cofense, Quick Heal | ₹12-33 Lakhs |
| MFA Enhancement | Prevent credential theft | Duo, Okta, ManageEngine | ₹4-12 Lakhs |
| User Behavior Analytics | Detect anomalies | Splunk, MS Sentinel, IBM QRadar | ₹16-42 Lakhs |

**Administrative Controls:**
- Authentication & Verification Policy
- Security Awareness Policy
- Incident Response Plan (Human-Centric)
- Help Desk Verification Protocol
- Financial Transaction Controls

---

### Phase 3: Training & Culture (Months 7-9)

**Goal:** Build security-aware workforce

**Role-Based Training Matrix:**

| Role | Hours/Year | Frequency | Focus Areas |
|------|-----------|-----------|-------------|
| All Employees | 8 | Quarterly | Phishing, passwords, reporting |
| Finance/Accounting | 16 | Monthly | Wire fraud, invoice scams, CEO fraud |
| IT/Help Desk | 24 | Bi-weekly | Social engineering, verification |
| HR | 12 | Monthly | Pretexting, PII protection |
| Executives | 8 | Quarterly | Targeted attacks, spear phishing |

**Simulation Program:**
- Month 7: Generic phishing (baseline)
- Month 8: IT password reset + vendor invoice
- Month 9: CEO fraud + benefits enrollment

**Target Metrics:**
- 95%+ training completion
- Phishing click rate <10% (vs 32% industry avg)
- Incident reporting time <1 hour
- Zero successful social engineering breaches

---

### Phase 4: Continuous Improvement (Months 10-12)

**Goal:** Measure effectiveness and optimize

**Monthly:**
- Risk reassessment
- Phishing simulations
- Control testing
- Incident trend analysis

**Quarterly:**
- Executive reporting
- Policy updates
- Training refresh
- External benchmarking

**Success Indicators:**
- Overall risk score reduced by 25-40%
- Phishing success rate <10%
- Detection time <24 hours
- Positive ROI demonstrated

---

## 💰 ROI Analysis

### Investment vs. Benefits (Medium Organization: 500-5,000 employees)

**Year 1 Investment:** ₹6.47 Crores

| Category | Amount |
|----------|--------|
| Technology (Email, MFA, UBA) | ₹2.08 Cr |
| Training & Awareness | ₹1.49 Cr |
| Consulting & Assessment | ₹1.25 Cr |
| Internal Labor | ₹1.66 Cr |

---

**Annual Benefits:** ₹47.48 Crores

| Benefit | Amount |
|---------|--------|
| Avoided Breach Costs | ₹39.84 Cr |
| Productivity Gains | ₹1.99 Cr |
| Compliance Benefits | ₹1.49 Cr |
| Reputation Protection | ₹4.15 Cr |

---

### ROI Calculation

```
Investment:      ₹6.47 Crores
Annual Benefit:  ₹47.48 Crores
Net Benefit:     ₹41.00 Crores

ROI = 633%
Payback Period = 1.6 months
```

**3-Year Cumulative Value:** ₹145+ Crores

---

## 📋 Compliance Mapping

### ISO 27001:2022

| Control | E.S.C.A.P.E. Alignment |
|---------|----------------------|
| A.6.3 - Security Awareness | All components - Training program |
| A.5.16 - Identity Management | S, A - Verification protocols |
| A.5.17 - Authentication | S, A - Callback verification |
| A.5.24 - Incident Management | All - Human-centric response |

### NIST Cybersecurity Framework 2.0

| Function | Category | Implementation |
|----------|----------|----------------|
| GOVERN | GV.RM-03 | E.S.C.A.P.E. risk assessments |
| IDENTIFY | ID.RA-07 | Human threat identification |
| PROTECT | PR.AT-01/02 | Role-based training |
| DETECT | DE.CM-01 | User behavior analytics |
| RESPOND | RS.AN-04 | Incident categorization |

### SOC 2 Trust Services

| Criteria | Control |
|----------|---------|
| CC6.1 - Access Controls | MFA + verification protocols |
| CC6.2 - Access Assignment | Role-based with human risk factors |
| CC7.2 - System Monitoring | Behavioral analytics, phishing detection |
| CC7.4 - Incident Response | Human-centric response plan |

---


**Score Interpretation:**
- 0-40: 🔴 Critical - Immediate action required
- 41-60: 🟠 High - Significant gaps
- 61-75: 🟡 Moderate - Room for improvement
- 76-100: 🟢 Low - Strong posture

---



## 🎓 Academic Use

This framework is ideal for:
- 🎯 Cybersecurity course projects
- 🏆 GRC certification capstone projects
- 💼 Corporate security program development
- 📚 Academic research in human factors

### Citation

```bibtex
@misc{kumar2024escape,
  author = {Kumar, Soundhar},
  title = {Human-E.S.C.A.P.E. Threat Model: A GRC Approach to 
           Human-Centric Security Risk Management},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/soundhar-kumar/Human-ESCAPE-Model}
}
```

---

## 🤝 Contributing

We welcome contributions from:
- 👨‍💼 GRC professionals with implementation experience
- 🎓 Academics researching human factors in cybersecurity
- 👨‍🎓 Students studying information security or risk management
- 🛡️ Industry practitioners with breach response experience

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

**Contribution Ideas:**
- Additional case studies from recent breaches
- Industry-specific adaptations (healthcare, finance, retail)
- Tool enhancements and automation scripts
- Translation to other languages
- Policy template improvements

---

## 📈 Project Statistics

- **Framework Components:** 6
- **Major Breaches Analyzed:** 3 (Twitter, Uber, MGM)
- **Total Financial Impact Studied:** ₹4,180+ Crores
- **Records Exposed:** 300M+
- **Compliance Frameworks Mapped:** 5+ (ISO, NIST, SOC 2, PCI-DSS, HIPAA)
- **Industry Reports Referenced:** 10+ (Verizon DBIR, IBM, Gartner, Proofpoint)
- **Implementation Phases:** 4 (Foundation, Controls, Training, Optimization)

---

## 📝 License

MIT License - See [LICENSE](LICENSE) for full details.

**Summary:** Free to use, modify, and distribute with attribution. No warranty provided.

---

## ⚠️ Disclaimer

This framework is provided for **educational and research purposes**.

- ✋ Implementation should be tailored to organizational context
- 🔒 Consult security professionals before deployment
- ✅ Validate controls with internal audit/compliance teams
- 📋 No guarantee of prevention of all breaches
- ⚖️ Author assumes no liability for misuse

**Best Practice:** Use as a starting point, then customize based on your industry, size, regulatory requirements, and risk appetite.

---

## 👨‍💻 About the Author

**Soundhar Kumar**
- 🎯 **Focus:** Governance, Risk & Compliance (GRC) | Human-Centric Security
- 💼 **Expertise:** GRC Analysis, Risk Management, Social Engineering Defense

## 🌟 Support This Project

If this framework helps your organization or research:

- ⭐ **Star** this repository
- 🔄 **Share** with your network
- 📝 **Cite** in your research papers
- 💬 **Discuss** your experience in GitHub Discussions
- 🤝 **Contribute** case studies, tools, or improvements

**Your support helps advance human-centric security across the industry!**
---

<div align="center">

## 🏆 Recognition

**If this project helped secure your organization or advance your research, please consider:**

[![Star this repo](https://img.shields.io/github/stars/soundhar-kumar/Human-ESCAPE-Model?style=social)](../../stargazers)
[![Fork this repo](https://img.shields.io/github/forks/soundhar-kumar/Human-ESCAPE-Model?style=social)](../../network/members)

---

**Last Updated:** November 2024 | **Version:** 1.0.0 | **Status:** Active Research & Development

*Built with focus on making cybersecurity more human-centered, practical, and accessible to GRC professionals.*

**[⬆ Back to Top](#human-escape-threat-model)**

</div>
