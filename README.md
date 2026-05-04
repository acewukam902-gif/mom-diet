# 妈妈高性价比饮食计划 PWA

这是一个静态 PWA 网页包，可部署到 GitHub Pages、Netlify、Vercel 或任意 HTTPS 静态站点。

## 文件说明

- `index.html`：手机优先版饮食计划页面
- `manifest.webmanifest`：PWA 应用名称、图标、启动方式
- `sw.js`：离线缓存 Service Worker
- `icons/`：桌面图标与 iOS 图标
- `.nojekyll`：GitHub Pages 使用，避免 Jekyll 处理静态文件
- `_headers`：Netlify 可读取的缓存/安全头配置
- `vercel.json`：Vercel 静态部署配置

## GitHub Pages 上传

1. 新建仓库。
2. 不要只上传外层文件夹；请把本文件夹内部所有文件直接放到仓库根目录。
3. 仓库根目录应直接看到 `index.html`、`manifest.webmanifest`、`sw.js`、`icons/`。
4. Settings → Pages → Source: Deploy from a branch → Branch: main → Folder: /(root)。
5. 等待部署完成后，用 `https://用户名.github.io/仓库名/` 打开。

## 手机安装

- iPhone：Safari 打开网址 → 分享 → 添加到主屏幕。
- Android：Chrome 打开网址 → 右上角 ⋮ → 安装应用 / 添加到主屏幕。

