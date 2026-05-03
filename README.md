# 妈妈饮食方案 PWA 网页包

这是一个静态 PWA 网页包，可部署到 GitHub Pages、Netlify 或 Vercel。部署后用 iPhone Safari 打开发布后的 `https://...` 地址，即可通过“分享 → 添加到主屏幕”添加成桌面 App 图标。

## 文件说明

- `index.html`：手机优化版饮食方案主页面
- `manifest.webmanifest`：PWA 应用名称、图标、启动方式配置
- `sw.js`：Service Worker，用于基础离线缓存
- `icons/`：PWA 和 iPhone 主屏幕图标
- `_headers`：Netlify 可读取的响应头配置
- `vercel.json`：Vercel 可读取的响应头配置
- `.nojekyll`：GitHub Pages 使用，避免 Jekyll 处理静态文件

## 本地测试

把本文件夹放到电脑上，在该目录运行：

```bash
python3 -m http.server 8080
```

然后浏览器打开：

```text
http://localhost:8080
```

注意：PWA 安装和 Service Worker 正式测试需要 `https://`，所以建议部署到线上平台后再用手机测试。
