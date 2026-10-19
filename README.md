# BREATHE Cost of Bar — Online website

## Publish via GitHub + Netlify
1. Create a private GitHub repository.
2. Upload `index.html`, `netlify.toml`, and `README.md` to the repository root.
3. In Netlify, choose Add new project > Import existing project > GitHub.
4. Select the repository, leave Build command empty, and set Publish directory to `.`.
5. Deploy. Netlify provides an HTTPS URL. Updates pushed to GitHub deploy automatically.

## Important data limitation
This version uses browser `localStorage` (`breathe_bar_cost_v1`). Hosting it on Netlify does NOT sync records across devices or provide login. Export Backup JSON from the old file before migrating. The old `file://` origin and new HTTPS origin have separate storage. Open the deployed site, use Backup & Data > Restore Backup, and verify ingredients and recipes.

For shared editing and login, a database backend, authentication, and access-control policies must be implemented and tested separately before staff use. Do not upload backups containing business data to the GitHub repository.
