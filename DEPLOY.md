# Team21 Academy Bible School — Deployment Guide

## 📁 What's in this package

```
t21bible/
├── index.html          ← The entire app (all 8 courses, all features)
├── manifest.json       ← PWA install config
├── sw.js               ← Service Worker (offline mode)
├── data/
│   └── courses.js      ← All course & lesson content (EN + FR)
└── assets/
    └── icons/          ← App icons (8 sizes for all devices)
        ├── icon-72.png
        ├── icon-96.png
        ├── icon-128.png
        ├── icon-144.png
        ├── icon-152.png
        ├── icon-192.png
        ├── icon-384.png
        └── icon-512.png
```

---

## 🚀 Deploy to GitHub Pages (Free — step by step)

### Step 1 — Create a GitHub account
If you don't have one: go to https://github.com and sign up (free).

---

### Step 2 — Create a new repository

1. Click the **+** button (top-right) → **New repository**
2. Name it exactly: `t21-bible-school`
   *(or any name you like — it becomes part of the URL)*
3. Set visibility: **Public** ✓
4. Leave everything else as default
5. Click **Create repository**

---

### Step 3 — Upload your files

On the new repository page:

1. Click **"uploading an existing file"** (or drag & drop)
2. Upload these files **maintaining the folder structure**:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `data/courses.js`  ← must be inside a `data` folder
   - All 8 files from `assets/icons/`  ← must be inside `assets/icons/`

**How to upload with folders:**
- On GitHub's upload page, you can drag entire folders
- Or click "choose your files" and select all files
- For `data/courses.js` — after upload, GitHub will ask for a path. Type: `data/courses.js`
- For icons — type: `assets/icons/icon-72.png` etc.

3. Scroll down → add a commit message: `Initial deploy`
4. Click **Commit changes**

---

### Step 4 — Enable GitHub Pages

1. In your repository, click **Settings** (top menu)
2. In the left sidebar, click **Pages**
3. Under "Source" → select **Deploy from a branch**
4. Branch: select **main** → folder: **/ (root)**
5. Click **Save**

GitHub will show: *"Your site is being published..."*
Wait 1–2 minutes, then it shows:
> ✅ Your site is live at: `https://YOUR-USERNAME.github.io/t21-bible-school/`

---

### Step 5 — Test on your phone

1. Open the URL on your Android or iPhone
2. You'll see an **"Install App"** banner appear after a few seconds
3. Tap **Install** → the app appears on your home screen like a native app
4. It works fully **offline** once installed

---

## 🌐 Custom Domain (Optional)

If you want `bible.team21academy.com` instead of a GitHub URL:

1. In your domain registrar (e.g. Namecheap, GoDaddy), add a CNAME record:
   - Host: `bible`
   - Points to: `YOUR-USERNAME.github.io`
2. In GitHub Pages Settings → Custom domain: type `bible.team21academy.com`
3. Check **Enforce HTTPS**

---

## 📲 Sharing the App

Once live, share it this way on WhatsApp or in church:

> *"Download our free Bible School app — works offline on any phone!*
> *Visit: https://YOUR-USERNAME.github.io/t21-bible-school/*
> *Then tap 'Install' to add it to your home screen."*

---

## 🔄 Updating Content

To add lessons or fix anything:
1. Go to your GitHub repository
2. Click on the file you want to edit (`data/courses.js` for content)
3. Click the ✏️ pencil icon
4. Make your changes
5. Commit — the live site updates in ~30 seconds

---

## ✅ Feature Checklist

| Feature | Status |
|---|---|
| 8 fully written courses (EN + FR) | ✅ |
| Onboarding (name + language) | ✅ |
| Language toggle EN/FR | ✅ |
| Quiz engine with explanations | ✅ |
| Progress tracking per lesson | ✅ |
| Progress dashboard on Profile | ✅ |
| Notes saved locally | ✅ |
| Verse bookmarks | ✅ |
| Completion certificates (Canvas) | ✅ |
| WhatsApp share / check-in | ✅ |
| PWA install (home screen) | ✅ |
| Full offline mode | ✅ |
| Mobile-first responsive design | ✅ |
| No server / no backend needed | ✅ |
| Free hosting on GitHub Pages | ✅ |

---

## 📞 Support

Team21 Academy · Yaoundé, Cameroon  
team21academy.com
