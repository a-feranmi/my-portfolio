# Feranmi Amole · Portfolio website

This folder **is** your website. It has no build step: Netlify serves these files exactly as they are.

```
feranmi-portfolio/
├── index.html      ← the whole site (all 6 pages, design, text, code)
├── img/            ← project screenshots ("after" images + raw_*.jpg "before" images)
└── README.md       ← this guide (not shown on the site)
```

---

## 1. Put it live on Netlify (first time, ~5 minutes)

1. **Unzip** `feranmi-portfolio.zip` on your computer. You'll get a folder called `feranmi-portfolio`.
2. Go to **https://app.netlify.com/signup** and sign up (choosing *Sign up with GitHub* is easiest, since you'll use GitHub later).
3. Go to **https://app.netlify.com/drop**.
4. **Drag the `feranmi-portfolio` folder** (the folder itself, not the zip) onto the page.
5. Wait ~20 seconds. Netlify gives you a random address like `jolly-panda-12ab.netlify.app`. Your site is live.
6. Pick your short address: **Site configuration → Change site name** → type `feranmi` (or `feranmiamole`, `feranmi-data` if it's taken) → **Save**.
   Your site is now **https://feranmi.netlify.app**.

### Turn on the contact form emails
The site's forms are already wired for **Netlify Forms** (the free plan includes a monthly allowance of submissions; check Netlify for the current limit).
1. In your site on Netlify: **Forms** (left menu) → **Enable form detection** (if asked) → then redeploy once (drag the folder onto the **Deploys** tab again).
2. A form called **contact** appears. Open **Forms → Form notifications → Add notification → Email notification** and enter `ample.oluwaferanmi26@gmail.com`.
3. Test it: send yourself a message from your live site's Contact page.

> The forms only send on the live Netlify site. Opening `index.html` directly on your computer will show "Sorry, that didn't send" — that's expected.

---

## 2. Updating the site later

### Option A: drag and drop (simplest)
1. Edit the files in your `feranmi-portfolio` folder (see "How to edit" below).
2. Open your site on Netlify → **Deploys** tab.
3. Drag the folder onto the box **"Need to update your site? Drag and drop your site output folder here."**
4. Live in under a minute, same address.

⚠️ Don't use app.netlify.com/drop again for updates; that creates a *new* site with a new address.

### Option B: GitHub (best long-term, edit from any browser or phone)
1. On GitHub (github.com/a-feranmi) → **New repository** → name it `portfolio` → **Create**.
2. Click **uploading an existing file** → drag in everything *inside* the folder (`index.html`, `img`, `README.md`) → **Commit changes**.
3. On Netlify: **Site configuration → Build & deploy → Link repository** (or *Add new site → Import an existing project → GitHub*) → choose `portfolio`. Leave the build command **empty** and publish directory as `/` → **Deploy**.
4. From now on: edit a file on github.com (pencil icon ✏️) or upload a new image → **Commit changes** → Netlify updates the live site automatically in about a minute.

Every past version is kept: **Deploys → pick an older deploy → Publish deploy** to undo a mistake.

---

## 3. How to edit (what to change, where)

Open `index.html` in any text editor (VS Code is free and best; Notepad works). Use **Ctrl+F** to find the text you want to change, change it, save.

| To change… | Search for… |
|---|---|
| Your intro on the home page | `I don't just build dashboards` |
| The typing roles under your name | `const roles=` |
| About page story | `My story` |
| Work experience timeline | `class="timeline"` (each job is one `<div class="job …">` block — copy a block to add a job) |
| Tools (name, confidence 1–5, what you use it for) | `const TOOLS=` (one line per tool; `l:4` = 4 of 5 bars) |
| Featured projects (top 5) | `const PROJ=` |
| More projects (cards) | `const MORE=` |
| "What was wrong" list for each project | `const FIXES=` |
| FAQ questions & answers | `const FAQ=` (each is `['category','Question','Answer']`) |
| Testimonials | `const TEST=` (each is `['quote','Name','Role, Company']`) |
| Hire-me SQL console tables | `const DB=` |
| Email / phone / links | your email address, `wa.me`, `linkedin.com`, `github.com` |

**Replacing a project screenshot:** put the new image in `img/` with the **same file name** (e.g. `img/sales.jpg`), or change the file name in `const PROJ=` (`img:'img/sales.jpg'`). Landscape images about 1600×900 px look best. The "before" image is `img/raw_<name>.jpg`.

**Placeholders:** anything shown in dashed amber on the site has `class="ph"` in the code. Search for `class="ph"` to find what's left to fill in. When everything is filled in, delete the yellow banner by searching for `class="proto"` and removing that one line.

**Tips**
- Text inside `'single quotes'` that needs an apostrophe must be written `\'` (e.g. `I\'m`).
- After editing, open `index.html` in your browser to check it before uploading.
- Not sure? Send the change to Claude and ask for an updated `index.html`.
