# Pro BMI Calculator

This is a small static BMI calculator (HTML/CSS/JS) that you can deploy to Vercel.

What I added for deployment:
- `index.html` (copy of your `bmi.html`) so the site root serves the app
- `vercel.json` (static build configuration)
- `.gitignore` (basic ignores)

## Quick deploy options

Option A — Deploy via Vercel (recommended, GUI)
1. Create a Git repository (if you don't have one):

```bash
cd /home/navgurukul/Desktop/bmi
git init
git add .
git commit -m "Initial commit: Pro BMI Calculator"
# create a remote on GitHub and push (replace with your remote URL)
git remote add origin <your-git-repo-url>
git push -u origin main
```

2. Go to https://vercel.com, log in, and click "New Project" → import your GitHub repository.
3. Vercel will detect a static project. Set the root if required and deploy. Your site will be live on a vercel.app subdomain.

Option B — Deploy using Vercel CLI (quick, from your machine)
1. Install Vercel CLI if you don't have it:

```bash
npm i -g vercel
```

2. From the project folder run:

```bash
cd /home/navgurukul/Desktop/bmi
vercel --prod
```

Follow the interactive prompts to link/create a Vercel project. The CLI will upload the static files and return the deployment URL.

## Notes & recommendations
- The project is a static site; no build step is necessary.
- If you change file names or add serverless functions later, update `vercel.json` accordingly.
- To keep history across sessions, consider using localStorage in `bmi.js`.

If you want, I can:
- Create a small GitHub Actions workflow to auto-deploy on push, or
- Add localStorage persistence for the history list.
