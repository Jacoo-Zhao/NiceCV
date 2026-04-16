<p align="center">
  <h1 align="center">CV Templates for PhD Candidates</h1>
  <p align="center">
    Production-ready LaTeX CV templates for PhD candidates, postdocs, and early-career researchers.
    <br />
    面向博士生、博士后及青年学者的学术简历 LaTeX 模板。
  </p>
  <p align="center">
    <a href="#english">English</a> · <a href="#中文说明">中文说明</a>
    <br /><br />
    <a href="mailto:zhaozyzyq@gmail.com">zhaozyzyq@gmail.com</a>
  </p>
</p>

---

<a name="english"></a>

## Overview

This repository provides **two professionally typeset LaTeX CV templates** — one in English and one in Chinese — specifically structured for academic career milestones: publications, research experience, teaching, grants, and service.

Both templates share a unified visual language: accent-blue section headings, `tabularx`-aligned entries with right-flushed dates, and compact spacing that maximizes content density without sacrificing readability.

### Templates at a Glance

| Template | Language | Engine | Preview |
|:---------|:---------|:-------|:--------|
| [`eng.tex`](eng.tex) | English | `pdflatex` | [eng.pdf](eng.pdf) |
| [`cn.tex`](cn.tex) | 中文 | `xelatex` | [cn.pdf](cn.pdf) |

## Features

- **Modular section structure** — Research Interests, Education, Publications, Research Experience, Industry Experience, Teaching & Service, Honors & Awards, and Skills. Comment out or reorder any `\section` block.
- **Publication list** — Numbered entries with bold author highlighting, venue formatting, and inline links to arXiv, code, demos, and slides.
- **Three reusable commands** — `\entry{}{}{}`, `\entrysub{}{}{}{}`, and `\honorrow{}{}{}` enforce consistent alignment across all entries.
- **Customizable color scheme** — Modify `accentblue`, `darkgray`, `lightgray`, and `rulecolor` in the preamble.
- **CJK-ready** — The Chinese template uses `ctex` + `xeCJK` with Noto Serif CJK SC, fully compatible with `xelatex`.

## Quick Start

**1. Get the source**

```bash
git clone https://github.com/<your-username>/CV_Templates_for_PhD_Candidates.git
cd CV_Templates_for_PhD_Candidates
```

**2. Edit** — Open `eng.tex` or `cn.tex` and replace the placeholder content with your information.

**3. Compile**

```bash
pdflatex eng.tex          # English template
xelatex  cn.tex           # Chinese template
```

> **Overleaf users:** Upload the `.tex` file directly. For the Chinese template, set the compiler to `XeLaTeX` in the Overleaf project settings.

## Requirements

| Dependency | Scope | Notes |
|:-----------|:------|:------|
| TeX Live Full / MiKTeX | Both templates | Includes all required packages |
| `fontawesome5` | Both templates | Icons for contact info |
| `ctex`, `xeCJK` | Chinese only | CJK typesetting support |
| Noto Serif CJK SC | Chinese only | Default CJK font; replaceable in `\setCJKmainfont{}` |

Core packages used: `geometry`, `hyperref`, `fontawesome5`, `titlesec`, `enumitem`, `tabularx`, `xcolor`, `microtype`, `lmodern`, `ifthen`, `amssymb`.

## Customization

| What | How |
|:-----|:----|
| **Colors** | Edit `\definecolor{accentblue}`, `{darkgray}`, `{lightgray}`, `{rulecolor}` |
| **Margins** | Adjust `\usepackage[margin=..., top=..., bottom=...]{geometry}` |
| **Font size** | Change `10pt` in `\documentclass[10pt, letterpaper]{article}` to `11pt` or `12pt` |
| **Sections** | Each section is fenced by `%===` comment blocks — delete, duplicate, or reorder freely |
| **CJK font** | Replace `Noto Serif CJK SC` in `\setCJKmainfont{}` with any installed CJK font |

## Project Structure

```
CV_Templates_for_PhD_Candidates/
├── eng.tex        # English CV template source
├── eng.pdf        # Compiled English preview
├── cn.tex         # Chinese CV template source
├── cn.pdf         # Compiled Chinese preview
└── README.md
```

## Contributing

Contributions of new language variants, field-specific layouts, and improvements are welcome.

