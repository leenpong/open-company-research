<div align="center">

# Open Company Research

**全球最完整的中文《上市公司研究》知识库**

_一套教你如何系统化研究一家公司的开源教材_

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](./LICENSE)
[![Docs: MkDocs Material](https://img.shields.io/badge/docs-MkDocs%20Material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
[![Markdown Lint](https://img.shields.io/badge/style-markdownlint-brightgreen.svg)](./.markdownlint.json)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![Made with ❤ in Chinese](https://img.shields.io/badge/language-中文-red.svg)](#)

[介绍](#-项目介绍) ·
[特点](#-特点) ·
[结构](#-项目结构) ·
[路线图](#-roadmap) ·
[学习路线](#-学习路线) ·
[贡献](#-贡献指南) ·
[FAQ](#-faq)

</div>

---

## 📖 项目介绍

**Open Company Research** 是一个开源、系统化、可持续维护的中文知识库，目标是回答一个问题：

> **如何专业地研究一家上市公司？**

本项目 **不是** 股票推荐，**不是** 财经新闻，**不是** 投资课程。
它是一套关于「公司研究方法论」的系统化教材——从财务报表、商业模式、行业格局，到竞争壁垒、管理层分析与估值框架，帮助读者建立独立、结构化的研究能力。

> ⚠️ **免责声明**：本知识库仅用于教育与研究目的，不构成任何投资建议。所有内容不代表任何买卖推荐，读者需为自己的决策负责。

## 🎯 目标

- 沉淀一套 **可复用、可迁移** 的公司研究方法论。
- 覆盖从 **入门基础** 到 **行业专题** 到 **实战案例** 的完整学习路径。
- 建立一个 **社区共建、长期维护** 的开放知识库。
- 提供 **标准化模板**，让任何人都能按同一套框架研究任意公司。

## ✨ 特点

- 📚 **系统化**：以方法论为主线，而非零散知识点。
- 🧩 **模板化**：公司、行业、财报、纪要均有标准模板。
- 🗺️ **结构化**：清晰的目录分层，便于检索与导航。
- 🎨 **可视化**：Mermaid 图表、思维导图、时间线全面支持。
- 🌐 **在线化**：基于 MkDocs Material 一键生成文档站点。
- 🤝 **开放化**：CC BY 4.0 协议，欢迎社区共建。

## 🗂️ 项目结构

```text
.
├── README.md                  项目说明
├── LICENSE                    开源协议（CC BY 4.0）
├── CHANGELOG.md               变更日志
├── CODE_OF_CONDUCT.md         行为准则
├── CONTRIBUTING.md            贡献指南
├── SECURITY.md                安全策略
├── ROADMAP.md                 路线图
├── STYLE_GUIDE.md             写作与格式规范
├── EDITORIAL_GUIDE.md         内容写作标准
├── PROJECT_RULES.md           工程 / 内容协作规则
├── mkdocs.yml                 MkDocs 站点配置
├── requirements.txt           文档构建依赖
│
├── docs/                      知识库正文
│   ├── index.md               站点首页
│   ├── 00-introduction/       项目导论
│   ├── 01-fundamentals/       研究基础方法论
│   ├── 02-ai-industry/        AI 行业专题
│   ├── 03-semiconductor/      半导体行业专题
│   ├── 04-cloud/              云计算行业专题
│   ├── 05-case-study/         实战案例研究
│   ├── 06-templates/          研究模板说明
│   ├── 07-learning/           学习资源（Books/Courses/Videos/Papers）
│   ├── 08-resources/          外部资源与工具
│   ├── 09-companies/          公司研究（按公司归档）
│   ├── 10-industry-maps/      产业链地图
│   ├── 11-notes/              研究笔记（按年份归档）
│   ├── glossary/              术语表
│   └── appendix/              附录
│
├── assets/                    静态资源
│   ├── images/                图片
│   ├── diagrams/              图表源文件
│   ├── logos/                 Logo
│   ├── mindmaps/              思维导图
│   └── timeline/              时间线
│
├── templates/                 可复制的研究模板
├── scripts/                   构建与维护脚本
├── examples/                  示例产出
├── resources/                 原始素材与参考资料
├── .claude/                   Claude Code 工程协作说明
└── .github/                   Issue / PR 模板与 CI 工作流
```

## 🛣️ Roadmap

项目按语义化版本分阶段推进，完整规划见 [ROADMAP.md](./ROADMAP.md)。

- **v0.1** — 项目初始化：目录、规范、工具链、CI。
- **v0.5** — 基础方法论成型：`01-fundamentals` 全部完成。
- **v1.0** — 首个完整行业专题 + 首个完整案例。
- **v2.0** — 多行业覆盖 + 可视化体系。
- **v3.0** — 社区规模化共建，成为中文公司研究事实标准。

## 🧭 学习路线

> 🚧 学习路线规划中，待正文内容完善后补全。

<!-- TODO: 补充「新手入门 → 进阶 → 专题 → 实战」的推荐阅读顺序 -->

## 🤝 贡献指南

我们欢迎任何形式的贡献——修正错别字、补充案例、绘制图表、完善方法论。

请先阅读：

- [CONTRIBUTING.md](./CONTRIBUTING.md) — 如何提交贡献
- [STYLE_GUIDE.md](./STYLE_GUIDE.md) — 写作与格式规范
- [EDITORIAL_GUIDE.md](./EDITORIAL_GUIDE.md) — 内容写作标准
- [PROJECT_RULES.md](./PROJECT_RULES.md) — 工程 / 内容协作规则
- [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) — 社区行为准则

## 📄 License

本项目内容采用 [**Creative Commons Attribution 4.0 International (CC BY 4.0)**](./LICENSE) 协议授权。
你可以自由地分享与演绎，但需注明出处。

## 🙏 鸣谢

感谢所有为本项目贡献内容、提出建议、参与讨论的社区成员。
同时感谢以下开源项目提供的灵感与工具：

- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [Microsoft Docs](https://learn.microsoft.com/)
- [OpenAI Cookbook](https://github.com/openai/openai-cookbook)
- Awesome 系列开源清单

## ❓ FAQ

<details>
<summary><strong>这是投资建议吗？</strong></summary>

不是。本项目仅提供研究方法论与教育内容，不构成任何投资建议，也不推荐任何证券。
</details>

<details>
<summary><strong>需要金融背景才能阅读吗？</strong></summary>

不需要。`01-fundamentals` 从零开始讲解研究方法，非科班读者同样适用。
</details>

<details>
<summary><strong>如何在本地预览文档站点？</strong></summary>

```bash
pip install -r requirements.txt
mkdocs serve
# 浏览器打开 http://127.0.0.1:8000
```
</details>

<details>
<summary><strong>我可以贡献自己的公司研究吗？</strong></summary>

当然可以。请使用 `templates/` 下的标准模板，并阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。
</details>

---

<div align="center">

如果这个项目对你有帮助，欢迎点一个 ⭐ Star 支持我们持续维护。

</div>
