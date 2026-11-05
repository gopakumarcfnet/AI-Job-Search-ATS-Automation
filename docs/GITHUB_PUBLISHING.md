# Publish this n8n project to GitHub

## Option A — GitHub website (no Git commands)

1. Sign in at [github.com](https://github.com/).
2. Click **+** (top right) → **New repository**.
3. Set repository name to `ai-job-search-ats-automation` and add a short description: `Five-stage n8n automation for job discovery and ATS-tailored resumes`.
4. Choose **Public** if this is for your portfolio. Do **not** initialize with a README if you intend to upload this package's README directly.
5. Click **Create repository**.
6. On the empty repository page choose **uploading an existing file** (or **Add file → Upload files**).
7. **Extract the ZIP first.** Upload the contents of the extracted folder, not the ZIP alone. Preserve paths: `README.md`, `workflow/ai-job-search-ats-automation.json`, `supabase/schema.sql`, `docs/workflow-architecture.png`, and `docs/GITHUB_PUBLISHING.md`.
8. Enter commit message `Add documented n8n job search automation` and click **Commit changes**.
9. Confirm GitHub displays the README and image correctly. Open the workflow JSON to confirm it contains placeholders, not private data.
10. Share the repository URL on LinkedIn or your resume.

> **Note:** The **Publish** button shown in the n8n editor publishes/activates the n8n workflow, not a GitHub repository.

## Option B — Git command line

From inside the extracted project folder:

```bash
git init
git add README.md workflow/ supabase/ docs/ .gitignore
git commit -m "Add documented n8n job search automation"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ai-job-search-ats-automation.git
git push -u origin main
```

Create the empty GitHub repository first. Replace `YOUR_USERNAME` with your actual GitHub username. GitHub may request authentication through a browser or credential manager.

## Before publishing: privacy checklist

- [ ] Export uses `you@example.com`, not your real email.
- [ ] Google Drive file and folder IDs are placeholders.
- [ ] Supabase project reference is a placeholder.
- [ ] No credentials, tokens, personal resume text, or execution logs are committed.
- [ ] The screenshot contains no confidential data.
- [ ] README claims reflect the current workflow and its known limitations.

## Updating later

Use **Add file → Upload files** to upload revised files, or commit and push changes using Git. Avoid posting a raw export after reconnecting private credentials. Re-sanitize each new export.
