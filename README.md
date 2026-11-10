# Ming Liu — Academic Homepage

白底、传统学术风格的单页主页。纯 HTML/CSS，无框架、无 JavaScript、无构建步骤，兼容 GitHub Pages。

## 文件与本地预览

- `index.html`：全部网页内容与样式。`UPDATE:` 注释标出常用修改位置。
- `README.md`：维护说明与资料来源，不显示在主页中。
- `assets/ming-liu.jpg`：本人提供的头像，保留原比例；从原始 AVIF 转为 JPEG 以兼容浏览器。

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
2. Research：修改 `id="research"` 下的方向与六个亮点。每条成果保留原文链接，不把计划写成已完成成果。
3. Publications：在 `ol.publications` 中复制一个完整的 `<li class="publication">…</li>`，替换作者、题目、期刊、卷、页码或文章编号、年份和 DOI，按年份倒序插入。编号自动生成。长作者列表使用首位作者加 `et al.`；不改变作者顺序。
4. Contact：确认邮箱、办公室与地址后修改。
5. 样式：文件顶部 `<style>` 内修改；颜色集中在 `:root`，手机样式在 `@media` 内。
6. Teaching：在 `id="teaching"` 下更新课程；以本人任课的 syllabus 确认代码与正式名称。这里记录授课经历，不代表所有课程都在当前学期开设。

主页按本人要求不展示 Research Group 区块或成员名单。

新增图片或 PDF 放入 `assets/` 文件夹并使用相对路径。替换头像时可沿用 `assets/ming-liu.jpg`，或同步修改页首图片的路径及尺寸。不要在网页中写 Mac 绝对路径。

## 确认设计后，用 GitHub Desktop 发布

1. 选择 `mingliuucr2.github.io` 仓库，先查看是否有远端更新。存在更新时，让 Work 协助合并，保留本地内容。
2. 在 **Changes** 中逐一检查改动，确认只有预期文件；用浏览器预览并检查链接。
3. 只有在你确认后，填写说明并点击 **Commit to …**（以界面显示的当前分支为准）。
4. 点击 **Push origin**。GitHub Pages 按仓库现有发布设置更新；若有延迟，可在 GitHub 的 Actions / Pages 查看状态。
5. 检查 <https://mingliuucr2.github.io/>。只提交到本地、未推送时，公开网站不会更新。

发布需要本人明确授权。2026-11-09 的初版已获授权并发布；本轮论文与研究方向更新也已获本人明确授权发布。仓库的 Pages 设置保持原样。

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

## 学术服务与主要研究贡献

