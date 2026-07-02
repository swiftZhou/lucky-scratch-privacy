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

---

## Where to use these URLs

### App Store Connect
- **Privacy Policy URL:** `.../privacy/`
- **Support URL:** `.../support.html`
- **Marketing URL** (optional): `.../` (root homepage)

### Google AdMob (after App Store approval)
When linking your iOS app in AdMob:
- **Marketing URL:** `https://swiftzhou.github.io/lucky-scratch-privacy/`
- **Technical support URL:** `https://swiftzhou.github.io/lucky-scratch-privacy/support.html`

Google crawls these pages to verify app name, bundle ID, and contact info.

### iOS app (in-app)
Privacy Policy link in Settings already points to `.../privacy/`.

---

## After App Store approval

Edit `docs/index.html` and replace the App Store search link with your real App Store URL:

```html
<a href="https://apps.apple.com/app/idYOUR_APP_ID">Download on the App Store</a>
```

Then commit and push.

---

## Updating content

```bash
cd Legal/lucky-scratch-privacy
# edit docs/index.html, docs/support/index.html, or docs/privacy/index.html
git add .
git commit -m "Update site content"
git push
```

Changes appear on GitHub Pages within a few minutes.

---

## GitHub Pages setup

**Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` → Folder: **`/docs`**
