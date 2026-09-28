# 恢复为没有 Portfolio 页的状态

## 需要替换

将 `_config.yml` 放回网站仓库根目录，导航会恢复为：About、Publications、Experience、Awards、中文。

## 需要删除

请从仓库中删除以下文件：

- `portfolio.html`
- `portfolio-projects/` 整个文件夹（里面是 8 个 Portfolio 详情页）

如果你的详情页文件夹名称是 `_projects/`，请只删除本次新增的 `research-1.html` 至 `research-4.html` 和 `design-1.html` 至 `design-4.html`，保留原有的作品集项目文件。

`assets/css/layout.css` 里新增的 Portfolio 样式即使暂时保留，也不会显示；如果希望完全清理，可以删除其中从 `/* Portfolio only` 开始的部分，但不是必须的。
