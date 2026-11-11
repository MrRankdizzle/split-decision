# Split Decision

Little Chute Mustangs Biology review lab for Essential Standard 3.2, Cell Size and Cell Division.
Students learn and practice mitosis, ratios and surface-area-to-volume, build a stop-motion mitosis
animation, work through pathology-lab cases, and export a portfolio artifact.

## Deploy

Static site: `index.html` plus the `img/` folder. No build step.

1. Create a new GitHub repository and upload everything in this folder (keep `img/` as a folder beside `index.html`).
2. In Vercel, choose "Add New Project", import the repository, leave Framework Preset as "Other", and deploy.

## Structure

- `index.html` is the whole app (styles, scripts, question banks, drawings).
- `img/` holds the photos and micrographs. If an image is missing, the app falls back to its drawn version.
- `img/icon.svg`, `img/favicon.png` and `img/apple-touch-icon.png` are the app icon (one cell pinching into two, in school colors).
- Optional photos: `img/hydra-budding.jpg`, `img/starfish-regrowing-arm.jpg` and `img/animal-cell-cleavage.jpg` (about 1200 x 800). Drop them into `img/` and the matching questions and the Cytokinesis lesson pick them up automatically; until then no picture is shown there.
- `vercel.json` sets long caching for images.

## Editing

Progress is saved per student in the browser (localStorage) under the student's name; students can back up and restore a JSON file from the top bar.
