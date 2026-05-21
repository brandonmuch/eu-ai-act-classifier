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

\```
============================================================
INPUT:          An AI that screens CVs for job applications
CLASSIFICATION: HIGH RISK
Article:        Article 6 + Annex III
Legal Basis:    Permitted but subject to strict compliance obligations.
Obligations:    Requires conformity assessment, risk management system,
                human oversight, and EU registration.
Principle:      Significant potential impact on health, safety, or
                fundamental rights.
------------------------------------------------------------
DISCLAIMER: This classification is indicative only.
Final determination requires qualified legal review
under EUR-Lex 2024/1689 (EU AI Act).
============================================================
\```

---

## How to Use

**1. Clone the repository**
\```bash
git clone https://github.com/brandonmuch/eu-ai-act-classifier.git
\```

**2. Open in Jupyter Notebook**
\```bash
jupyter notebook eu_ai_act_classifier.ipynb
\```

**3. Run all cells in order**

**4. Test your own use case at the bottom of Cell 4**
\```python
test("Describe your AI system here")
\```

---

## Legislative Basis

**Article 5: Prohibited AI Practices**  
Systems that manipulate human behaviour, enable social scoring, 
perform real-time biometric surveillance, or predict criminality 
from personality traits are prohibited entirely.

**Article 6 and Annex III: High-Risk AI Systems**  
Systems in employment, financial services, law enforcement, 
education, medical devices, and border control face mandatory 
conformity assessments, risk management systems, and EU registration.

**Article 50: Transparency Obligations**  
Chatbots, deepfakes, and emotion recognition systems must disclose 
they are AI to users.

**Recital 48: Minimal Risk**  
Spam filters, recommendation engines, and similar systems carry 
no mandatory obligations.

---

## Core Principle

The EU AI Act is built on one foundation. AI must be 
**human-centric, non-discriminatory, and dignity-preserving.**  
Every prohibition and obligation flows from this principle.

---

## Known Limitations

This tool uses keyword matching against plain-language descriptions. 
Edge cases and hybrid AI systems may require manual review against 
the full legislative text.

This is a governance aid, not a legal instrument.

---

## Disclaimer

This tool is indicative only. Final risk determination requires 
qualified legal review under EUR-Lex 2024/1689. The author accepts 
no liability for compliance decisions made on the basis of this 
tool alone.

---

## Author

**Brandon Muchenje**  
AI Governance and GRC Analyst  
BCom in Law (Cum Laude) | IBM Data Science | IAPP AIGP Training  
[LinkedIn](https://www.linkedin.com/in/brandon-m-muchenje) | 
[GitHub](https://github.com/brandonmuch)

---

## References

- [EU AI Act Full Text](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689)
- [NIST AI Risk Management Framework](https://www.nist.gov/artificial-intelligence)
- [ISO/IEC 42001](https://www.iso.org/standard/81230.html)
```
