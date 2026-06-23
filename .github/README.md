# .github folder

This folder contains repository automation and contribution helpers for the Open Hardware Application Security Audit Checklist.

Included files:

- `dependabot.yml` — asks Dependabot to monitor GitHub Actions used by this repository.
- `workflows/security-baseline.yml` — runs lightweight repository hygiene checks on pushes and pull requests to `main`.
- `ISSUE_TEMPLATE/checklist-improvement.yml` — structured issue form for improvements to checklist content or templates.
- `ISSUE_TEMPLATE/security-review.yml` — structured issue form for student project security-review tracking.
- `ISSUE_TEMPLATE/config.yml` — disables blank issues and points vulnerability reports toward the repository security policy.
- `pull_request_template.md` — reviewer checklist for content and security updates.

Before relying on the workflow, confirm that the root `SECURITY.md` contains the correct security-contact method.
