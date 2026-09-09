# 藏语语音合成资源合集

综述论文配套仓库：

> **Recent Advances in Tibetan Speech Synthesis: A Survey（藏语语音合成最新进展综述）**
> 王超、蔡雨晴、多杰仁增、朱玉磊、刘雨桐、肖金颖、姬拉毛、张朋勃、尼玛扎西
> 投稿期刊：IEEE Transactions on Audio, Speech, and Language Processing (TASLP)

本仓库提供综述中资源清单、研究特征与证据分层编码的机器可读版本，并在有公开标识符的
藏语语音资源处附上链接。

## 范围与证据窗口

综述的叙述性证据窗口**冻结于 2026 年 8 月 27 日**，以保证论文中每一条主张都对应固定、
可追溯的记录集。本仓库在该窗口之外持续更新：新的藏语 TTS 资源、基准与复现工作会陆续
加入，并带 `added_after_freeze` 日期字段，保证冻结后的记录与支撑论文表格的记录始终
可区分。

## 内容

| 文件 | 对应论文表格 | 说明 |
|---|---|---|
| `data/resources.csv` | 表 II 与表 VIII | 全部 12 项藏语语音资源（R01–R12）：方言、说话人数、规模、标注、访问状态、FAIR 筛查、来源标识 |
| `data/studies.csv` | 表 V | 藏语 TTS 研究（2011–2025）：技术路线、前端报告、评估方式、核验状态 |
| `data/evidence_tiers.csv` | 表 VII | 按技术路线的描述性证据分层编码 |

## 字段说明（`data/resources.csv`）

- `resource_id` — R01–R12，与论文中的编号完全一致
- `resource_name` — 来源论文报告的资源名称
- `dialect` — 方言/语言覆盖（卫藏、安多、康巴等）
- `speakers`、`size`、`sampling_rate` — 按来源报告；`NR` = 来源未报告
- `annotation` — 报告的标注类型
- `access_status`、`license` — 来源报告的访问与许可条款
- `paper_title`、`authors`、`venue`、`year`、`doi` — 文献标识
- `fair_f/fair_a/fair_i/fair_r` — 来源报告的 FAIR 就绪度筛查
- `tts_relevant` — 该资源是面向 TTS 还是识别相关
- `added_after_freeze` — 论文冻结窗口内的记录此字段为空

## 访问说明

许多藏语语音资源见于文献但未公开发布。`NR`（未报告）值直接来自来源论文，本综述不
推断缺失的元数据。如果你维护其中某项资源并能提供公开定位符、许可证或更正后的元数
据，欢迎提交 issue 或 pull request。

## 引用

使用本合集请引用综述论文（论文发表后补充 BibTeX）及本仓库（见英文版 README 中的
BibTeX 条目，Zenodo DOI 待发布时分配）。

## 许可证

本仓库数据文件拟以 CC BY 4.0 许可发布（正式发布前确认）。
