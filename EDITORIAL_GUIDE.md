# Editorial Guide

本指南定义 **Open Company Research** 的内容写作标准。它 **不是** 教材本身，
而是所有章节作者（人工或 ChatGPT）在撰写内容时必须遵循的编辑规范。

> 工程与内容分离：本文件只定义「怎么写」，不定义「写什么」。
> 工程侧规范见 [STYLE_GUIDE.md](./STYLE_GUIDE.md) 与 [PROJECT_RULES.md](./PROJECT_RULES.md)。

## 目录

- [Book Writing Standards](#book-writing-standards)
- [Chapter Structure](#chapter-structure)
- [Heading Style](#heading-style)
- [Markdown Rules](#markdown-rules)
- [Mermaid Rules](#mermaid-rules)
- [Reference Style](#reference-style)
- [Internal Linking](#internal-linking)
- [Cross References](#cross-references)
- [Glossary Rules](#glossary-rules)
- [Image Naming](#image-naming)
- [Citation Rules](#citation-rules)
- [Writing Consistency](#writing-consistency)

## Book Writing Standards

- 目标读者：具备基础但希望系统学习公司研究方法的读者。
- 立场：客观、中立、可验证。**禁止任何投资建议、荐股或买卖判断。**
- 事实优先：每一个结论都必须能追溯到公开、可核实的来源。
- 方法导向：讲「如何研究」，而非「结论是什么」。
- 单一职责：一个文件只讲清楚一个主题，避免章节膨胀。
- 语言：简体中文为主，专有名词保留英文原文（NVIDIA、EBITDA、SaaS）。

## Chapter Structure

每个章节建议遵循统一骨架（具体小节可按需增减）：

1. **概述 / Overview** — 本章要回答的问题。
2. **核心概念 / Key Concepts** — 必要的定义与框架。
3. **方法与步骤 / Method** — 可操作的研究流程。
4. **示例 / Example** — 演示方法（非投资建议）。
5. **常见误区 / Pitfalls** — 易错点与纠偏。
6. **小结 / Summary** — 要点回顾。
7. **延伸阅读 / Further Reading** — 指向 `07-learning` 与外部来源。

## Heading Style

- 使用 ATX 风格（`#`），层级不得跳级。
- 每个文件有且仅有一个一级标题 `#`，作为页面标题与导航名。
- 标题为名词短语，简洁、不以标点结尾。
- 同一文件内同级标题不得重复。
- 标题层级最深到 `####`，超过说明结构需拆分。

## Markdown Rules

- 遵循 [`.markdownlint.json`](./.markdownlint.json)。
- 无序列表用 `-`，有序列表用 `1.`。
- 代码块使用围栏并标注语言。
- 强调用 `*斜体*` 与 `**加粗**`。
- 中英文之间、中文与数字之间留一个空格。
- 表格用于结构化对比，避免用表格堆砌长文本。
- 文件末尾保留一个空行。

## Mermaid Rules

- 使用 ` ```mermaid ` 围栏。
- 一图一主题，节点文字精炼；复杂逻辑拆成多张小图。
- 方向优先 `TD` 或 `LR`。
- 图表须服务于正文，正文需对关键图表作文字说明。
- 可编辑源文件放入 `assets/diagrams/`。

## Reference Style

- 外部观点用引用块 `>` 呈现并标注出处。
- 数据必须标注来源与时间（如「来源：公司 2025 财年 10-K」）。
- 链接锚文本要有意义，禁止「点击这里」。
- 优先引用一手来源（招股书、年报、交易所公告、监管文件）。

## Internal Linking

- 站内链接使用相对路径，指向具体文件（如 `../01-fundamentals/README.md`）。
- 不要硬编码站点域名。
- 目录入口统一指向该目录的 `README.md`。
- 移动或重命名文件后，必须同步更新所有引用，保证无死链。

## Cross References

- 首次出现的重要概念，链接到 `glossary` 中对应条目。
- 相关章节之间使用「参见 / See also」互链。
- 公司与行业交叉引用：`09-companies` ↔ `10-industry-maps`。
- 避免循环引用造成阅读困惑，交叉引用应有明确方向性。

## Glossary Rules

- 术语集中维护于 `docs/glossary/`。
- 每个术语条目包含：中文名、英文名 / 缩写、定义、必要示例。
- 定义中立、简洁，不夹带观点。
- 正文首次出现的术语链接到术语表，其后可直接使用。

## Image Naming

- 图片存放于 `assets/images/<主题>/`。
- 命名用 `kebab-case`，语义化：`nvidia-revenue-2020-2025.png`。
- 必须提供替代文本（alt text）。
- 优先矢量或压缩位图（PNG / WebP），单张建议 < 500 KB。
- 图片版权需合规，注明来源。

## Citation Rules

- 关键数据与引述必须给出可核实来源。
- 引用格式统一：`来源：<机构 / 文件>，<年份 / 日期>`。
- 能提供原始链接的，附上稳定链接（如 SEC EDGAR、交易所公告页）。
- 不得引用未经证实的传闻、内幕或小道消息。
- 二手来源应尽量回溯到一手出处。

## Writing Consistency

- 术语、公司名、单位在全书内保持一致（如统一「营收」而非「收入 / 营业额」混用）。
- 数字与单位规范：金额标注币种（USD / CNY），大数用「亿 / 万亿」并保持一致。
- 时态与口吻统一，保持中立叙述。
- 复用统一模板（见 `templates/`）以保证结构一致。
- 提交前对照本指南自查，并通过 markdownlint 与 `mkdocs build`。
