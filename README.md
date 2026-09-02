# Galgame网站

一个明亮编辑部风格的 Galgame 站点目录，纯 HTML/CSS/JavaScript，可直接部署到 GitHub Pages。

## 部署

1. 将本目录内容推送到 `galwiki.github.io` 仓库的 `main` 分支。
2. 在仓库 Settings → Pages 中选择 GitHub Actions。
3. `pages.yml` 会自动发布根目录，地址为 <https://galwiki.github.io/>。

## 维护目录

编辑 `sites.json` 即可增加站点。首页交互会自动读取名称、分类、简介、标签、评分和更新时间；详情页需要同时新增 `sites/<slug>/index.html`，并把 URL 与日期加入 `sitemap.xml`。

## SEO 与自定义域名

所有 canonical、Open Graph、JSON-LD 和 sitemap URL 当前使用 `https://galwiki.github.io/`。迁移到自定义域名时，请全局替换这些地址，并在仓库根目录新增 GitHub Pages 要求的 `CNAME` 文件。

下载资源站仅作为第三方索引，访问前请自行核验版权、文件安全与当地法律。
