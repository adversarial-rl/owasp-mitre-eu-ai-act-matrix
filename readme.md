# 🛡️ AI Compliance & Security Matrix (OWASP × MITRE ATLAS × EU AI Act × ISO 42001)

[![Live Engine](https://img.shields.io/badge/Live%20Interactive%20Engine-Adversarial--RL-00FF88?style=for-the-badge&logo=googlechrome&logoColor=black)](https://adversarial-rl.org/ai-compliance-matrix/)
[![License: MIT](https://img.shields.io/badge/License-MIT-00B4FF.svg?style=for-the-badge)](LICENSE)
[![Normative Scope](https://img.shields.io/badge/Regulatory-EU%20AI%20Act%20Art.%2015-FF6B35?style=for-the-badge)](https://adversarial-rl.org/ai-governance-eu-ai-act-iso-42001/)

An open, verifiable normative mapping bridging technical adversarial machine learning vulnerabilities (**OWASP LLM Top 10**, **MITRE ATLAS**) to statutory audit mandates under the **EU Artificial Intelligence Act (Article 15)**, **ISO/IEC 42001:2023**, and **ISO/IEC 27001:2022**.

---

### 🌐 Official Interactive Engines & Online Tools

* 👉 **Interactive Matrix & Dynamic CSV Exporter:**  
  [https://adversarial-rl.org/ai-compliance-matrix/](https://adversarial-rl.org/ai-compliance-matrix/)
* 🔍 **Client-Side MCP & Agent Security Linter:**  
  [https://adversarial-rl.org/mcp-agent-security-scanner/](https://adversarial-rl.org/mcp-agent-security-scanner/)
* 🐍 **Hardened Python (.py) Audit Script Synthesizer:**  
  [https://adversarial-rl.org/ai-agent-script-generator/](https://adversarial-rl.org/ai-agent-script-generator/)
* 📊 **AI & Robotics Job Displacement Evaluator:**  
  [https://adversarial-rl.org/ai-job-displacement-calculator/](https://adversarial-rl.org/ai-job-displacement-calculator/)

---

## 📋 Normative Mapping Summary

| ID | Threat / Vulnerability | OWASP LLM | MITRE ATLAS | EU AI Act Reference | Mandatory ISO Control | Technical Audit Evidence |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **ARL-MAP-01** | Indirect Prompt Injection via RAG | LLM01 | AML.T0051.001 | Article 15(4) & 15(5) | ISO 42001 B.6.2.4 · ISO 27001 A.8.26 | Red-teaming canary logs verifying <1% jailbreak bypass on untrusted ingested documents. |
| **ARL-MAP-02** | Excessive Agency & Tool Hijacking | LLM06 | AML.T0053 | Article 14 & Article 15(1) | ISO 42001 B.6.1.2 · ISO 27001 A.5.15 | Strict JSON schema validation, microVM escape testing, and required HITL approval logs. |
| **ARL-MAP-03** | Cross-Tenant Leak in Vector DB | LLM08 | AML.T0024 | Article 10 & Article 15(3) | ISO 42001 B.7.4 · ISO 27001 A.8.3 | k-NN similarity penetration audit demonstrating zero ACL metadata leakage across tenants. |
| **ARL-MAP-04** | Training Data Poisoning & Backdoors | LLM04 | AML.T0020 | Article 15(5) | ISO 42001 B.7.2 · ISO 27001 A.8.9 | SHA-256 dataset provenance verification and spectral activation analysis on LoRA weights. |
| **ARL-MAP-05** | AI Supply Chain Compromise | LLM03 | AML.T0010 | Article 15(1) & Article 17 | ISO 42001 B.6.2.2 · ISO 27001 A.5.21 | Signed CycloneDX AI-BOM and static bytecode scanning showing zero unsafe deserialization. |
| **ARL-MAP-06** | PII Extraction & Membership Inference | LLM02 | AML.T0025 | Article 10(5) & GDPR Art. 32 | ISO 42001 B.8.2 · ISO 27001 A.5.34 | Perplexity and verbatim memorization test logs across 10,000 extraction probes. |

---

## 📦 Data Formats Available

This repository provides the normative framework in structured formats for direct integration into GRC (Governance, Risk, Compliance) software:
* [`data/ai_compliance_matrix.csv`](data/ai_compliance_matrix.csv)
* [`data/ai_compliance_matrix.json`](data/ai_compliance_matrix.json)

For live real-time filtering, keyword search, and custom CSV generation without cloning this repo, use the official web interface:  
🔗 **[https://adversarial-rl.org/ai-compliance-matrix/](https://adversarial-rl.org/ai-compliance-matrix/)**

---

## ⚖️ License
Released under the [MIT License](LICENSE). Maintained by [Adversarial RL](https://adversarial-rl.org/).
