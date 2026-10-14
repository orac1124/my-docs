# 我的技术文档（my-docs）

基于 MkDocs 的示例文档项目，使用 GitHub Actions 自动构建并部署到 GitHub Pages。

## 在线访问

<https://orac1124.github.io/my-docs/>

## 本地预览

```bash
pip install mkdocs-material
mkdocs serve
```

## 部署流程

推送到 main 分支（docs/** 或 mkdocs.yml 发生变更）时，GitHub Actions 自动执行：

1. 检出代码
2. 配置 Python 3.9 环境
3. 安装 mkdocs-material
4. `mkdocs build` 构建静态站点到 site 目录
5. 将 site 目录发布到 gh-pages 分支，由 GitHub Pages 托管
