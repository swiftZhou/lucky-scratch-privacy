# Lucky Scratch — Privacy Policy (GitHub Pages)

Hosted privacy policy for the **Lucky Scratch** iOS app.

**Live URL (after setup):**  
`https://<your-github-username>.github.io/lucky-scratch-privacy/privacy/`

**Contact:** zhouhaigame@outlook.com

---

## 1. Create the GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `lucky-scratch-privacy`
3. Visibility: **Public** (required for free GitHub Pages)
4. Do **not** add a README, `.gitignore`, or license (this folder already has them)
5. Click **Create repository**

## 2. Push this folder to GitHub

In Terminal, from this directory (`Legal/lucky-scratch-privacy`):

```bash
cd Legal/lucky-scratch-privacy

git init
git add .
git commit -m "Add Lucky Scratch privacy policy for GitHub Pages"
git branch -M main
git remote add origin https://github.com/<your-github-username>/lucky-scratch-privacy.git
git push -u origin main
```

Replace `<your-github-username>` with your GitHub account name.

## 3. Enable GitHub Pages

1. Open the repo on GitHub → **Settings** → **Pages**
2. **Build and deployment** → Source: **Deploy from a branch**
3. Branch: `main` → Folder: **`/docs`**
4. Click **Save**
5. Wait 1–3 minutes. Your site will be at:  
   `https://<your-github-username>.github.io/lucky-scratch-privacy/privacy/`

## 4. Update the iOS app URL

In `SandArtASMR/Controllers/SettingsViewController.swift`, set `AppLinks.privacyPolicy` to your live Pages URL, for example:

```swift
static let privacyPolicy = URL(string: "https://<your-github-username>.github.io/lucky-scratch-privacy/privacy/")!
```

Also paste the same URL in **App Store Connect** → App Privacy → Privacy Policy URL.

## 5. Updating the policy

1. Edit `docs/privacy/index.html` (or sync from `../privacy-policy.html` in the parent `Legal` folder)
2. Update the **Last updated** date at the top of the HTML
3. Commit and push:

```bash
git add docs/privacy/index.html
git commit -m "Update privacy policy"
git push
```

Changes usually appear on GitHub Pages within a few minutes.

---

## Optional: custom domain

If you own a domain (e.g. `sandartasmr.app`):

1. Add a `CNAME` file in `docs/` containing your domain (e.g. `sandartasmr.app`)
2. Configure DNS with your registrar (A/CNAME records per GitHub Pages docs)
3. Enable **Enforce HTTPS** in repo **Settings** → **Pages**

Then update the in-app URL to `https://yourdomain.com/privacy/`.
