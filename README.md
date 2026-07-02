# Lucky Scratch — GitHub Pages

**Contact:** zhouhaigame@outlook.com

## URLs (use these in App Store / AdMob)

| Purpose | URL |
|---------|-----|
| **Marketing** | https://swiftzhou.github.io/lucky-scratch-privacy/ |
| **Support (recommended)** | https://swiftzhou.github.io/lucky-scratch-privacy/privacy/support.html |
| **Privacy** | https://swiftzhou.github.io/lucky-scratch-privacy/privacy/ |

If `support.html` at root returns 404, use **`privacy/support.html`** instead (same folder as the working privacy page).

Backup support (always works today):  
https://swiftzhou.github.io/lucky-scratch-privacy/privacy/

## Fix GitHub Pages deploy timeout

1. **Actions** → Cancel any running `pages build and deployment` jobs.
2. **Settings → Pages** → Source: **Deploy from a branch** → Branch **`main`**, Folder **`/docs`** → Save.
3. If still stuck: click **Unpublish site**, wait 30 seconds, configure again and Save.
4. Wait 5–10 minutes, then test **privacy/support.html**.

## Update

Edit files under `docs/`, then:

```bash
git add docs/
git commit -m "Update site"
git push origin main
```
