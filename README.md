# DM0025 · Vocational Exam Question Samples / 职业考题样例

**Dataset card / 数据集卡片** · Zovda sample dataset. This repository is the GitHub mirror of the card; the data files are hosted on Hugging Face — **[download the dataset / 下载数据集](https://huggingface.co/datasets/Zovda/dm0025-vocational-exam-question-samples)**.

本仓库是数据集卡片的 GitHub 镜像，数据文件托管在 Hugging Face，**[点击下载 / download](https://huggingface.co/datasets/Zovda/dm0025-vocational-exam-question-samples)**。

| Item / 项目 | Value / 值 |
|---|---|
| Dataset ID / 数据集编号 | DM0025 |
| Files / 数据文件 | 16 |
| Size / 数据体积 | 44.11 KB |
| Language / 语言 | zh |
| Tasks / 任务类别 | question-answering, text-classification |
| Hugging Face / 数据地址 | [dm0025-vocational-exam-question-samples](https://huggingface.co/datasets/Zovda/dm0025-vocational-exam-question-samples) |
| Provided by / 提供方 | Zovda |
| Contact / 联系邮箱 | lucas@zovda.com |

## Overview / 简介

80 questions across 16 vocational certification and skills categories, 5 per category; each item carries a prompt with structured A/B/C/D options and a second-level exam or trade tag.

16 个职业资格与技能门类，每门 5 题共 80 题；每题含题干与 A/B/C/D 结构化选项，并标注到二级门类（具体考试 / 工种）。

## What's inside / 数据内容

- 16 JSONL files, one directory per category: transport, sports & health, IT, general knowledge, civil service, military & firefighting, agriculture & veterinary, medicine, dentistry, engineering skills, construction, education & psychology, law, design & media, accounting and finance.
- 16 个 JSONL 文件，按门类分目录：交通运输、体育健康、信息技术、公共常识、公务事业、军事消防、农林兽医、医药卫生、口腔医学、工科技能、建筑工程、教育心理、法律法学、设计传媒、财务会计、金融从业。
- Fields: top-level category, second-level category, question type, prompt, options, confidence, decision basis.
- 字段：一级门类、二级门类、题型、题干、选项、置信度、判定依据。

## Specifications / 规格

- Format: UTF-8 JSONL, one record per line
- 格式：UTF-8 JSONL，逐行一条记录
- Scale: 16 files / 80 questions / 44.11 KB
- 规模：16 文件 / 80 题 / 44.11 KB
- Options are structured A/B/C/D arrays; this batch has no answer or explanation fields (available on request)
- 选项为 A/B/C/D 结构化数组；本批不含答案与解析字段（可按需配售）

## Suitable tasks / 适用任务

- Vocational exam question-bank construction
- 职业资格考试题库构建
- Classification and retrieval by certificate family or trade
- 按证书族/工种的题目分类与检索
- Exam QA and question-generation evaluation
- 考试类问答与题目生成评测

## Files / 文件清单

Paths below are relative to the Hugging Face repository root. 下表路径相对于 Hugging Face 仓库根目录。

| # | File | Size |
|---|---|---|
| 1 | `dm0025/交通运输/样例.jsonl` | 2.21 KB |
| 2 | `dm0025/体育健康/样例.jsonl` | 2.53 KB |
| 3 | `dm0025/信息技术/样例.jsonl` | 2.04 KB |
| 4 | `dm0025/公共常识/样例.jsonl` | 3.01 KB |
| 5 | `dm0025/公务事业/样例.jsonl` | 2.51 KB |
| 6 | `dm0025/军事消防/样例.jsonl` | 3.89 KB |
| 7 | `dm0025/农林兽医/样例.jsonl` | 2.81 KB |
| 8 | `dm0025/医药卫生/样例.jsonl` | 2.74 KB |
| 9 | `dm0025/口腔医学/样例.jsonl` | 2.42 KB |
| 10 | `dm0025/工科技能/样例.jsonl` | 2.10 KB |
| 11 | `dm0025/建筑工程/样例.jsonl` | 2.33 KB |
| 12 | `dm0025/教育心理/样例.jsonl` | 2.55 KB |
| 13 | `dm0025/法律法学/样例.jsonl` | 2.84 KB |
| 14 | `dm0025/设计传媒/样例.jsonl` | 3.31 KB |
| 15 | `dm0025/财务会计/样例.jsonl` | 3.63 KB |
| 16 | `dm0025/金融从业/样例.jsonl` | 3.21 KB |

## Download / 下载

The files are not stored in this repository. 数据文件不在本仓库内，请从 Hugging Face 获取。

- Dataset page / 数据集页面: https://huggingface.co/datasets/Zovda/dm0025-vocational-exam-question-samples
- Direct file URL / 单文件直链: `https://huggingface.co/datasets/Zovda/dm0025-vocational-exam-question-samples/resolve/main/<path from MANIFEST.csv>`

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="Zovda/dm0025-vocational-exam-question-samples",
    repo_type="dataset",
    local_dir="./dm0025-vocational-exam-question-samples",
)
```

```python
from huggingface_hub import hf_hub_download

hf_hub_download(
    repo_id="Zovda/dm0025-vocational-exam-question-samples",
    repo_type="dataset",
    filename="<path from MANIFEST.csv>",
    local_dir="./dm0025-vocational-exam-question-samples",
)
```

## Rights and disclaimer / 授权与声明

Items are tagged to a second-level exam or trade. Samples demonstrate schema and data conventions; contact us for licensing at scale.

题目来源标注到二级门类。样例用于展示字段结构与数据规范；规模化商用授权请联系我们。

This dataset is shared to demonstrate data organisation, technical specifications and delivery structure. For formal licensing, large-scale access or custom production, contact lucas@zovda.com.

本数据集仅用于展示数据组织方式、技术规格与交付结构。正式授权、规模化取数与定制生产请联系 lucas@zovda.com。

## About Zovda / 关于 Zovda

Zovda builds, cleans, annotates and packages training data across video, audio, images, e-commerce image-text pairs, exam question banks, embodied AI and coding-agent corpora.

Zovda 提供多模态与文本训练语料的数据采集、清洗、标注与结构化交付服务，覆盖视频、音频、图像、电商图文、K12 与职业题库、具身智能、代码智能体等方向。

**Contact / 联系方式:** lucas@zovda.com
