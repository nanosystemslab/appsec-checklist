# Open Hardware Application Security Audit Checklist

Application security audit checklist and reusable templates for open hardware projects with internet connectivity.

This repository is intended for student research projects that add Wi-Fi, Ethernet, cellular, Bluetooth gateways, LoRaWAN gateways, MQTT, HTTP APIs, web dashboards, cloud logging, remote control, over-the-air updates, or other internet-connected features to open hardware.

## What this provides

- A practical security audit workflow for internet-connected hardware projects.
- Stop-sign questions that trigger faculty/PI review before connection.
- Low/medium/high risk classification for student hardware projects.
- Detailed checklist sections for threat modeling, network exposure, identity, authentication, authorization, TLS, secrets, firmware, web/API security, data protection, dependencies, SBOMs, logging, incident response, and public release.
- Template files that students can copy into individual project repositories.
- GitHub-ready security policy, CI examples, Dependabot configuration, and web-publishing notes.

## Start here

1. Read [`CHECKLIST.md`](CHECKLIST.md).
2. Copy the relevant files from [`templates/`](templates/) into the student project repository.
3. Complete `templates/audit-record.md`, `templates/risk-classification.md`, and `templates/threat-model.md` before connecting a device to any network.
4. For public or field releases, complete `templates/release-signoff.md` and include a project-specific `SECURITY.md`.

## Basic go/no-go rule

> No identity, no encryption, no update path, no logs, no internet.

A project should not be connected to the public internet, university network, cloud broker, web dashboard, or shared lab infrastructure until it has unique credentials, encrypted traffic, no committed secrets, no unnecessary public inbound services, documented remote-command authorization, dependency scanning, and a basic threat model.

## Recommended use in a research group

Use the checklist at four gates:

1. **Design review** — before buying parts or selecting firmware/cloud stack.
2. **Pre-network review** — before connecting to Wi-Fi, Ethernet, cellular, Bluetooth gateway, LoRaWAN gateway, MQTT broker, HTTP API, cloud dashboard, university network, or public internet.
3. **Pre-demo/release review** — before public demo, conference demo, GitHub release, field test, collaborator deployment, or publication of deployment instructions.
4. **Post-change review** — after adding remote control, OTA updates, new sensors, cloud logging, human data, authentication, AI/LLM integration, or a public web interface.

## Source basis

This checklist is grounded in public guidance from OWASP, NIST, CISA, GitHub, OpenSSF, OASIS MQTT, CycloneDX, SLSA, OSV, and firmware-security documentation. See [`docs/REFERENCE_SOURCES.md`](docs/REFERENCE_SOURCES.md) for the maintained source list.

## Repository files

- [`CHECKLIST.md`](CHECKLIST.md) — full reference document.
- [`templates/`](templates/) — copy-and-fill student project templates.
- [`docs/GITHUB_UPLOAD_GUIDE.md`](docs/GITHUB_UPLOAD_GUIDE.md) — instructions for publishing or updating this repository.
- [`docs/FUTURE_UPDATE_PROMPT.md`](docs/FUTURE_UPDATE_PROMPT.md) — prompt for future standards refreshes.
- [`.github/workflows/security-baseline.yml`](.github/workflows/security-baseline.yml) — example dependency and repository security workflow.
- [`.github/dependabot.yml`](.github/dependabot.yml) — example Dependabot configuration.
- [`SECURITY.md`](SECURITY.md) — vulnerability reporting policy template for this repository.

## GitHub Pages

The `docs/index.md` file is provided so this repository can later be published as a simple GitHub Pages site. To enable it, go to **Settings -> Pages**, choose **Deploy from a branch**, select `main`, and set the folder to `/docs`.

## License

Recommended license: [Creative Commons Attribution 4.0 International](LICENSE.md).

Suggested attribution:

> Open Hardware Application Security Audit Checklist by Nanosystems Lab, University of Hawaiʻi at Mānoa, licensed under CC BY 4.0.

If substantial executable software is added later, consider licensing code files separately under MIT, BSD-3-Clause, or Apache-2.0 while keeping documentation under CC BY 4.0.

## Disclaimer

This repository provides educational and procedural guidance. It is not a substitute for institutional IT/security policy, laboratory safety review, IRB/privacy review, export-control review, sponsor requirements, or legal advice.

## History and Intent

This checklist grew out of challenges faced in project development at the UH Nanosystems Lab regarding connectivity of open hardware designs. This led to a conversation between Dr. J.J. Brown (leader of the UH Nanosystems Lab) and Wm. Salt Hale during the 2026 UW POSE workshop (Pathways to Open Source Ecosystems) wherein the suggestion of an application security audit checklist was first made. J.J. Brown developed this content through assistance of Ai (ChatGPT), and it is intended as reference material to review and reference in developing internet-connected open hardware systems. Please note the Disclaimer above. 