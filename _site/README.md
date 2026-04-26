# 春江量化研报网站

这是春江量化的官方研报网站，使用 Jekyll 和 GitHub Pages 构建。

## 结构

- `static/`: 存放研报 PDF 文件
- `index.md`: 主页，列出所有研报
- `_config.yml`: Jekyll 配置
- `.github/workflows/deploy.yml`: GitHub Actions 工作流，用于自动部署

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