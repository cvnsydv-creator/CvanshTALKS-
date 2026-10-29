# CvanshTALKS - UPSC Study Hub

A mobile-friendly, dark-premium static website starter for a public UPSC CSE study platform.

## Included
- `index.html`: complete responsive website in one file.
- `README.md`: this setup and deployment guide.

## Honest feature status
This is a static starter site. It does **not** currently have:
- student login or accounts
- database or cloud-saved study progress
- working quiz engine
- admin content publishing panel
- community/chat/comments
- live current-affairs feed

Those features require a real backend and security rules. The current-affairs cards are explicitly sample placeholders. Replace them with verified, dated content before treating the section as live.

## Publish from Android with GitHub + Cloudflare Pages

### A. Create the GitHub repository
1. Open https://github.com/ in Chrome and sign in/create an account.
2. Tap `+` then `New repository`.
3. Repository name: `cvanshtalks` (or your preferred name).
4. Choose **Public** if you want the source code public. Do not upload private documents, passwords, API keys or student data.
5. Create the repository.

### B. Add the website file
1. Open the new repository.
2. Tap **Add file** → **Create new file**.
3. Enter the exact filename `index.html`.
4. Open the supplied `index.html` file from this ZIP in a text editor on your phone, select all, copy, then paste it into GitHub's editor.
5. Scroll down to **Commit changes**. Commit directly to the main branch.
6. Optional: add this `README.md` in the same way, or upload it from the ZIP.

### C. Deploy using Cloudflare Pages
1. Open https://dash.cloudflare.com/ and sign in/create an account.
2. Find **Workers & Pages** → **Create** → **Pages** → **Connect to Git** (wording may vary).
3. Connect GitHub and select your `cvanshtalks` repository.
4. Project name: `cvanshtalks`.
5. For a plain HTML site, choose no framework / `None`.
6. Build command: leave blank.
7. Build output directory: `/` or `.` as accepted by the dashboard. If the dashboard requires a directory, use the repository root (`/` or `.`); do not enter `dist` because this site does not build into a dist folder.
8. Start deployment and wait for the deployment to finish.
9. Open the generated `*.pages.dev` URL on your phone. Test the navigation and all links.

### D. Updating the website
1. Open the GitHub repository.
2. Open `index.html` → pencil/edit icon.
3. Make your changes and commit them.
4. Cloudflare Pages should redeploy after the commit. Check the deployment status if changes do not appear.

## Important before inviting students
- Replace sample current-affairs cards with dated, source-linked material.
- Share only content you created or have permission to redistribute. Linking to official/public sources is safer than rehosting copyrighted PDFs.
- Do not collect passwords or student information until a real authentication/database setup is implemented and tested.
- Never put service-role keys, private tokens or secrets in `index.html` or any public GitHub repository.
- A free plan has usage/storage limits; it is not unlimited.
