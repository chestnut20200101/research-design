# Research × Design

设计研究课程项目的最终静态网站。

## 网站文件

- `index.html` — 完整网站入口文件（图片已内嵌，无需额外资源文件）
- `.gitignore` — 忽略常见系统文件

## Cloudflare Pages 部署

1. 将本仓库连接到 Cloudflare Pages。
2. Production branch 选择 `main`。
3. Framework preset 选择 None / 无框架。
4. Build command 留空（如界面要求可使用 `exit 0`）。
5. Build output directory 使用 `.`。
6. 部署后，仓库根目录的 `index.html` 即为网站首页。

## Vercel 部署

1. 在 Vercel 导入本 GitHub 仓库。
2. Framework Preset 选择 `Other`。
3. Build Command 留空。
4. 使用仓库根目录作为静态网站目录。
5. 部署即可。

后续只要更新 `main` 分支中的 `index.html`，连接 GitHub 的托管平台即可自动重新部署。
