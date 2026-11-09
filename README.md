# Ming Liu — Academic Homepage

白底、传统学术风格的单页主页。纯 HTML/CSS，无框架、无 JavaScript、无构建步骤，兼容 GitHub Pages。

## 文件与本地预览

- `index.html`：全部网页内容与样式。`UPDATE:` 注释标出常用修改位置。
- `README.md`：维护说明与资料来源，不显示在主页中。

用浏览器打开 `index.html` 即可预览。也可以在仓库文件夹中运行：

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

然后访问 <http://127.0.0.1:8000>。预览后在终端按 Control+C 停止服务。本地预览不会更新公开网站。

## 以后通过 Work 更新

让 Work 打开此仓库：`/Users/mingliu/Documents/GitHub/mingliuucr2.github.io`。例如：

> 请更新本地学术主页，加入以下已确认的论文（提供作者、题目、期刊、年份、DOI）。保持现有风格，按年份倒序排列，检查电脑和手机预览。先不要提交或推送。

常用修改：

1. About：修改 `id="about"` 下的文字。
2. Research：修改 `id="research"` 下的方向与四个亮点。每条成果保留原文链接，不把计划写成已完成成果。
3. Publications：在 `ol.publications` 中复制一个完整的 `<li class="publication">…</li>`，替换作者、题目、期刊、卷、页码或文章编号、年份和 DOI，按年份倒序插入。编号自动生成。长作者列表使用首位作者加 `et al.`；不改变作者顺序。
4. Contact：确认邮箱、办公室与地址后修改。
5. 样式：文件顶部 `<style>` 内修改；颜色集中在 `:root`，手机样式在 `@media` 内。

主页按本人要求不展示 Research Group 区块或成员名单。

新增图片或 PDF 时可再建 `assets/` 文件夹，使用相对路径，例如 `assets/photo.jpg`；目前无需额外资源。不要在网页中写 Mac 绝对路径。

## 确认设计后，用 GitHub Desktop 发布

1. 选择 `mingliuucr2.github.io` 仓库，先查看是否有远端更新。存在更新时，让 Work 协助合并，保留本地内容。
2. 在 **Changes** 中逐一检查改动，确认只有预期文件；用浏览器预览并检查链接。
3. 只有在你确认后，填写说明并点击 **Commit to …**（以界面显示的当前分支为准）。
4. 点击 **Push origin**。GitHub Pages 按仓库现有发布设置更新；若有延迟，可在 GitHub 的 Actions / Pages 查看状态。
5. 检查 <https://mingliuucr2.github.io/>。只提交到本地、未推送时，公开网站不会更新。

发布需要本人明确授权。本次主页发布已获得授权；仓库的 Pages 设置保持原样。

## 内容依据与亮点选择

核对日期：2026-11-09。精选兼顾研究相关性、早期影响力与近期进展，并非完整论文清单或引用排名。没有展示会变化的引用次数，也没有添加未经确认的成员、招生活动或个人照片。

- 用户提供的 [Google Scholar](https://scholar.google.com/citations?user=1bPwuWgAAAAJ&hl=en)：确认身份、研究关键词，浏览引用排序与年份排序。排除专利、封面条目、重复记录，以及已有正式论文的预印本。
- [UCR Faculty Profile](https://profiles.ucr.edu/app/home/profile/mingliu)：院系、单位、邮箱和办公室。保留 faculty 的宽泛表述，不依赖旧新闻中的职称。
- 原版 `index.html`：Nanophotonics、Plasmonics、Nanoscale imaging、Quantum sensing。
- [Science Advances 2025](https://doi.org/10.1126/sciadv.adv7614)，[开放全文](https://pmc.ncbi.nlm.nih.gov/articles/PMC12309688/)，[UCR 研究介绍](https://ece.ucr.edu/highlights/2025/08/23/ucr-researchers-shed-light-photo-electricity-generation)：三维光电流成像，分离 PV/PTE 贡献；当前研究主线。
- [Nano Letters 2024](https://doi.org/10.1021/acs.nanolett.4c03163)，[开放全文](https://pmc.ncbi.nlm.nih.gov/articles/PMC11421074/)：NV 纳米金刚石的等离激元捕获与荧光增强；连接量子发光体方向。
- [Nature Communications 2021](https://doi.org/10.1038/s41467-021-27216-5)：碳纳米管上 6 nm 分辨率的透射与散射光谱成像。
- [Nature Photonics 2019](https://doi.org/10.1038/s41566-019-0456-9)：高效纳米聚焦与 1 nm 分辨率的无透镜 TERS。与 2021 工作共同构成成像亮点；不混同两种测量的分辨率。
- [Nano Letters 2017](https://doi.org/10.1021/acs.nanolett.7b03449)：毛细力辅助洁净转移；体现二维材料器件制备方法。
- [Nano Letters 2012](https://doi.org/10.1021/nl204202k) 与 [Nature 2011](https://doi.org/10.1038/nature10067)：双层与单层石墨烯光调制器；体现早期第一作者工作。
- [Nature Nanotechnology 2010](https://doi.org/10.1038/nnano.2010.128)：光驱动等离激元马达；体现纳米尺度光力操控。
- [Physical Review Letters 2008](https://doi.org/10.1103/PhysRevLett.101.047401)：等离激元诱导透明；保留高影响力合作工作，按原作者顺序引用。

未来更新时重新核对原文，尤其是联系方式和新论文的正式出版信息。
