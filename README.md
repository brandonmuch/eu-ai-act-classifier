# EU AI Act Risk Classification Tool

![Python](https://img.shields.io/badge/Python-3.x-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Source](https://img.shields.io/badge/Source-EUR--Lex%202024%2F1689-navy)

> A Python-based compliance tool that classifies AI systems against the four 
> risk tiers established under EU Regulation 2024/1689 (EU AI Act).
> Built from primary legislation, not third-party summaries.

---

## Overview

Given a plain-language description of an AI system, the tool returns:

- The applicable **risk tier** under EU Regulation 2024/1689
- The specific **legislative article** governing that classification
- The **compliance obligations** the deploying organisation must meet
- The **fundamental rights principle** the classification protects

---

## Risk Tiers

| Tier | Article | Meaning |
|------|---------|---------|
| 🔴 Unacceptable Risk | Article 5 | Prohibited. Cannot be deployed in the EU. |
| 🟠 High Risk | Article 6 + Annex III | Permitted with strict compliance obligations. |
| 🟡 Limited Risk | Article 50 | Permitted with transparency obligations only. |
| 🟢 Minimal Risk | Recital 48 | Permitted. No mandatory requirements. |

---

## Example Output
