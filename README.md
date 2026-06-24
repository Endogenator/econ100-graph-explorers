# ECON 100 Graph Explorers: deploy and link

These are self-contained interactive HTML tools. Canvas sandboxes uploaded HTML and strips the
JavaScript, so they must be hosted somewhere that runs scripts. Vercel does, and keeps the URLs
stable so your Canvas links never break when a tool is updated.

## Files in this folder

- index.html ........................ landing page that lists every tool
- Econ100_InteractiveGraphLab_01_SupplyDemand.html
- Econ100_InteractiveGraphLab_02_FirmProfitLoss.html   (Chapters 6 and 7)
- Econ100_InteractiveGraphLab_03_PPF.html
- Econ100_InteractiveGraphLab_04_Monopoly.html
- Econ100_InteractiveGraphLab_05_ADAS.html ........... ADD THIS YOURSELF (your existing AD/AS engine,
  renamed to this, or edit the link in index.html to match your filename)

## Deploy with GitHub + Vercel (recommended, stable and updatable)

1. Create a new GitHub repository, for example econ100-graph-explorers.
2. Add every file in this folder to the repo root and push.
3. In Vercel, New Project, import that repo. No framework, no build step, it is static.
4. Deploy. You get a URL like https://econ100-graph-explorers.vercel.app

To update a tool later: replace the file in the repo, push, and Vercel redeploys to the same URL.
Your Canvas links keep working untouched.

## Deploy faster (no repo)

In this folder, run the Vercel CLI:

    vercel

Follow the prompts. Or drag this folder onto the Vercel dashboard, New Project, Deploy.

## The resulting URLs

- Landing page:  https://YOUR-PROJECT.vercel.app/
- Each tool:     https://YOUR-PROJECT.vercel.app/Econ100_InteractiveGraphLab_03_PPF.html
                 (same pattern for each filename)

## Point the Canvas module pages at these

In each Canvas module page you already built, replace REPLACE-WITH-FILE-LINK in the button with
the matching Vercel tool URL above, then delete the red instructor line. The button opens the tool
in a new tab, scripts intact.

If you would rather link one place, point a single Canvas link at the landing page URL and students
reach every tool from there.
