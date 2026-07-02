# Lucky Scratch — Privacy Policy (GitHub Pages)

Hosted privacy policy for the **Lucky Scratch** iOS app.

**Live URL:**  
https://swiftzhou.github.io/lucky-scratch-privacy/privacy/

**Contact:** zhouhaigame@outlook.com

---

## Enable GitHub Pages (required — do this once)

The repo files are correct. Pages only works after you turn it on in GitHub settings.

1. Open **Settings → Pages**:  
   https://github.com/swiftZhou/lucky-scratch-privacy/settings/pages

2. Under **Build and deployment** → **Source**, choose:  
   **Deploy from a branch**  
   (Do **not** use “GitHub Actions” — that caused `deployment_queued` timeouts.)

3. Under **Branch**:
   - Branch: **`main`**
   - Folder: **`/docs`**
   - Click **Save**

4. Wait 1–3 minutes. A green banner should show:  
   `Your site is live at https://swiftzhou.github.io/lucky-scratch-privacy/`

5. Open the privacy page:  
   https://swiftzhou.github.io/lucky-scratch-privacy/privacy/

### If it still shows 404

- Confirm **Source** is **Deploy from a branch**, not GitHub Actions.
- Confirm folder is **`/docs`**, not `/ (root)`.
- Repo must be **Public**.
- Wait up to 10 minutes after first save, then hard-refresh the browser.

---

## iOS app URL

Already set in the app:

```swift
static let privacyPolicy = URL(string: "https://swiftZhou.github.io/lucky-scratch-privacy/privacy/")!
```

Use the same URL in **App Store Connect** → Privacy Policy URL.

---

## Updating the policy

1. Edit `docs/privacy/index.html`
2. Update the **Last updated** date
3. Commit and push:

```bash
git add docs/privacy/index.html
git commit -m "Update privacy policy"
git push
```

Changes appear on GitHub Pages within a few minutes.
