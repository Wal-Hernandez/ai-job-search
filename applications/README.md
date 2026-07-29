# Applications

This directory holds one folder per job application. Each folder contains the full artifact set for that application so you can review, revise, or recompile everything in one place.

## Folder naming convention

```
applications/<company>-<role>/
```

Use lowercase, hyphenated names. Examples:

- `applications/texau-backend-developer/`
- `applications/mercadolibre-senior-full-stack/`

## Required files per application

Each application folder should contain:

| File | Purpose |
|------|---------|
| `job-posting.md` | The job posting text or a link + summary. |
| `evaluation.md` | Fit evaluation using `04-job-evaluation.md`. |
| `cv.tex` | Tailored CV for the role. |
| `cv.pdf` | Compiled CV (2 pages). |
| `cover-letter.tex` | Tailored cover letter. |
| `cover-letter.pdf` | Compiled cover letter (1 page). |
| `interview-notes.md` | STAR stories, likely questions, talking points, questions to ask. |

## Optional files

- `application-form-fields.txt` — Pasted free-text fields from portal applications (see `08-application-forms.md`).
- `follow-up.md` — Notes on thank-you emails, recruiter conversations, or outcomes.

## Note on version control

The `.tex` source files and markdown notes in this directory are tracked. The compiled `.pdf` files are generated artifacts and are ignored by the root `.gitignore`. You can always recompile from the `.tex` sources.
