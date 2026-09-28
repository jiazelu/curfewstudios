# curfew studios — vercel deployment

this is the current static site, including all pages, fonts, gray placeholders,
updated hero, and black/white text selection. no environment variables or build
step are required.

## recommended: github + vercel

1. unzip this package.
2. create a github repository and upload its contents. vercel.json and the dist
   folder must be at the repository root (not inside an extra folder).
3. open https://vercel.com/new and import that repository.
4. use framework preset "other", an empty build command, and output directory
   "dist". the included vercel.json supplies these settings and clean page URLs.
5. deploy. check the home, work, services, about, and project-detail pages.
6. add a domain from your vercel project's settings > domains if desired.

## alternative: terminal

with node.js installed, open a terminal in the unzipped folder and run:

    npx vercel --prod

sign in when prompted and create a new project. the root is this folder;
vercel serves dist using the included configuration.

## regular updates

edit dist/data.js for project titles, client names, descriptions, and media paths.
edit dist/app.js for page layouts and other text; edit dist/styles.css for styling.
put new assets in dist/assets and reference them using /assets/filename.

for github deployments, commits pushed to the connected production branch
trigger deployment. for terminal deployments, run npx vercel --prod again.
changes made to the ChatGPT-hosted copy do not automatically sync to this export.

source snapshot: b9be869533ee0c01dc4f1b9198d125a40d8f3e4f
