# ⚠️ GitHub Pages 修复指南（必读）

## 报错原因

`actions/deploy-pages@v5` + `Deployment cancelled` 表示：

**Pages 的 Source 选成了「GitHub Actions」**，但 Actions 部署被取消/冲突，网站会 **404**。

本仓库 **不需要** 任何 Actions workflow，请用 **分支部署**。

---

## 正确设置（3 步）

### 1. 取消 Actions

打开：https://github.com/swiftZhou/lucky-scratch-privacy/actions  

取消所有正在运行的 workflow（包括 `pages build and deployment`、`deploy-pages`）。

### 2. 改 Pages 源（关键）

打开：https://github.com/swiftZhou/lucky-scratch-privacy/settings/pages

| 设置项 | 必须选 |
|--------|--------|
| **Source** | **Deploy from a branch**（不要选 GitHub Actions） |
| **Branch** | `main` |
| **Folder** | **`/docs`** |
| 然后 | **Save** |

若之前点过 Unpublish，Save 后会重新发布。

### 3. 等待 3–10 分钟

测试这些链接（都应返回 200）：

- https://swiftzhou.github.io/lucky-scratch-privacy/
- https://swiftzhou.github.io/lucky-scratch-privacy/privacy/
- https://swiftzhou.github.io/lucky-scratch-privacy/privacy/support.html

---

## AdMob / App Store 填这些 URL

| 用途 | URL |
|------|-----|
| 营销网址 | `https://swiftzhou.github.io/lucky-scratch-privacy/` |
| 技术支持 | `https://swiftzhou.github.io/lucky-scratch-privacy/privacy/support.html` |
| 隐私政策 | `https://swiftzhou.github.io/lucky-scratch-privacy/privacy/` |

---

## 不要做的事

- ❌ 不要选 **GitHub Actions** 作为 Pages Source  
- ❌ 不要添加 `.github/workflows` 部署 workflow  
- ❌ 不要使用 `gh-pages` 分支（已删除）

---

## 仍然失败？

1. Settings → Pages → **Unpublish** → 等 30 秒  
2. 再按上面 Step 2 重新 **Save**  
3. 若还是不行，新建仓库 `lucky-scratch-web`，只放 `docs/` 内容，重新开 Pages

Contact: zhouhaigame@outlook.com
