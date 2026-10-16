# Dandelion

Dandelion is a digital contracting platform concept that connects clients with student developers through coding competitions. This repository holds the project's landing page and its startup workspace archive.

## Overview

Dandelion's model: a client posts a project with requirements, budget and timeline; student developer teams build competing solutions independently; the client reviews each submission through an isolated virtual machine without seeing source code; and the client picks a winner, at which point payment is released from escrow and the code is pushed to the client's GitHub repository via GitHub Actions.

This repository does not contain an implementation of that platform. It contains:

- **`index.html`** - a single-file static landing page describing the platform (how it works, features, and benefits for clients and developers), deployed to GitHub Pages.
- **Startup workspace documents** - the business, marketing, legal, operations and design material produced while running the Dandelion pilot in 2023-2024, including the Dandelion x Empath web development competition.

## What's inside

```
.
├── index.html            # Static landing page (HTML + inline CSS)
├── .github/workflows/
│   └── pages.yml         # Deploys the repository root to GitHub Pages on push to main
├── Design/               # Logos, favicons (used by index.html), cover images, mockups
├── Business/             # Initial idea, business model canvas, pitch deck, market sizing, strategy
├── Strategy/             # Experiment plans and next-step notes
├── Product/              # Product roadmap and workflow meeting notes
├── Marketing/            # Market research, customer interviews, competition handouts and forms
├── Operations/           # Workflow docs, KPIs, competition operations
├── Customer Care/        # Client requirement docs, email drafts, code quality assessments
├── Legal/                # Terms and conditions, NDA and agreement templates
├── Development/          # Development journal, quality control notes
├── Investors/            # Incubator application and outreach drafts
├── Logistics/            # Onboarding agenda, weekly report templates
├── Meeting notes/        # Meeting notes
├── Finance/, University/ # Miscellaneous supporting material
└── Archives/             # Earlier backups of the workspace
```

Most documents are Office files (`.docx`, `.xlsx`, `.pptx`) and PDFs.

## Tech stack

- Landing page: plain HTML and CSS (no build step, no JavaScript framework)
- Hosting: GitHub Pages via GitHub Actions

## Running the landing page locally

No build is required. Open `index.html` in a browser, or serve the folder so the favicon paths resolve:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

Pushing to `main` triggers `.github/workflows/pages.yml`, which uploads the repository root and deploys it to GitHub Pages.

## Status

Archived startup project. The workspace documents date from 2023-2024; the landing page was redesigned in December 2025.
