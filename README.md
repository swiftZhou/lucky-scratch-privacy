# Lucky Scratch — Web Pages (GitHub Pages)

Public pages for **Lucky Scratch** iOS app — App Store, AdMob, and legal compliance.

**Contact:** zhouhaigame@outlook.com

---

## Live URLs

| Purpose | URL |
|---------|-----|
| **Marketing URL** (homepage) | https://swiftzhou.github.io/lucky-scratch-privacy/ |
| **Technical Support URL** | https://swiftzhou.github.io/lucky-scratch-privacy/support.html |
| **Privacy Policy URL** | https://swiftzhou.github.io/lucky-scratch-privacy/privacy/ |

Legacy redirect: `/support/` → `/support.html`

---

## GitHub Pages setup (important)

If new pages return **404**, GitHub Pages may not be redeploying from `main` + `/docs`. Use this setup:

### Step A — Enable Actions deploy (automatic)

Every push to `main` runs `.github/workflows/deploy.yml` and updates the `gh-pages` branch.

### Step B — Point Pages to gh-pages branch

1. Open https://github.com/swiftZhou/lucky-scratch-privacy/settings/pages
2. **Source:** Deploy from a branch
3. **Branch:** `gh-pages` → **`/ (root)`**
4. Click **Save**
5. Wait 2–5 minutes, then test the URLs above

### Alternative (manual docs deploy)

If you prefer no Actions: Source = `main`, Folder = `/docs`, then click **Save** again after each push to force a rebuild.

---

## AdMob / App Store

- **Marketing URL:** `https://swiftzhou.github.io/lucky-scratch-privacy/`
- **Technical support URL:** `https://swiftzhou.github.io/lucky-scratch-privacy/support.html`
- **Privacy Policy URL:** `https://swiftzhou.github.io/lucky-scratch-privacy/privacy/`

---

## Updating content

```bash
cd Legal/lucky-scratch-privacy
# edit files under docs/
git add .
git commit -m "Update site"
git push
```

If using the Actions workflow, the site updates automatically after the workflow succeeds.
