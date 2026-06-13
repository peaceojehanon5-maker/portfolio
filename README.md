# Peace Ojehanon — Portfolio

A single-page personal portfolio. Built as one self-contained `index.html`
(HTML + CSS + JavaScript inline, fonts loaded from Google Fonts), so it works
anywhere static files are served and needs no build step.

```
portfolio/
├── index.html              ← the whole site
├── Peace_Ojehanon_CV.pdf   ← linked by the "Download CV" buttons
└── README.md               ← this file
```

---

## Put it online with GitHub Pages (free)

1. **Create a GitHub account** at https://github.com if you don't have one.
2. **Create a new repository.** The simplest option: name it
   `your-username.github.io` (replace with your actual username) — GitHub
   serves that one at the root of your personal Pages URL. Any other name
   works too; see step 5.
3. **Upload the files.** On the new repo page click **Add file → Upload files**,
   then drag in `index.html` and `Peace_Ojehanon_CV.pdf`. Commit.
4. **Turn on Pages.** Repo **Settings → Pages**. Under *Build and deployment*,
   set **Source = Deploy from a branch**, **Branch = main**, folder **/(root)**.
   Save.
5. **Wait ~1 minute**, then visit your site:
   - repo named `your-username.github.io` → `https://your-username.github.io`
   - any other repo name (e.g. `portfolio`) → `https://your-username.github.io/portfolio`
6. **Add the link** to your CVs and LinkedIn once it's live.

That's it — every time you upload a changed `index.html`, the live site updates.

### Prefer the command line?
```bash
git init
git add .
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

---

## Free alternatives (all fine, pick one)

| Host | How | Custom domain |
|------|-----|---------------|
| **GitHub Pages** *(recommended)* | as above | yes, free |
| **Cloudflare Pages** | connect the repo at pages.cloudflare.com | yes, free |
| **Netlify** | drag the folder onto app.netlify.com/drop | yes, free |
| **GitLab Pages** | push repo + add a small CI file | yes, free |

---

## Things to know about the links

- **Live + Code links are already wired in** to point at
  `github.com/peaceojehanon5-maker/...`. The two "View live" projects
  (audio DSP, QGIS) are already deployed and work now. The three "Code"
  links (audio-dataset-pipeline, herb-image-classifier, hotel-revenue-dss)
  resolve as soon as you create those repos with the same names — see the
  separate **GIT_UPLOAD_GUIDE.md**.
- **LinkedIn article links** all point to your LinkedIn profile. If you want
  each to open its specific article, replace the `href` on each line with the
  article's direct URL.

## Editing tips
- All colours live in the `:root` block at the top of the `<style>` section.
  The amber accent is `--amber`; the brand navy is `--navy`.
- The site is fully readable with JavaScript disabled; the JS only adds the
  sticky-header tint, mobile menu, scroll reveals and active-nav highlighting.
- Responsive down to small phones, keyboard-focusable, and honours
  "reduce motion" system settings.
