 GitHub 教育资源清单

> 整理自公众号文章《一些对小学生价值非常高的网络学习资源》（月半宵夜趣）
> 整理日期：2026-09-12 ｜ 已逐一核验仓库是否存在、内容是否有效（星级、大小、文件结构）

## 一、北师大版小学数学（重点）

| 仓库 | 说明 | 状态 |
|---|---|---|
| [jackli01030/shiyi-math-practice](https://github.com/jackli01030/shiyi-math-practice) | **北师大版一年级上册数学（2024版）练习网站**。支持口算/智力题/比多少等分类练习，儿童友好，练习记录存本地，可打印。已部署在线版：https://jackli01030.github.io/shiyi-math-practice/ | ✅ 已核实 |
| [pengboyjak/textbook-library](https://github.com/pengboyjak/textbook-library) | 中国 K12 中小学教材库，收录 2637 本教材/目录元数据（catalog.json / csv），含北师大版数学书目索引，附 SKILL.md 可被 AI 直接使用 | ✅ 已核实 |
| [mtcsol/awesome-k12-books](https://github.com/mtcsol/awesome-k12-books) | K12 教材/练习册/专项学习资料精选合集（README 巨型清单），按年级与学科整理 | ✅ 已核实 |
| [kska32/ebooks](https://github.com/kska32/ebooks) | 收藏的电子书合集（数学类教材内部公开文档，约数万本，含北师大/人教版等）｜注意仓库可能体积大 | ✅ 已核实 |
| [wizarot/math-tree](https://github.com/wizarot/math-tree) | 数学学习知识图谱，对标国内课标内容，可作知识点树状梳理参考 | ✅ 已核实 |
| [1wri/textbook](https://github.com/1wri/textbook) | 小学/初中/高中各科教材电子版（README 内提供网盘等下载入口） | ⚠️ 仅索引 |
| [34426/Books](https://github.com/34426/Books) | 同上，教材电子版索引 | ⚠️ 仅索引 |

### 北师大数学使用建议
- 一年级的家长直接用 [shiyi-math-practice](https://jackli01030.github.io/shiyi-math-practice/) 在线给娃练口算，无需本地部署。
- 需要按单元/课时备课、出题时，结合本地技能：`xinkebiao-math-alignment`（2022课标）、`teaching-plan-writer`（教案）、`k12-smart-teacher`（练习/试卷）。

## 二、OD（Oxford Discover）英语学习

| 仓库 | 说明 | 状态 |
|---|---|---|
| [AlikiXu/Oxford-Discover-Vocab-Master](https://github.com/AlikiXu/Oxford-Discover-Vocab-Master) | OD 词汇闪卡（每词配图 + MP3 音频），OD1 动物/自然主题，可直接给孩子用 | ✅ 已核实 |
| [celianong/oxford_discover_vocab_builder](https://github.com/celianong/oxford_discover_vocab_builder) | OD 词表生成工具（Python）：一条命令产出 Anki 卡 / Notion 卡 / 填空题工作表 / Word文档 | ✅ 已核实 |
| [rasulovabubakir11-ai/oxford](https://github.com/rasulovabubakir11-ai/oxford) | Oxford 学习 Web App（React/TS）：AI 翻译、听力实验室、语法挑战、单词查找游戏等 | ✅ 已核实 |
| [thanhnbt/OxfordDiscovery](https://github.com/thanhnbt/OxfordDiscovery) | OD3 4GE Assessment Revision 评估复习网页（kindle 适配），可当闯关复习用 | ✅ 已核实 |
| [Vanessa01210/oxford_discover1](https://github.com/Vanessa01210/oxford_discover1) | OD1 单页练习（index.html）+ logo，适合低年级过知识点 | ✅ 已核实 |
| [mikikimi/oxford-read-n-discover-audio](https://github.com/mikikimi/oxford-read-n-discover-audio) | Oxford Read and Discover 全套 L1-L6 音频（936 条 mp3，约 1.6GB）｜**体积大，建议 git clone 或按 Level 单独下载** | ✅ 已核实 |
| [mikikimi/oxford-read-n-discover](https://github.com/mikikimi/oxford-read-n-discover) | 同系列的 PDF/阅读资源（约 2.8GB） | ✅ 已核实 |

> OD 与「读与发现」是两套：OD 主教材大文件（PDF/音视频）多在网盘站（多课吧 doc8 / 学霸智库），GitHub 上主要能抓到**词表、闪卡、工具和网页应用**。OD 全能工具即 [thinking-scaffolds 技能]（本地已有）。

## 三、英语词库（通用）

| 仓库 | 说明 | 状态 |
|---|---|---|
| [lilinji/English](https://github.com/lilinji/English) | 「全网最全英语单词词库」，含全国各教材版本同步词书 328 本（人教/外研/苏教/**北师大版英语**等），xlsx 可直接导入 Anki/欧路/百词斩 | ✅ 已核实 |
| [viper-00/oxford-dictionarys](https://github.com/viper-00/oxford-dictionarys) | Oxford 3000 / 5000 / Phrase List 中英对照词表 | ✅ 已核实 |
| [betterlearn/english-wordlists](https://github.com/betterlearn/english-wordlists) | 四六级/托福/GRE等常见词表（含牛津高阶 OALD8 对照） | ✅ 已核实 |

## 四、抓取/使用方式备忘

- 小仓库（词表/闪卡/工具）直接 `git clone`，无需登录。
- OD 大仓库（`mikikimi/oxford-read-n-discover*`）用：
  ```bash
  git clone --depth 1 https://github.com/mikikimi/oxford-read-n-discover-audio.git
  ```
  若要省流量，可先 `gh api repos/mikikimi/oxford-read-n-discover-audio/git/trees/<branch>?recursive=1` 列出文件清单，再按需下载单个 Level。
- 教材电子版索引类仓库（1wri/textbook 等）README 里的网盘链接需自行鉴别有效期。