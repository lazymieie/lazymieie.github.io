# 郭嘉欣的学术主页

基于 [Academic Pages](https://github.com/academicpages/academicpages.github.io)，保留原生 Jekyll 结构和主题，内容依据用户提供的简历整理。

## 页面

- 首页：`_pages/about.md`，个人介绍、研究方向、动态、精选论文、实习与奖励。
- 论文：`_pages/publications.html`，正式会议论文和在审稿件分栏。
- 论文详情：`_publications/deppo.md`、`_publications/egas.md`。
- 项目：`_pages/projects.md`。
- 简历：`_pages/cv.md`，适合公开的网页简历。
- 基本信息：`_config.yml`；菜单：`_data/navigation.yml`。
- 头像：`images/cartoon-cat.svg`，来自 Twemoji，按 CC BY 4.0 署名；不使用真人照片。
- 个性样式：`_sass/_custom.scss`，在 Academic Pages 样式之后加载。

未加入原始简历 PDF、手机号、年龄、民族和政治面貌。DEPPO 全文已收录于 `files/DEPPO.pdf`，首页、论文列表和 CV 中可直接打开，详情页提供下载。未提供的 GitHub、Google Scholar、其他论文全文、代码链接和完整作者列表保持空缺。不会生成指向其他学者的示例链接。

正式网址：[https://lazymieie.github.io/](https://lazymieie.github.io/)

目标仓库：[lazymieie/lazymieie.github.io](https://github.com/lazymieie/lazymieie.github.io)

## 发布到 GitHub Pages

1. 在自己的 GitHub 账号下创建名为 `USERNAME.github.io` 的仓库，将 `USERNAME` 替换为真实账号名。
2. 修改 `_config.yml` 中的 `url` 为 `https://USERNAME.github.io`，`repository` 为 `USERNAME/USERNAME.github.io`，`author.github` 为真实用户名。
3. 将本项目的内容（包括 `.github`）放入自己的仓库，推送到 `main` 或 `master`。不要推送到 Academic Pages 官方仓库。
4. 在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。
5. 在 **Actions** 中运行 `Build and deploy academic homepage`，等待成功；正式网址为 `https://USERNAME.github.io/`。

工作流使用 Ruby 3.3、Jekyll 4.4，构建时使用 `_config.yml` 中的正式域名，并读取 GitHub Pages 的子路径。也支持普通项目仓库路径。

官方说明：[创建 GitHub Pages 网站](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)。

## 本地预览

需要 Ruby 3.3 或更新版本、Bundler 和 Node.js：

```sh
bundle config set --local path vendor/bundle
bundle install
npm install
npm run build:js
bundle exec jekyll serve --config _config.yml,_config_local.yml --host 127.0.0.1 --port 4000
```

浏览器打开 `http://127.0.0.1:4000/`。修改 `_config.yml` 后重启 Jekyll。正式发布由 GitHub Actions 完成，无需上传 `_site` 或 `vendor`。

## 新增论文

在 `_publications/` 新建 Markdown 文件：

```yaml
---
title: "Paper title"
collection: publications
category: conferences  # 或 manuscripts
permalink: /publication/paper-slug/
year: 2026
sort_order: 3          # 大的数字排在前面
venue: "Conference / Manuscript · Under Review"
author_role: "First author"
selected: true        # 是否显示在首页
summary: "A short description of the contribution."
paperurl: "https://..." # 没有真实链接时删除此行
codeurl: "https://..."  # 没有真实链接时删除此行
share: false
comments: false
---
```

正文填写工作介绍。不要把项目起止时间当成论文发表日期；当前条目只显示已提供的年份。

## 模板示例与许可

模板自带的示例论文、课程、博客与辅助工作流已归档至本地 `local/template-samples/`，该目录同时被 Git 与 Jekyll 排除。原始模板说明保留在 `README.md`。保留 MIT 许可及 Academic Pages / Minimal Mistakes 署名。
