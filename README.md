# Leonardo de Castro — Applied Data Science & AI Engineering

Editable Astro + Tailwind CSS portfolio starter, prepared for the personal GitHub Pages repository:
`leonardo-f-decastro/leonardo-f-decastro.github.io`.

## 1. Run locally

Requires Node.js 22 or newer and npm.

```bash
npm install
npm run dev
```

Open the localhost URL printed by Astro. Build before publishing:

```bash
npm run build
```

**Important:** Internet connectivity is required to install dependencies. The package cannot be installed in the authoring sandbox, so the build has **not** been executed here. The supplied static HTML preview was rendered separately and visually checked.

## 2. Publish to GitHub Pages

This is a GitHub **user site**, so `astro.config.mjs` intentionally has no `base` prefix.

1. Clone the **new** repository `https://github.com/leonardo-f-decastro/leonardo-f-decastro.github.io` locally.
2. Copy the contents of this project folder into the repository root. Preserve hidden `.github` and `.gitignore` files. Keep the destination repository's existing `.git` folder.
3. Run `npm install` to create a `package-lock.json`, and commit the lockfile. Verify `npm run build` works.
4. In repository **Settings → Pages**, change **Source** from **Deploy from a branch** to **GitHub Actions**.
5. Commit and push to the `main` branch. The workflow in `.github/workflows/deploy.yml` builds and deploys the site.
6. Open **Actions** for deployment progress, then visit `https://leonardo-f-decastro.github.io`.

Example, after cloning:

```bash
npm install
npm run build
git add .
git commit -m "Launch professional Astro portfolio"
git push origin main
```

You may need to refresh the Pages setting after the workflow is committed, and approve workflow access if GitHub asks.

## 3. Content accuracy / publishing checklist

- [ ] Verify project claims, role descriptions, technology lists and ownership against your CV and records.
- [ ] Obtain client or employer permission before adding proprietary architecture, screenshots, KPIs or names.
- [ ] Replace the intentionally synthetic forecasting demo only if you have approved real data.
- [ ] Add an email or LinkedIn contact link once you choose which address/profile should be public.
- [ ] Add a final PDF résumé and link in the navbar/footer after reviewing it.
- [ ] Migrate a subset of notebook posts from the original `data_science_blog` repository, preserving dates and appropriate citations/links.
- [ ] Add descriptive Open Graph imagery if desired.

This starter does **not** claim numerical project results or use confidential client data.

## 4. Files

- `src/layouts/SiteLayout.astro` — shared header, footer, metadata and base styling.
- `src/pages/index.astro` — homepage including forecasting demo.
- `src/pages/work/index.astro` — project collection.
- `src/pages/work/*.astro` — case-study foundations.
- `src/pages/writing.astro` — research and original blog archive.
- `src/pages/about.astro`, `src/pages/contact.astro` — bio and contact.
- `src/styles/global.css` — visual system and responsive styles (includes Tailwind 4 import).
- `public/favicon.svg` — geometric portfolio brand mark.

## 5. GitHub repository recovery

Original public website: `https://leonardodecastro.github.io/`.
Original notebook repository (previously identified): `https://github.com/leonardodecastro/data_science_blog`.

Do not overwrite old Git history or transfer control of the original domain. The new site remains independent.
