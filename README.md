# A1 Deutsch Quiz – Deploy on Render

Static site. No build step required.

## Deploy (GitHub method – recommended)

1. Create a free account at https://render.com
2. Push this folder to a GitHub repository
3. In Render Dashboard → **New** → **Static Site**
4. Connect the GitHub repo
5. Settings:
   - **Build Command**: leave empty (or `echo ok`)
   - **Publish Directory**: `.`  (or the folder that contains index.html)
6. Click **Create Static Site**

Your site will get a URL like:
`https://a1-deutsch-quiz.onrender.com`

## Deploy (manual drag & drop alternative)

Render static sites are usually Git-connected. You can also use any static host
(Netlify Drop, Cloudflare Pages, GitHub Pages) by uploading this folder.

## Notes

- IndexedDB statistics stay in each user's browser (not on the server)
- HTTPS is automatic on Render → PWA install works
- Free tier may spin down after inactivity; first load can be a few seconds
