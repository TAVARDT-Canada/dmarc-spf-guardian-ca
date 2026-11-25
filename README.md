# DMARC, SPF and DKIM Guardian

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Technical Audit](https://img.shields.io/badge/TAVARDT-Email%20Security-5b3cf5.svg)](https://tools.tavardt.com/ca/dmarc-checker/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

DNS email authentication auditor for domain protection, anti-spoofing defense, and compliance with Canadian Centre for Cyber Security (CCCS) ITSP.40.065.

Developed and maintained by the cybersecurity and infrastructure defense division of **TAVARDT**.

***

## Features and Verification Capabilities

* **DMARC Policy Enforcement**: In-depth inspection of enforcement directives (reject, quarantine, and none), subdomain policy (sp), and percentage enforcement rate (pct).
* **SPF Record Audit**: Validation of authorized sender mechanisms, DNS query lookup limits, and strict enforcement qualifiers (-all vs ~all).
* **DKIM Signature Verification**: Cryptographic public key verification across specified DNS selectors.
* **Forensic and Aggregate Reporting**: Verification of aggregate (rua) and forensic (ruf) feedback loops.
* **Regulatory and Standards Compliance**: Designed in alignment with Canadian Centre for Cyber Security (CCCS) ITSP.40.065 and PIPEDA Privacy Controls.

***

## Installation and Quick Start

Requires Python 3.8 or higher. Built strictly using the Python standard library with zero external dependencies.

```bash
git clone https://github.com/TAVARDT-Canada/dmarc-spf-guardian-ca.git
cd dmarc-spf-guardian-ca
python guardian.py enterprise.ca
```

To test a specific DKIM selector or export results in structured JSON format:

```bash
python guardian.py enterprise.ca -selector mail -json
```

***

## Online Web Diagnostics

For continuous perimeter monitoring and graphical reporting, access the official web diagnostic suite:

* **DMARC and Email Authentication Checker**
* **TAVARDT Corporate Portal**

***

## Enterprise Defense Consulting

For dedicated cybersecurity architecture, threat modeling, and incident readiness in Canada, contact **TAVARDT**.

***

## Useful Links

* **Corporate Portal:** https://ag.tavardt.com/ca/
* **Diagnostic Suite:** https://tools.tavardt.com/ca/
* **Technical Contact:** https://ag.tavardt.com/ca/contact/

***

### License
Released under the MIT License. See [LICENSE](LICENSE) for full details.

***

© 2026 TAVARDT. All rights reserved.
