# Hao Mo — Academic Homepage

Target URL: https://minimo6666.github.io/

A simple, responsive academic homepage adapted from [Keunhong Park's website](https://keunhong.com/). The original serif typography, restrained colors, generous spacing, highlights, and publication layout are retained in a buildless HTML/CSS version.

## 本地预览

下载仓库后，双击 `index.html` 即可查看。无需 Node、Ruby、Jekyll 或编译。

也可以在项目目录运行 `python3 -m http.server 8000`，再打开 `http://localhost:8000`。这是可选的本地预览方式。

## 修改内容

| 内容 | 文件 |
| --- | --- |
| 个人介绍、论文、教育经历、联系邮箱 | `index.html` |
| 网页版 CV（可打印为 PDF） | `cv.html` |
| 字体、颜色、间距、移动端布局 | `assets/styles.css` |
| 头像 | `assets/images/avatar.png` |
| 论文配图 | `assets/images/` |
| 论文 BibTeX | `assets/bib/` |

目前头像为 GitHub 公开头像；可以用自己的方形照片替换 `avatar.png`，同时更新 `index.html` 中图片的 alt 描述。个人介绍、教育经历若变化，请同时更新首页和 CV。没有已确认的 Google Scholar 账号或 SCDM 代码链接，因此暂未放置这些入口。

在 `cv.html` 中点击 **Print / Save PDF**，在浏览器打印窗口中选择“另存为 PDF”；建议关闭浏览器的页眉页脚。此页面根据已知信息整理，不包含未经提供的工作经历或奖项。

添加新论文时，复制 `index.html` 中 `<article class="publication">` 的完整区块，更换标题、作者、会议、简介、图片和链接；如需添加上方精选卡片，复制 `<article class="highlight">` 区块。保留作者的实际顺序。

## GitHub Pages 部署

1. 在 `minimo6666` 账号下创建公开仓库，名称必须为 `minimo6666.github.io`。
2. 将本项目的所有文件放在仓库根目录（不要多套一层文件夹），推送至 `main` 分支。
3. 在仓库 **Settings → Pages → Build and deployment** 中选择 **Deploy from a branch**。
4. 选择 **main** 分支和 **/ (root)**，点击 **Save**。
5. 等待 Pages 部署成功，访问 https://minimo6666.github.io/ 。

无需服务器、固定 IP 或付费域名。`.nojekyll` 表示直接发布静态文件。网页文件已经包含在仓库中，不需要额外构建步骤。后续修改并提交到 `main` 会触发更新。

可选域名以后再绑定；不要保留其他模板作者的 `CNAME`。如果更改 GitHub 用户名或域名，请同步修改 HTML 的 canonical/og:url、`robots.txt`、`sitemap.xml` 和 CV 中的 Website 链接。

字体通过 Google Fonts 加载；不可用时会回退到系统衬线字体，文字和网站功能仍可使用。

## 信息来源

- [Bernoulli Flow Models — arXiv](https://arxiv.org/abs/2610.11362)
- [BFM code and NeurIPS 2026 poster information](https://github.com/minimo6666/BFM_NeurIPS2026)
- [SCDM — arXiv](https://arxiv.org/abs/2501.17876)
- Personal education information supplied by the site owner.
- The figures are original images from the corresponding papers. BibTeX files cite the verified arXiv versions; conference labels are shown separately on the pages.

## Attribution and license

Original design and template: [Keunhong Park](https://keunhong.com/), [keunhong/keunhong.github.io](https://github.com/keunhong/keunhong.github.io).

The original template is licensed under [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/). This adapted website design and template code are distributed under the same license. Changes include replacing personal content, adapting the layout to two papers, adding responsive and print styles, and converting the Jekyll/Tailwind template to standalone HTML/CSS.

Personal content, profile image, and paper figures are attributed to Hao Mo and the respective authors; the template license does not imply a new license grant over third-party research material.
