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
- `vercel.json` sets long caching for images.

## Editing

Progress is saved per student in the browser (localStorage) under the student's name; students can back up and restore a JSON file from the top bar.

## Navigation, menu and accessibility

- The three proficiency levels are buttons in the top bar (each ring shows progress, a green check means the checkpoint is done). The tabs for the current level sit under the bar, so lessons and the Stop-Motion Studio get the full width of the screen.
- The Menu button (three lines) is on the landing page and in the top bar. It holds Portfolio, Backup, Switch student, the Word bank and every setting.
- Display and accessibility settings are saved per device under `splitDecision.settings`, so they work before sign-in: text size, light/dark, high contrast, calm animations, read aloud (with a slower speed and select-to-hear), dyslexia-friendly text (Lexend), reading ruler, color-blind friendly colors, and Word help with optional Spanish.
- Hints, fewer answer choices and the frame-label option are saved with each student. Supports in use are listed on the portfolio.
- The app never follows the device's reduced-motion preference; calm motion is chosen in the Menu.
