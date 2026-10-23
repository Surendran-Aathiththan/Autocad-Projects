# CLAUDE.md

## What this repo is

A public **AutoCAD portfolio** for Surendran Aathiththan, hosted at
https://github.com/Surendran-Aathiththan/Autocad-Projects. Its audience is recruiters,
hiring engineers and prospective clients, who mostly see it through the GitHub web UI.
The goal of most work here is to make each project easy to understand at a glance:
a clear preview image, a short description, and the skills it demonstrates.

## Layout

- One folder per project (`3d projects/`, `Building planning/`, `Boat Design For Autralian Client Project/`).
- Each project folder holds the source `.dwg` plus exports (`.png`, `.pdf`) and any reference material.
- The root `README.md` is the portfolio landing page: hero image + a table linking every project.

## Rules

- **Never edit, rewrite or "fix" `.dwg`, `.pdf`, `.png`, `.jpg` or `.docx` files.** They are binary
  and authored in AutoCAD/Word. Only read them (images and PDFs can be viewed for writing descriptions).
- **Ask before renaming or moving folders/files.** Folder names appear in README links (URL-encoded,
  e.g. `3d%20projects`), and renaming rewrites git history for large binaries. If a rename is approved,
  update every link in every README in the same commit.
- Folder and file names contain spaces: always quote paths and URL-encode spaces (`%20`) in Markdown links.
- Do not describe AI-generated images (`ChatGPT Image ...png`, `Gemini_Generated_Image_...png`) or third-party
  images (e.g. the `jmse-...jpg` journal figure) as the owner's own drawings. Label them as concept/reference
  material with attribution, or suggest moving them to a `reference/` subfolder.
- Treat client work as potentially confidential: do not add client names, contract details or measurements
  beyond what is already published without asking.
- Commit locally when asked; **always ask before `git push`**.

## Writing style for READMEs

- Short and scannable: one preview image, 2–4 sentence summary, then a bullet list of
  "Skills shown" (e.g. 2D drafting, dimensioning, layers, 3D solid modelling, plotting/layouts).
- State the AutoCAD version used and how to view the file (AutoCAD 2018+ or the free Autodesk Viewer).
- Use relative links and relative image paths so they render on GitHub.

## Tooling notes (Windows)

- `git` is not on PATH in this environment. Use GitHub Desktop's bundled git:
  `& "$env:LOCALAPPDATA\GitHubDesktop\app-3.6.7\resources\app\git\cmd\git.exe" <args>`
  (the version folder may change after GitHub Desktop updates).
- `gh` (GitHub CLI) is not installed.
- The shell is Windows PowerShell 5.1: no `&&`, use `;` or `if ($?) { ... }`.
