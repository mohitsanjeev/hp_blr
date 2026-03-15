# 🛡️ SOC Analyst — Dos & Don'ts

> A quick-reference 1-pager for Security Operations Center analysts.

---

## ✅ DOs

### Monitoring & Detection
- **Do** monitor alerts continuously and triage them by severity (Critical → High → Medium → Low).
- **Do** correlate events across multiple data sources (SIEM, EDR, firewall, logs) before concluding.
- **Do** document every action taken during an investigation — timestamps matter.
- **Do** follow the established incident response playbook for each alert type.
- **Do** escalate promptly when an alert exceeds your authority or expertise level.

### Communication
- **Do** communicate clearly and concisely in tickets — state what you found, what you did, and what's next.
- **Do** notify stakeholders proactively during active incidents, even with partial information.
- **Do** hand off open investigations with full context during shift changes.

### Hygiene & Best Practices
- **Do** keep your tools, signatures, and threat intelligence feeds up to date.
- **Do** perform regular threat hunting even when the queue is quiet.
- **Do** follow the principle of least privilege when accessing systems during investigations.
- **Do** use approved, sanctioned tools only — log all investigative actions.

---

## ❌ DON'Ts

### Investigation Mistakes
- **Don't** close an alert without a documented reason — "false positive" still needs justification.
- **Don't** assume an alert is benign just because it looks familiar — context always matters.
- **Don't** run untrusted scripts or open suspicious files on production or analyst machines.
- **Don't** rely solely on automated tools — apply human judgment to every investigation.

### Communication Failures
- **Don't** sit on a high-severity alert waiting for more data — escalate early, update often.
- **Don't** share incident details outside of approved channels (no personal email, no public chat).
- **Don't** make promises about resolution timelines unless confirmed with the team lead.

### Operational Risks
- **Don't** modify firewall rules, block IPs, or isolate hosts without proper authorization.
- **Don't** work around policies or take shortcuts under time pressure — document and escalate instead.
- **Don't** ignore anomalies just because they don't trigger a formal alert.

---

## 🚨 Golden Rules

| Rule | Why It Matters |
|------|----------------|
| **Log everything** | Forensics and audits depend on it |
| **Escalate early** | Delay worsens impact |
| **Assume breach** | Keeps you sharp and thorough |
| **Trust, but verify** | Even internal traffic can be compromised |

---

*Last updated: March 2026 | Owner: SOC Team Lead*
