# Threat Modeling for AI

## Why STRIDE no longer covers the AI attack surface  

STRIDE (Spoofing · Tampering · Repudiation · Information disclosure · Denial of service · Elevation of privilege) still helps for classic web / API layers, but modern AI systems expose **five new categories of risk**:

- **Model & data supply-chain attacks** – poisoning training corpora, swapping or downgrading models  
- **Prompt-level exploits** – prompt injection, jailbreaks, cross-model leakage  
- **Autonomous / agentic behaviour** – tool misuse, goal drift, self-replication  
- **Run-time amplification loops** – cascading errors, spam or malware propagation  
- **Governance & trust failures** – privacy breaches, bias, copyright violations  

These issues dominate recent incident reports and appear throughout the OWASP LLM Top 10 and MITRE ATLAS threat catalogues. :contentReference[oaicite:0]{index=0}  

---

## Frameworks that fill STRIDE’s gaps for AI security  

- **MITRE ATLAS** – a public knowledge-base of tactics, techniques, and real-world cases for attacking ML/LLM systems; think “ATT&CK for AI”. :contentReference[oaicite:1]{index=1}  
- **OWASP LLM / GenAI Top 10 (2025)** – community-curated list of the most common failures in generative-AI apps, with mitigations. :contentReference[oaicite:2]{index=2}  
- **OWASP Agentic-AI Threats & Mitigations** – threat taxonomy focused on single- and multi-agent systems (memory hijack, tool escalation, infinite loops). :contentReference[oaicite:3]{index=3}  
- **CSA MAESTRO** – the first threat-modeling method built specifically for agentic AI (Multi-Agent Environment, Security, Threat, Risk & Outcome). :contentReference[oaicite:4]{index=4}  
- **Google Secure AI Framework (SAIF)** – end-to-end control catalogue plus an interactive self-assessment covering training → deployment → operations. :contentReference[oaicite:5]{index=5}  
- **NIST AI Risk Management Framework 1.0** – a U.S. standard for *Govern → Map → Measure → Manage* AI risk across the entire life-cycle. :contentReference[oaicite:6]{index=6}  

> **Take-away:** keep STRIDE for your traditional software stack, but pair it with one or more of the above so you also cover model-, data-, and agent-centric risks.

---

## “Agentic tool – where is it?”  

### Agent-Wiz (open-source CLI)  
- **Repo:** <https://github.com/Repello-AI/Agent-Wiz> :contentReference[oaicite:7]{index=7}  
- **Purpose:** parses LangGraph, CrewAI, AutoGen & friends, visualises agent ↔ tool graphs, auto-scores each step with the MAESTRO taxonomy, and spits out HTML/JSON/Markdown security reports.  
- **Quick start:**  
  ```bash
  pip install agent-wiz
  agent-wiz scan path/to/your_app.py --output report.html
