# LaTeX Resume with GitHub Actions

Tracks LaTeX resume changes and builds PDF via GitHub Actions.

Latest release PDF: [Releases](https://github.com/vinaysurendran/resume/releases/latest)

## Usage

1. Fork this repository.
2. Enable GitHub Actions under the "Actions" tab.
3. In Settings > Actions > General, set Workflow Permissions to "Read and write".
4. Modify `resume.tex`.
5. Go to Releases, draft a release, tag it (e.g., v0.1), and publish.
6. After build completes, download PDF from release assets.

Direct download URL format:
`https://github.com/{yourUsername}/resume/releases/latest/download/{yourUsername}_resume.pdf`

## Workflow Details

On release creation, `.github/workflows/release.yml` executes:

- Builds `resume.tex` to `resume.pdf` using `xu-cheng/latex-action`
- Uploads PDF to release assets as `{username}_resume.pdf`

## Local Build (Optional)

Install LaTeX. Compile with:


## Structure

- `resume.tex`: LaTeX source
- `.github/workflows/release.yml`: Workflow definition
- `README.md`: Project documentation