# 春江量化研报网站

这是春江量化的官方研报网站，使用 Jekyll 和 GitHub Pages 构建。

## 结构

- `static/`: 存放研报 PDF 文件
- `index.html`: 根页面，根据浏览器语言自动重定向到中文或英文版本
- `zh/index.md`: 中文主页，列出所有研报
- `en/index.md`: 英文主页，列出所有研报
- `_config.yml`: Jekyll 配置
- `.github/workflows/deploy.yml`: GitHub Actions 工作流，用于自动部署

## 国际化 (i18n)

网站支持中文和英文：
- 根据浏览器语言自动重定向：中文浏览器 -> `/zh/`，其他 -> `/en/`
- 每个页面底部有手动切换语言的链接

## 使用方法

1. 将研报 PDF 文件放入 `static/` 文件夹
2. 推送代码到 GitHub 的 main 分支
3. GitHub Actions 会自动构建并部署到 GitHub Pages

网站地址：https://Chunjiang-Intelligence.github.io/Investment-Report/

## 本地开发

安装依赖：
```bash
bundle install
```

构建站点：
```bash
bundle exec jekyll build
```

预览站点：
```bash
bundle exec jekyll serve
```