- Graduate Advisor for Enrolled Students 的职责由本人在本轮明确提供，写入 About；没有从旧版研究生手册推断当前职责或任期。
- Research 开头按本人要求明确写出主要贡献为发明 high-external-efficiency nanofocusing，并附 [Nature Photonics 2019 原文](https://doi.org/10.1038/s41566-019-0456-9)。
- 论文摘要报告外部纳米聚焦效率约 50%；[合作者 Xuezhi Ma 的项目介绍](https://sites.google.com/view/xuezhi-ma/research/high-external-efficiency-nanofocusing-for-lens-free-near-field-optical-nano) 明确描述超过 50% 的光纤入射光聚焦到纳米线尖端。
- 本人进一步明确 5 nm 指光学热点尺寸，故网页写作 “an optical hotspot approximately 5 nm in size”。不将其误写成 5 nm³ 体积或探针尖端半径；5 nm 热点尺寸的直接依据为本人的澄清。


## Teaching 内容依据

用户提供的课程档案中，以下六份 syllabus 均明确列 Ming Liu 为 instructor；Teaching 仅据此提取课程名称和教学范围。没有把听课评估、他人课程示例或参考资料算作本人的授课经历。课程文件不随网页发布。

| 课程 | 正式名称 | 核对的 syllabus 学期 |
| --- | --- | --- |
| EE 030B | Fundamentals of Electric Circuits II | Spring 2026 |
| EE 100A | Electronic Circuits I | Winter 2021 |
| EE 100B | Electronic Circuits II | Spring 2025 |
| EE 117 | Electromagnetics II | Winter 2018 |
| EE 201 / MSE 207 | Applied Quantum Mechanics | Fall 2024 |
| EE 204 | Advanced Electromagnetics | Spring 2022 |

介绍强调从本科电路与电子设计到电磁学、研究生量子力学的教学广度，不声称未核实的教学奖项、学生评价或学习成效。


## 本轮核对记录（已获发布授权，2026-11-09）

- 已展开核对用户 Scholar 的全部 64 条记录，交叉检查 [ORCID 0000-0001-9849-1845](https://orcid.org/0000-0001-9849-1845) 的公开作品记录与出版商页面。Scholar/ORCID 可能缺漏，因此不声称这是完整职业生涯目录。
- Nano Letters：确认 5 篇，现已全部纳入本页：2012 双层石墨烯调制器、2016 银纳米线探针、2017 洁净转移、2019 远程激发 TERS、2024 NV 纳米金刚石。没有按期刊声望分组，统一按年份倒序。
- 期刊已由本人更正为 ACS Applied Materials & Interfaces（ACS AMI）。本页纳入已核对的全部 4 篇：2020 热输运、2022 热整流与热晶体管、2022 physics-guided inverse design、2023 ML-assisted optical microscopy。
- 新增 [Nano Letters 2016](https://doi.org/10.1021/acs.nanolett.6b02802) 和 [Nano Letters 2019](https://doi.org/10.1021/acs.nanolett.8b03399)，题目、年份、卷页与 DOI 以出版商记录为准。
- ML 新增正式论文：[Physics-Guided Neural-Network-Based Inverse Design of a Photonic–Plasmonic Nanodevice for Superfocusing](https://doi.org/10.1021/acsami.2c05083)，ACS Applied Materials & Interfaces 14, 27397–27404 (2022)；[Machine Learning Enhanced Optical Microscopy for the Rapid Morphology Characterization of Silver Nanoparticles](https://doi.org/10.1021/acsami.3c02448)，ACS Applied Materials & Interfaces 15, 18244–18251 (2023)；[Strategical Deep Learning for Photonic Bound States in the Continuum](https://doi.org/10.1002/lpor.202100658)，Laser & Photonics Reviews 16, 2100658 (2022)。不把该文的封面条目 DOI 10.1002/lpor.202270049 重复计为研究论文。
- Bayesian optimization、electrochemical interfaces 与 NV quantum sensing 的研究方向来自本人本轮说明。未找到可直接归属本人的 Bayesian optimization 或 electrochemical-interface 专题论文，所以网页将其表述为研究兴趣/方向，没有编造论文或声称已完成相应实验。NV 已发表工作的确证范围是捕获与荧光增强，没有声称已测得量子传感性能。
- Biography 沿用第一人称，并加入用户建议的 ML 表述；Research 以 nanofocusing 为主线，明确展示 physics-guided learning、inverse design、Bayesian optimization 和 ML-assisted nanoscale imaging。
- 本轮共 16 篇论文，其中 Nano Letters 5 篇、ACS Applied Materials & Interfaces 4 篇；题目、作者身份、期刊、卷页、年份与 DOI 已按个人记录、出版商页面和 DOI 注册数据交叉核对。
- 头像由本人于本轮提供，页首在姓名左侧显示；使用原图比例，不改变面部内容。
- 补入 [Thermal Rectifier and Thermal Transistor of 1T/2H MoS₂ for Heat Flow Management](https://doi.org/10.1021/acsami.1c21226)，ACS AMI 14, 4434–4442 (2022)，及 [Experimental Study on Thermal Conductivity and Rectification in Suspended Monolayer MoS₂](https://doi.org/10.1021/acsami.0c07544)，ACS AMI 12, 28306–28312 (2020)。两篇 DOI 注册记录中的 Ming Liu 均与本人 ORCID 一致。
