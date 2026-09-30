# Krishna Fit

Privacy-first fitness dashboard with editable goals, macros, built-in workouts, WHOOP alternate-workout calories, recovery, supplements, reminders, and lab tracking.

## Current features
- Edit start weight, goal weight, start date, goal date, calories and protein
- Default personal goal: 98 kg → 78 kg by March 30, 2027 (fully editable)
- Meal/macro logging
- App workout / Different workout / Rest day
- WHOOP workout manual entry and CSV import
- WHOOP calories shown separately with optional 0–100% eat-back
- Recovery + sauna guidance
- Supplement list, doses/notes, times, adherence checkboxes
- Browser notifications while app is open
- Copyable supplement schedule for ChatGPT reminder automations
- Blood-test report files stored locally in IndexedDB
- Lab value tracking using the report's own reference range
- Conservative lab-aware training, lifestyle and supplement considerations
- PWA manifest/service worker

## Run locally
```bash
python3 -m http.server 8000
```
Open `http://localhost:8000`.

## GitHub Pages
1. Create a repo called `krishna-fit`.
2. Put `index.html`, `manifest.json`, `sw.js`, and `README.md` in the repo root.
3. GitHub → Settings → Pages → Deploy from branch → `main` / root.
4. Open the Pages URL in iPhone Safari → Share → Add to Home Screen.

## Privacy and medical boundaries
Personal logs and attached reports stay in the browser in this standalone edition and are not part of the repository. Lab guidance is informational, not diagnosis or treatment. The app does not prescribe supplement doses. Iron, high-dose vitamins, kidney/liver-related supplementation, or major workout changes around abnormal labs should be clinician-guided.

Closed-app Web Push, automated email reminders and live WHOOP OAuth require backend services and are not included in this standalone build.