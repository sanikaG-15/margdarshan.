# MARGDARSHAN — Career Guidance Platform

A responsive, deployment-ready static website to help students explore career directions, compare education pathways, find official scholarship and learning resources, and sketch an education budget.

## What's included

- Career discovery with search, study-stage filters, and career detail dialogs.
- Course pathway cards with typical duration, entry routes, and questions to check before applying.
- Links to official scholarship, education-finance, career-service, entrance-exam, and learning platforms.
- Education affordability planner showing estimated total cost, planned support, family contribution, and remaining gap.
- Downloadable text version of the education budget plan.
- English, Hindi, and Marathi interface options.
- Light and dark themes.
- Responsive layout for desktop, tablet, and mobile.
- Saved career shortlist, language, theme, and budget preferences stored in the visitor's browser.
- No build step, database, backend, API key, framework, or paid service required.
- SEO metadata, favicon, web manifest, and optional security headers for Netlify-compatible hosting.

## Run locally in VS Code

1. Download and extract `margdarshan-deployment.zip`.
2. Open the extracted `margdarshan-site` folder in VS Code.
3. Install the **Live Server** extension if it is not already installed.
4. Right-click `index.html` and choose **Open with Live Server**.
5. The website should open in your browser. Double-clicking `index.html` can also preview the site, but a local server is closer to the hosted environment.

## Deploy to Netlify (beginner-friendly)

1. Extract the ZIP file.
2. Sign in to Netlify and choose its manual deploy / drag-and-drop option for a new site.
3. Upload the **contents** of the `margdarshan-site` folder. Make sure `index.html`, `style.css`, and `app.js` are at the published root; do not upload only the ZIP as a webpage.
4. Netlify will provide a public URL. Open that URL on a phone and computer and test navigation, language switching, themes, external links, and the budget calculator.
5. In Netlify site settings, connect a custom domain if you own one. Supported hosting providers can supply HTTPS automatically.

The `netlify.toml` file sets the publish directory to the project root, and `_headers` defines common security headers for Netlify-compatible static hosting.

## Deploy to GitHub Pages

1. Create a GitHub repository and upload all files from this folder to the repository root.
2. Open **Settings → Pages**.
3. Under the build/deployment source, select **Deploy from a branch**, choose the default branch (usually `main`) and the `/ (root)` folder, then save.
4. When GitHub Pages reports a successful deployment, open the URL shown on the Pages settings screen.
5. Re-test the public URL. GitHub Pages does not apply the Netlify `_headers` file; it is safe to leave it in the repository.

## Deploy to Vercel

Import the repository into Vercel. For a static site, use the project root as the output directory and no build command. If Vercel asks for a framework, choose **Other**. Deploy, then test the published URL.

## Important before public launch

- Add the project owner's real contact/support details if you need a contact channel; no fake contact details are included.
- Check all external links periodically. Government portals, scheme names, deadlines, eligibility rules, and application URLs can change.
- Career and course duration/eligibility notes are broad guidance. Costs are not guaranteed official fee quotes; they depend on the institution, location, course, and year.
- The website does **not** collect accounts or sync data between devices. A saved career list, language preference, theme, and budget are stored in that browser only. Clearing browser storage or switching devices may remove or hide that data.
- MARGDARSHAN is an independent guidance project, not an official government portal. It cannot confirm scholarship eligibility, admission, exam eligibility, employment, or loan approval.
- Before adding analytics, login, forms, a chatbot, or a database, publish an appropriate privacy notice and secure those services.
- Google Fonts are a network-loaded visual enhancement; the layout has local system-font fallbacks when the font service is unavailable.

## Project files

- `index.html` — page structure and content.
- `style.css` — visual design, themes, responsive layouts, and reduced-motion support.
- `app.js` — career/course data, translations, search/filter behavior, shortlist storage, and budget calculator.
- `favicon.svg` — MARGDARSHAN icon.
- `site.webmanifest` — browser site metadata.
- `_headers` — optional security headers for Netlify-compatible hosting.
- `netlify.toml` — Netlify publish directory and response headers.
- `robots.txt` — allows ordinary search-engine crawling.

## Technology

HTML5, CSS3, and vanilla JavaScript. No framework dependency or compilation step is required.
