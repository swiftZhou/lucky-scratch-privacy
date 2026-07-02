# Lucky Scratch — GitHub Pages

**Contact:** zhouhaigame@outlook.com

## URLs

| Page | URL |
|------|-----|
| Marketing | https://swiftzhou.github.io/lucky-scratch-privacy/ |
| Support | https://swiftzhou.github.io/lucky-scratch-privacy/support.html |
| Privacy | https://swiftzhou.github.io/lucky-scratch-privacy/privacy/ |

Backup support (if `support.html` is not live yet):  
https://swiftzhou.github.io/lucky-scratch-privacy/privacy/#support

## Fix Pages timeout (important)

1. Open **Actions** and **Cancel** any running `pages build and deployment` workflows.
2. Open **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: **`main`**
   - Folder: **`/docs`**
   - Save
3. Wait 3–10 minutes, then open the Support URL above.

Do **not** use GitHub Actions as the Pages source. All site files are in the `docs/` folder.

## Update site

```bash
cd Legal/lucky-scratch-privacy
# edit files under docs/
git add docs/
git commit -m "Update site"
git push origin main
```
