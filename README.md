# BI Xia 畢夏 — 个人主页

这是整理后的 Jekyll / GitHub Pages 源码。五页分别为 About、Publications、Experience、Awards、中文。

## 替换方法

1. 先备份现有仓库或记录当前 commit。
2. 解压后，将 bbixia.github.io 文件夹里面的内容放到仓库根目录，不要上传 ZIP，也不要套一层同名文件夹。
3. 这是完整替换包：先移除旧网站文件，再复制本包文件。保留仓库 .git 目录及你自己配置的 GitHub 工作流。仅覆盖同名文件不会删除旧作者的页面！
4. 提交后等待你原来的 GitHub Pages 构建完成。若使用分支发布，沿用当前分支和 /(root) 配置。
5. 打开五页确认；浏览器可用 Cmd+Shift+R 强制刷新。

## 日常修改

- 首页：index.md
- 论文：publications.md
- 设计项目及工作：experience.md
- 奖项：awards.md
- 中文：cn.md
- 姓名、联系方式、导航：_config.yml
- 左栏头像及社交链接：_includes/author-bio.html
- 页面结构：_layouts/page.html
- 字体、间距及头像尺寸：assets/css/main.css；首行 --avatar-size: 100px 控制方形头像边长。
- 头像文件：images/bixia.jpg

## 清理说明

删除旧作者博客、兴趣、混杂的 services 页面、旧中英文 CV、旧中文论文/奖项、旧头像/图标及介绍文档；移除旧统计账号、评论系统和所有第三方图标请求。仅 LICENSE 保留原始版权声明，并从网站构建输出排除。

采用一个统一页面布局，头像只在左侧栏显示，固定为 100 × 100 像素；手机屏幕上显示在正文上方。CSS 不依赖外部 CDN。保留本次提供的身份、履历及引用信息，仅修复明显拼写、语法和邮件链接问题，未独立核实论文信息。

原有作品集 PDF 和图片仍保留。超出本次确认五页范围的作品集页面源码及项目描述放在 _archive，暂不发布，以免误删你的材料。作品集外链仍在 Experience 页面。

## 本地构建（需要 Ruby 和 Bundler）

bundle install
bundle exec jekyll serve

GitHub Pages 可直接处理本项目的标准 Jekyll/Liquid/Kramdown 文件。发布前可运行 bundle exec jekyll build。
