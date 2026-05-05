# Jian Wu — Academic Homepage (Hugo Blox)

🌐 **Live site**: https://jackng88.github.io/jianwu88/

Built with **Hugo** + **Hugo Blox Academic CV** theme (same as rongtingting.github.io).

---

## Quick Start (5 steps)

### Step 1 — Install Hugo (Mac)
```bash
brew install hugo go
hugo version   # needs v0.112+
```

### Step 2 — Clone & init theme
```bash
git clone https://github.com/jackng88/jianwu88.git
cd jianwu88
hugo mod get   # downloads the theme automatically
```

### Step 3 — Preview locally
```bash
hugo server
# Open http://localhost:1313/jianwu88/
```

### Step 4 — Add your photo
Put your photo at:
```
assets/media/author.jpg    ← rename your photo to author.jpg
```
(Square image, min 400×400px recommended)

### Step 5 — Push to GitHub
```bash
git add .
git commit -m "Add Hugo academic site"
git push origin main
```

Then: GitHub repo → **Settings → Pages → Source: GitHub Actions** ✅

---

## File Structure

```
jianwu88/
├── hugo.yaml                          ← Main config (baseURL, menus, params)
├── content/
│   ├── _index.md                      ← Homepage sections layout
│   ├── authors/admin/_index.md        ← YOUR BIO (edit this!)
│   ├── publication/                   ← Your 9 papers (pre-filled)
│   │   ├── 2017-kdm2b/
│   │   ├── 2018-chromatin/
│   │   ├── 2019-epsc-nature/
│   │   ├── 2020-glycodelin/
│   │   ├── 2021-bovine-epsc/
│   │   ├── 2022-erv-tet1/
│   │   ├── 2023-human-epsc/
│   │   ├── 2023-ctc/
│   │   └── 2024-epsc-criteria/
│   ├── post/                          ← Blog posts
│   │   └── scrna-tutorial/
│   └── project/                       ← Research projects
│       └── lung-genomics/
├── assets/media/
│   └── author.jpg                     ← PUT YOUR PHOTO HERE
└── .github/workflows/deploy.yml       ← Auto-deploy on push
```

---

## What to edit

| What | File |
|------|------|
| Bio, interests, education | `content/authors/admin/_index.md` |
| Homepage sections order | `content/_index.md` |
| Navigation menu | `hugo.yaml` (menus section) |
| Add new blog post | `hugo new content/post/my-post/index.md` |
| Add new publication | `hugo new content/publication/my-paper/index.md` |
| Site colors/font | `hugo.yaml` (params.appearance) |

---

## Pages you get (like Rongting)

| URL | Content |
|-----|---------|
| `/jianwu88/` | Home: Bio + Experience + Publications + Contact |
| `/jianwu88/post/` | Blog posts list |
| `/jianwu88/publication/` | All publications |
| `/jianwu88/project/` | Research projects |
| `/jianwu88/post/scrna-tutorial/` | Individual post |
