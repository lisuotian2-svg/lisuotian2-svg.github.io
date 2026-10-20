# LI.DEV 个人作品集 V2

部署：将 index.html、style.css、app.js、posts.json 和 blog/ 文件夹放到 GitHub Pages 仓库的 main 分支根目录。Settings → Pages → Deploy from a branch → main / (root)。

## 功能
- GitHub API 自动读取 `lisuotian2-svg` 公开且非 fork 的仓库；私有仓库不展示。
- 中英文切换、明暗主题切换，浏览器 localStorage 记忆偏好。
- 响应式页面、滚动动画、尊重减少动态效果设置。
- `posts.json` 管理文章列表；`blog/*.html` 存放文章正文。
- GitHub 数据受公开 API 速率限制；失败时显示提示，不暴露密钥。

## 新增博客
复制 blog/welcome.html 为 blog/新文章.html，修改内容，并在 posts.json 添加一条对应 slug、日期、中文英文标题及摘要。注意 JSON 语法。

## 注意
博客示例文章仅为占位内容。GitHub 公共 API 的统计可能有缓存或请求限制。浏览器直接双击 index.html 时 fetch 可能被限制，建议使用 `python -m http.server 8000` 本地预览或发布后测试。
