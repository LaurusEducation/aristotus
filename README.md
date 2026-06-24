# Aristotus College — Static Site

Plain HTML/CSS, no build step. Four pages with a shared nav.

```
index.html        Home
about.html        About
programmes.html   Programmes
contact.html      Contact
css/style.css     Shared styles
images/           Put hero.jpg and other images here
```

## Edit content
Open each `.html` file and replace the placeholder text (look for "Replace this…").
The nav bar is repeated in each file — if you add a page, update the nav in all four.

## Add the hero image
Drop a file named `hero.jpg` into `images/`. The homepage hero references it.

## Contact form
GitHub Pages cannot send email by itself. To make the form work:
1. Sign up free at https://formspree.io
2. Create a form, copy your endpoint
3. In `contact.html`, replace `YOUR_FORM_ID` in the `action="…"` URL.

## Deploy to GitHub Pages
From the repo folder (e.g. `aristitus_web`):

```bash
git add .
git commit -m "Add static site"
git push origin main
```

Then on GitHub: repo **Settings → Pages → Source: Deploy from a branch →
Branch: main / root → Save**. Your site appears at
`https://<username>.github.io/<repo>/` within a minute or two.

## Custom domain (optional)
In Settings → Pages, add your domain (e.g. `aristotuscollege.com`) and create the
DNS records GitHub shows you. Add a file named `CNAME` containing just the domain.
