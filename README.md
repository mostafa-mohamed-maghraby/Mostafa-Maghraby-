# Mostafa Maghraby – Portfolio Website

Static website (HTML + CSS + JavaScript). No build step, no server, no installs.

## Files (keep these names and this structure exactly)

```
index.html                       ← the whole website (design, animations, functions)
assets/hero.webp                 ← main photo under your name (transparent cut-out)
assets/about.jpg                 ← round photo in "Who is Mostafa?"
assets/Mostafa_Maghraby_CV.pdf   ← file the "Download CV" buttons save
README.md                        ← this file (optional on GitHub)
```

`index.html` must stay in the root of the repository, next to the `assets` folder.
File names are case-sensitive on GitHub (`hero.webp` is not the same as `Hero.webp`).

## Publish on GitHub Pages (no coding, from the browser)

1. Sign in at https://github.com (or create a free account).
2. Click **+** (top right) → **New repository**.
   - Name: `portfolio` (any name), or `YOUR-USERNAME.github.io` to get the shortest link.
   - Choose **Public**. Click **Create repository**.
3. On the empty repository page click **uploading an existing file**.
4. Unzip `portfolio.zip` on your computer. Open the folder and drag **the files inside it**
   (`index.html`, the `assets` folder, `README.md`) into the GitHub upload area.
   Do not drag the outer folder itself, or `index.html` ends up one level too deep.
5. Wait until all files are listed, then click **Commit changes**.
6. Go to **Settings → Pages**.
   - Source: **Deploy from a branch**
   - Branch: **main**, folder **/(root)** → **Save**.
7. Wait 1–2 minutes and refresh the Pages screen. Your link appears at the top:
   - `https://YOUR-USERNAME.github.io/portfolio/` (repository named `portfolio`)
   - `https://YOUR-USERNAME.github.io/` (repository named `YOUR-USERNAME.github.io`)

## Publish with Git (terminal)

```bash
cd portfolio
git init
git add .
git commit -m "Portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
git push -u origin main
```
Then do step 6 above (Settings → Pages).

## Test before and after publishing

- Preview locally: double-click `index.html`. It works offline except the fonts
  (they load from Google Fonts, so you need internet to see the exact typefaces).
- After publishing, check:
  - the logo splash animation, then the dark hero with both red strips scrolling;
  - the tabs are hidden during the intro, then scroll away with the page (not fixed);
  - sections fade in and out when you scroll down and back up;
  - counters (6, 3+, 2) count up each time you reach them;
  - hover or touch the Services boxes, the My Work boxes and the round About photo;
  - **Download CV** (top menu and Contact section) downloads the PDF;
  - Vimeo, H.S.M-Store, Instagram and LinkedIn links open;
  - the contact form opens WhatsApp (your number) with the message already filled in.

## Editing later

- Change a photo or the CV: replace the file inside `assets/` and keep the **same file name**.
  On GitHub: open the file → **…** → Delete, then upload the new one with the same name
  (or use **Add file → Upload files**, which replaces it).
- Change text or links: open `index.html` on GitHub, click the pencil icon, edit, then **Commit changes**.
  Updates appear after about a minute.
- Colors are variables at the top of the `<style>` block (`--red`, `--bg`, `--ink`).

## Good to know

- The contact form opens WhatsApp (wa.me link to your number) with the visitor's name, email, service
  and project details already written. They only press send in WhatsApp, so nothing is stored by the site.
  To change the number, search `201033137003` in `index.html` (it appears in the form code and the WhatsApp links).
- The "Download CV" buttons use normal links, so they work on any host.
- Dark mode follows the visitor's device; the ◐ button in the menu switches it.
- A custom domain can be added later in **Settings → Pages → Custom domain**.
