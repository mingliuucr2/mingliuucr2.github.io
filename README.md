# Ming Liu — Academic Homepage

UC Riverside 教授个人主页。本地静态站点，纯 HTML/CSS，无框架或构建步骤；GitHub Pages 可直接使用。更新网页时，先在本地预览并审阅，再提交和发布。

## 文件

- `index.html`：首页，依次包含个人简介、四个研究方向、实验室探索项目、精选论文、教学、研究生学业指导、联系方式和博士生招生信息。
- `publications.html`：保留旧主页已核对的全部 16 篇论文（标题、作者、期刊、卷页、年份、DOI）。
- `assets/site.css`：两个页面共用的响应式样式。
- `assets/ming-liu.jpg`：本人提供的头像。
- `assets/nanofocusing-figure.png`、`assets/nv-nanodiamond-figure.jpg`、`assets/photocurrent-figure.jpg`：开放获取论文中的原图；来源和许可见下文。请保留页面图注。

## 本地预览

在仓库文件夹运行：

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

打开 <http://127.0.0.1:8000/>，检查首页和 <http://127.0.0.1:8000/publications.html>。结束时按 Control+C。本地预览不会更改公开网站。

## 后续维护

1. 用 Work 打开 `/Users/mingliu/Documents/GitHub/mingliuucr2.github.io`，让它先检查 Git 状态。
2. 在 `index.html` 修改相应 `<section id="…">` 的文字。研究成果和探索项目的状态要分开写；没有发表的测量结果不要当作已经验证的结果。
3. 新论文先核对 DOI、完整标题、作者身份、期刊、卷页和年份，再更新 `publications.html`。如属精选论文，也更新首页的 `#publications`。不要从 Google Scholar 的引用数或封面条目推断正式论文信息。
4. 课程以本人任课 syllabus 为准。主页的课程列表记录授课经历，不代表当学期课程安排。
5. 用本地预览检查电脑和手机布局、图片、导航和外部链接。只有审阅通过后，再用 GitHub Desktop 检查改动、提交并点击 **Push origin**；GitHub Pages 部署完成后再检查公开网址。
6. 修改 `assets/site.css` 后，同时将 `index.html` 和 `publications.html` 中的 `site.css?v=7` 版本号递增，以免浏览器继续显示缓存的旧样式。

主页按本人要求不显示 Research Group 或组员名单。不要将内部实验记录、学生信息、课程资料、未发表图像或电路细节放入仓库。

## 研究图片来源与使用

这些图片来自 Ming Liu 署名的正式论文，且本次只使用完整原图，没有裁掉科学标签。图注在主页逐一链接原文及许可。更换或编辑图片前，先核对各篇许可；尤其不要修改 Nano Letters 图片，因为它采用 ND（禁止改编）许可。

| 本地图片 | 原文 | 许可 |
| --- | --- | --- |
| `nanofocusing-figure.png` | [Ma et al., Nature Communications 12, 6868 (2021), Fig. 1](https://doi.org/10.1038/s41467-021-27216-5) | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| `nv-nanodiamond-figure.jpg` | [Liang et al., Nano Letters 24, 11661–11668 (2024), article figure](https://doi.org/10.1021/acs.nanolett.4c03163) | [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| `photocurrent-figure.jpg` | [Xu et al., Science Advances 11, eadv7614 (2025), Fig. 1](https://doi.org/10.1126/sciadv.adv7614) | [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) |

## 内容依据

- [UCR Faculty Profile](https://profiles.ucr.edu/app/home/profile/mingliu)：现职 Professor、UC Berkeley 应用物理博士（2010）、此前博士后经历、早期工作、邮箱和办公室。
- [Google Scholar](https://scholar.google.com/citations?user=1bPwuWgAAAAJ&hl=en)、[ORCID](https://orcid.org/0000-0001-9849-1845) 与出版商 DOI 页面：本页沿用此前核对的 16 篇论文；其中 Nano Letters 5 篇，ACS Applied Materials & Interfaces 4 篇。完整清单不是对整个职业生涯论文总数的断言。
- 本人提供的课程档案中，六门课程的 syllabus 均列 Ming Liu 为 instructor：EE 030B (Spring 2026)、EE 100A (Winter 2021)、EE 100B (Spring 2025)、EE 117 (Winter 2018)、EE 201 / MSE 207 (Fall 2024)、EE 204 (Spring 2022)。原始课程文件不在网站仓库。
- Graduate Advisor 的职责及咨询范围由本人提供；TA 申请和分配问题按本人文字指向 ECE Graduate Student Affairs Office。
- 高效纳米聚焦的效率和热点尺寸由本人及已发表研究说明；5 nm 指光学热点尺寸，不写成 nm³。2024 Nano Letters 已发表的是 NV 纳米金刚石捕获和荧光增强；ODMR 量子成像是正在开发的目标。非线性电化学谱学为探索方向，不声称已有正式结果。
