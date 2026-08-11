# Territory Planning Tool — Demo

Static HTML prototype for the Frontera X Sales Territory Planner. No build step, no dependencies to install — every file is self-contained and can be opened directly in a browser or served as static files.

## Pages

| File | Description |
|---|---|
| `index.html` | Landing page linking to everything below |
| `frontera-my-regions.html` | Sales Regions list + country overview + map |
| `frontera-region-details.html` | Single region: overview, staffing, visit planner, sales assumptions |
| `frontera-country-details.html` | Country overview, Corteva sales data, INSSE validation, data upload |
| `frontera-account.html` | Account settings, units/currency preferences |
| `frontera-signup.html` | Sign up / log in / verify identity flow |
| `frontera-ui-kit-full.html` | Full design system reference + icon library |

## Viewing locally

Just open `index.html` in a browser — no server required. Internal links between pages are relative, so as long as all files stay in the same folder, navigation between pages works.

## Deploying with GitHub Pages

1. Go to **Settings → Pages** in this repo
2. Under "Build and deployment", set **Source** to `Deploy from a branch`
3. Set branch to `main` and folder to `/ (root)`
4. Save — your site will be live at `https://<username>.github.io/<repo-name>/` within a minute or two

## Notes

- These are static prototypes with demo data — no backend, no real authentication, no persistence between sessions.
- Map tiles are served from CARTO's free Positron basemap (no API key required).
- Some interactive elements (file upload, delete confirmation, etc.) simulate the real behavior with `alert()` placeholders — swap these for real API calls when integrating.