1. Fork the repository.
2. Create a feature branch: `git checkout -b feat/your-template`.
3. Add or modify templates, and include a compiled PDF preview.
4. Open a pull request describing your changes.

Please ensure all `.tex` files compile without errors before submitting.

## License

This project is licensed under the [MIT License](LICENSE).

---

<a name="中文说明"></a>

## 中文说明

### 概述

本仓库提供 **两套专业排版的 LaTeX 学术简历模板** ——英文版与中文版——专为博士生、博士后及青年学者设计，涵盖学术求职、奖学金申请及科研岗位所需的核心板块。

两套模板采用统一的视觉风格：蓝色主题色标题、基于 `tabularx` 的对齐排版（日期右对齐）、紧凑行距以最大化内容密度，同时保持良好的可读性。

### 模板概览

| 模板文件 | 语言 | 编译引擎 | 预览 |
|:---------|:-----|:---------|:-----|
| [`eng.tex`](eng.tex) | English | `pdflatex` | [eng.pdf](eng.pdf) |
| [`cn.tex`](cn.tex) | 中文 | `xelatex` | [cn.pdf](cn.pdf) |

### 功能特性

- **模块化章节结构** — 研究兴趣、教育经历、发表论文、研究经历、业界经历、荣誉奖项、其他信息。可自由注释、删除或调整章节顺序。
- **论文列表** — 编号排列，支持作者加粗、会议/期刊名称格式化，以及 arXiv、代码、演示的内联链接。
- **三个复用命令** — `\entry{}{}{}`、`\entrysub{}{}{}{}`、`\honorrow{}{}{}` 确保所有条目对齐一致。
- **可自定义配色** — 在导言区修改 `accentblue`、`darkgray`、`lightgray`、`rulecolor` 即可全局切换主题色。
- **中文排版支持** — 使用 `ctex` + `xeCJK`，默认字体为 Noto Serif CJK SC，通过 `xelatex` 编译。

### 快速开始

**1. 获取源码**

```bash
git clone https://github.com/<your-username>/CV_Templates_for_PhD_Candidates.git
cd CV_Templates_for_PhD_Candidates
```

**2. 编辑** — 打开 `eng.tex` 或 `cn.tex`，将占位内容替换为您的个人信息。

**3. 编译**

```bash
pdflatex eng.tex          # 英文模板
xelatex  cn.tex           # 中文模板
```

> **Overleaf 用户：** 直接上传 `.tex` 文件即可。中文模板请在项目设置中将编译器切换为 `XeLaTeX`。

### 环境要求

| 依赖项 | 适用范围 | 说明 |
|:-------|:---------|:-----|
| TeX Live Full / MiKTeX | 所有模板 | 包含全部所需宏包 |
| `fontawesome5` | 所有模板 | 联系方式图标 |
| `ctex`、`xeCJK` | 仅中文模板 | CJK 排版支持 |
| Noto Serif CJK SC | 仅中文模板 | 默认中文字体，可在 `\setCJKmainfont{}` 中替换 |

### 自定义指南

| 修改项 | 方法 |
|:------|:-----|
| **配色方案** | 编辑 `\definecolor{accentblue}`、`{darkgray}`、`{lightgray}`、`{rulecolor}` |
| **页边距** | 调整 `\usepackage[margin=..., top=..., bottom=...]{geometry}` |
| **字号** | 将 `\documentclass[10pt, ...]` 中的 `10pt` 改为 `11pt` 或 `12pt` |
| **章节增删** | 每个章节由 `%===` 注释行分隔，可自由删除、复制或重排 |
| **中文字体** | 将 `\setCJKmainfont{}` 中的 `Noto Serif CJK SC` 替换为任意已安装的 CJK 字体 |

### 参与贡献

欢迎提交新语种模板、学科专用布局或其他改进。

1. Fork 本仓库。
2. 创建特性分支：`git checkout -b feat/your-template`。
3. 添加或修改模板，并附上编译后的 PDF 预览。
4. 发起 Pull Request 并简要描述您的更改。

提交前请确保所有 `.tex` 文件可无错误编译。

### 许可证

本项目基于 [MIT 许可证](LICENSE) 开源。

---

<p align="center">
  如果这些模板对您有所帮助，请为本仓库点亮 Star 以帮助更多学术同仁发现它。
  <br />
  If you find these templates useful, consider giving this repo a star.
</p>
