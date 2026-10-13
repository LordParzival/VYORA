# VYORA

AI-assisted GitHub issue-to-pull-request automation.

## Setup
1. Create a GitHub repository named `VYORA`.
2. Upload the files from this ZIP, preserving `.github/workflows/ai-build.yml`.
3. In repository Settings → Secrets and variables → Actions, add `OPENAI_API_KEY`.
4. In repository Settings → Actions → General → Workflow permissions, enable **Read and write permissions** and **Allow GitHub Actions to create and approve pull requests** (if available).
5. Create an issue label named `ai-build`.
6. Open an issue describing a Python feature, then apply `ai-build`.
7. Review the generated pull request and code before merging.

The workflow generates `generated/proposal.py` from each labeled issue. It does not modify existing files or auto-merge. API usage incurs costs. Model availability may vary by API account.
