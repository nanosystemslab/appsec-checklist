# GitHub Upload Guide

Recommended repository name: `open-hardware-appsec-checklist`.

Recommended owner: `nanosystemslab`.

Recommended description: `Application security audit checklist and templates for open hardware projects with internet connectivity.`

## Browser workflow

1. Sign in to GitHub.
2. Go to the Nanosystems Lab organization.
3. Select **New repository**.
4. Owner: `nanosystemslab`.
5. Repository name: `open-hardware-appsec-checklist`.
6. Choose **Public** unless internal/private information is added.
7. Create the repository.
8. Unzip the GitHub-ready package locally.
9. In the repository, use **Add file -> Upload files** and upload the unzipped contents.
10. Commit with the message `Initial release of open hardware appsec checklist`.
11. In **Settings -> Code security and analysis**, enable available secret scanning, push protection, Dependabot alerts, and code scanning features.
12. In **Settings -> Pages**, optionally publish from the `main` branch using the `/docs` folder.

## Command-line workflow

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

## First edits before publishing

- Replace the placeholder security email in `SECURITY.md`.
- Confirm maintainer/contact language in `README.md`.
- Confirm author/citation metadata in `CITATION.cff`.
- Remove any internal-only notes before making the repository public.
- Decide whether GitHub Pages should be enabled now or after a later web-design pass.
