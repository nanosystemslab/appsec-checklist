# Reference Sources

- **R1.** [OWASP Internet of Things Security Verification Standard (ISVS)](https://owasp.org/www-project-iot-security-verification-standard/)
- **R2.** [OWASP Internet of Things Security Testing Guide (ISTG)](https://owasp.org/www-project-iot-security-testing-guide/)
- **R3.** [OWASP Application Security Verification Standard (ASVS)](https://owasp.org/www-project-application-security-verification-standard/)
- **R4.** [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- **R5.** [NIST SP 800-213: IoT Device Cybersecurity Guidance](https://csrc.nist.gov/pubs/sp/800/213/final)
- **R6.** [NISTIR 8259A: IoT Device Cybersecurity Capability Core Baseline](https://csrc.nist.gov/pubs/ir/8259/a/final)
- **R7.** [NISTIR 8259B: IoT Non-Technical Supporting Capability Core Baseline](https://csrc.nist.gov/pubs/ir/8259/b/final)
- **R8.** [NIST SP 800-218: Secure Software Development Framework (SSDF) Version 1.1](https://csrc.nist.gov/pubs/sp/800/218/final)
- **R9.** [NIST Cybersecurity Framework 2.0](https://www.nist.gov/publications/nist-cybersecurity-framework-csf-20)
- **R10.** [NIST Privacy Framework](https://www.nist.gov/privacy-framework)
- **R11.** [CISA Secure by Design](https://www.cisa.gov/resources-tools/resources/secure-by-design)
- **R12.** [CISA Vulnerability Disclosure Policy Template](https://www.cisa.gov/vulnerability-disclosure-policy-template)
- **R13.** [CISA Known Exploited Vulnerabilities Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)
- **R14.** [CERT Guide to Coordinated Vulnerability Disclosure](https://certcc.github.io/CERT-Guide-to-CVD/)
- **R15.** [OWASP Threat Dragon](https://owasp.org/www-project-threat-dragon/)
- **R16.** [OWASP Zed Attack Proxy (ZAP)](https://www.zaproxy.org/)
- **R17.** [GitHub: Adding a security policy to your repository](https://docs.github.com/code-security/getting-started/adding-a-security-policy-to-your-repository)
- **R18.** [GitHub: Secret scanning push protection](https://docs.github.com/en/code-security/concepts/secret-security/push-protection)
- **R19.** [GitHub: Dependabot alerts](https://docs.github.com/code-security/dependabot/dependabot-alerts/about-dependabot-alerts)
- **R20.** [GitHub: Code scanning with CodeQL](https://docs.github.com/code-security/code-scanning/introduction-to-code-scanning/about-code-scanning-with-codeql)
- **R21.** [OSV-Scanner](https://google.github.io/osv-scanner/)
- **R22.** [OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/)
- **R23.** [OWASP CycloneDX Bill of Materials Standard](https://cyclonedx.org/)
- **R24.** [OpenSSF Scorecard](https://openssf.org/projects/scorecard/)
- **R25.** [SLSA: Supply-chain Levels for Software Artifacts](https://slsa.dev/)
- **R26.** [Mozilla SSL Configuration Generator](https://ssl-config.mozilla.org/)
- **R27.** [OASIS MQTT Version 5.0 Specification](https://docs.oasis-open.org/mqtt/mqtt/v5.0/mqtt-v5.0.html)
- **R28.** [Espressif ESP-IDF Secure Boot documentation](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/security/secure-boot-v2.html)
- **R29.** [Espressif ESP-IDF Flash Encryption documentation](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/security/flash-encryption.html)
- **R30.** [OWASP Software Assurance Maturity Model (SAMM)](https://owasp.org/www-project-samm/)
- **R31.** [OWASP Top Ten Web Application Security Risks](https://owasp.org/www-project-top-ten/)
- **R32.** [OWASP API Security Project / API Security Top 10](https://owasp.org/www-project-api-security/)
- **R33.** [OWASP Web Security Testing Guide stable version](https://owasp.org/www-project-web-security-testing-guide/stable/)
- **R34.** [OWASP Software Component Verification Standard (SCVS)](https://owasp.org/www-project-software-component-verification-standard/)
- **R35.** [CISA 2025 Minimum Elements for a Software Bill of Materials (SBOM)](https://www.cisa.gov/resources-tools/resources/2025-minimum-elements-software-bill-materials-sbom)
- **R36.** [CISA Software Bill of Materials for AI - Minimum Elements](https://www.cisa.gov/resources-tools/resources/software-bill-materials-ai-minimum-elements)
- **R37.** [NIST SP 800-218 Rev. 1 / SSDF Version 1.2 Initial Public Draft](https://csrc.nist.gov/pubs/sp/800/218/r1/ipd)
- **R38.** [GitHub Docs: Creating a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)
- **R39.** [GitHub Docs: Uploading a project to GitHub](https://docs.github.com/en/get-started/start-your-journey/uploading-a-project-to-github)
- **R40.** [GitHub Docs: Configuring a publishing source for GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- **R41.** [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)


# GitHub repository packaging and publication guide

Recommended repository name: `open-hardware-appsec-checklist`.

Recommended owner: `nanosystemslab`.

Recommended short description: `Application security audit checklist and templates for open hardware projects with internet connectivity.`

Recommended visibility: public, if this is intended as a reusable lab/community resource. Use private only if you add institutional internal contacts, unpublished research details, or examples containing sensitive information.

## Recommended repository structure

```text
open-hardware-appsec-checklist/
├── README.md
├── CHECKLIST.md
├── LICENSE.md
├── SECURITY.md
├── CONTRIBUTING.md
├── CITATION.cff
├── .gitignore
├── .env.example
├── .nojekyll
├── docs/
│   ├── index.md
│   ├── GITHUB_UPLOAD_GUIDE.md
│   ├── REFERENCE_SOURCES.md
│   └── FUTURE_UPDATE_PROMPT.md
├── templates/
│   ├── audit-record.md
│   ├── threat-model.md
│   ├── data-flow-checklist.md
│   ├── asset-inventory.md
│   ├── risk-classification.md
│   ├── security-ownership.md
│   ├── network-exposure-review.md
│   ├── api-endpoint-inventory.md
│   ├── command-register.md
│   ├── device-registry.md
│   ├── secrets-inventory.md
│   ├── data-inventory.md
│   ├── firmware-release-record.md
│   ├── incident-response.md
│   ├── release-signoff.md
│   └── mqtt-acl-example.conf
└── .github/
    ├── dependabot.yml
    └── workflows/
        └── security-baseline.yml
```

## Browser upload workflow

1. Sign in to GitHub and go to the Nanosystems Lab organization.
2. Select **New repository**.
3. Owner: `nanosystemslab`.
4. Repository name: `open-hardware-appsec-checklist`.
5. Description: `Application security audit checklist and templates for open hardware projects with internet connectivity.`
6. Choose **Public** unless you add internal-only material.
7. It is fine to initialize with a README if you plan to edit in the browser, but easiest is to upload the prepared repository package directly.
8. In the new repository, use **Add file -> Upload files** and upload the unzipped contents of the GitHub-ready package.
9. Commit with message: `Initial release of open hardware appsec checklist`.
10. Go to **Settings -> Code security and analysis** and enable available secret scanning, push protection, Dependabot alerts, and CodeQL/code scanning features as appropriate for the account/plan.
11. Go to **Settings -> Pages** and publish from the `main` branch using the `/docs` folder if you want a simple public web page.

## Command-line upload workflow

```bash
unzip open-hardware-appsec-checklist-github-ready-v1.1.zip
cd open-hardware-appsec-checklist

git init
git add .
git commit -m "Initial release of open hardware appsec checklist"
git branch -M main
git remote add origin https://github.com/nanosystemslab/open-hardware-appsec-checklist.git
git push -u origin main
```

## License recommendation

Recommended license for this checklist/reference-document repository: **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

Why: this is primarily documentation, teaching material, templates, and checklist content rather than a software library. CC BY 4.0 permits copying, redistribution, adaptation, and reuse, including by other labs, provided attribution is given.

Suggested attribution line:

```text
Open Hardware Application Security Audit Checklist by Nanosystems Lab, University of Hawaiʻi at Mānoa, licensed under CC BY 4.0.
```

If you later add substantial executable software, consider adding a separate `LICENSE-CODE` file using MIT, BSD-3-Clause, or Apache-2.0 for software components, while keeping the documentation under CC BY 4.0.

## Before public release, replace these placeholders

- Security contact email in `SECURITY.md`.
- Preferred maintainer/contact in `README.md`.
- Citation author details in `CITATION.cff`.
- Any University of Hawaiʻi or Nanosystems Lab branding language that should be institutionally reviewed.
- Any internal URLs, IP ranges, private emails, sponsor details, or unpublished project examples.

# Future update prompt

Use this prompt in a future ChatGPT session when you want to refresh the checklist and repository:

```text
Please update my Open Hardware Application Security Audit Checklist repository and downloadable files. Use the current date and review current official guidance from OWASP, NIST, CISA, GitHub, OpenSSF, OASIS MQTT, CycloneDX, SPDX, OSV, and relevant firmware/security documentation. Compare the current sources against the previous repository files, identify material changes, update the checklist, reference document, Markdown web version, template pack, GitHub README, SECURITY.md, GitHub Actions/Dependabot examples, source list, and future-update notes. Treat final published standards as requirements and draft/public-comment documents as watch items unless they have become final. Preserve the practical student-lab workflow, stop-sign questions, risk classification, add-on catalog, and template structure. Produce updated downloadable DOCX, Markdown, template ZIP, and GitHub-ready repository ZIP files, and summarize the most important source changes with citations.
```
