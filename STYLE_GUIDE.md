# 写作与格式规范（Style Guide）

本规范定义 **Open Company Research** 的写作与格式标准。所有贡献都必须遵循，
以保证知识库在 300+ 文档规模下依然一致、可维护、可检索。

## 目录

- [总则](#总则)
- [Markdown 规范](#markdown-规范)
- [标题规范](#标题规范)
- [命名规范](#命名规范)
- [图片规范](#图片规范)
- [Mermaid 规范](#mermaid-规范)
- [引用与来源规范](#引用与来源规范)
- [文件组织规范](#文件组织规范)
- [Git Commit 规范](#git-commit-规范)
- [目录与导航规范](#目录与导航规范)

## 总则

- 语言：以 **简体中文** 为主，专有名词保留英文原文（如 NVIDIA、EBITDA）。
- 中英文之间、中文与数字之间加一个空格：`营收 100 亿美元`、`NVIDIA 的 GPU`。
- 客观中立，所有结论必须有数据或来源支撑。
- **禁止投资建议**：不得出现「买入」「卖出」「目标价」等荐股表述。
- 每个文档聚焦一个主题，避免内容膨胀。

## Markdown 规范

- 遵循 [`.markdownlint.json`](./.markdownlint.json) 规则。
- 使用 ATX 风格标题（`#`），而非下划线。
- 无序列表统一用 `-`，有序列表用 `1.`（渲染器自动编号）。
- 代码块使用围栏（```` ``` ````）并标注语言。
- 强调用 `*斜体*` 与 `**加粗**`。
- 每个文件以单个 `#` 一级标题开头，且全文只有一个一级标题。
- 文件末尾保留一个空行。

## 标题规范

- 标题层级不得跳级（`#` → `##` → `###`）。
- 标题使用名词短语，简洁明确，不以标点结尾。
- 同一文档内同级标题不重复。
- 一级标题即页面标题，用于自动生成导航。

## 命名规范

- 目录：`NN-kebab-case`，前缀两位数字用于排序，如 `01-fundamentals`。
- Markdown 文件：`kebab-case.md`，如 `business-model.md`。
- 公司 / 专有名词文件：保留可识别名称，如 `nvidia.md`。
- 资源文件：`kebab-case`，并置于 `assets/` 对应子目录。
- 一律使用小写字母、数字与连字符，避免空格与中文文件名。

## 图片规范

- 图片存放于 `assets/images/<主题>/`。
- 文件名语义化：`nvidia-revenue-2020-2025.png`。
- 必须提供替代文本：`![NVIDIA 2020–2025 营收](../assets/images/...)`。
- 优先使用矢量或压缩后的 PNG / WebP，单张建议 < 500 KB。
- 引用使用相对路径，便于本地与线上一致。

## Mermaid 规范

- 使用围栏语法 ` ```mermaid `。
- 图表需有清晰主题，节点文字简洁。
- 复杂图表拆分为多个小图，而非一张巨图。
- 方向优先 `TD`（自上而下）或 `LR`（自左而右）。

````markdown
```mermaid
flowchart LR
  A[营收] --> B[毛利]
  B --> C[营业利润]
  C --> D[净利润]
```
````

## 引用与来源规范

- 数据必须注明来源（年报、财报、公开披露）与时间。
- 引用外部观点使用引用块 `>` 并标注出处。
- 链接使用有意义的锚文本，避免「点击这里」。
- 关键数据尽量给出原始出处链接（如 SEC、交易所公告）。

## 文件组织规范

- 每个 `docs/` 子目录必须包含 `README.md` 作为该章节入口。
- 相关文档就近组织在同一目录下。
- 资源与正文分离：正文在 `docs/`，静态资源在 `assets/`。
- 模板放在 `templates/`，示例产出放在 `examples/`。

## Git Commit 规范

采用 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/)：

```text
<type>(<scope>): <subject>
```

- `type`：`feat` / `fix` / `docs` / `style` / `refactor` / `chore` / `ci`。
- `scope`：改动范围，如 `case-study`、`fundamentals`、`ci`。
- `subject`：祈使句、简洁、不以句号结尾。

示例：`feat(fundamentals): add discounted cash flow chapter`

## 目录与导航规范

- 目录采用 `NN-` 数字前缀控制排序。
- 每个目录的 `README.md` 承担章节索引职责。
- 导航依赖 `awesome-pages` 插件与 `.pages` 文件自动生成。
- 新增目录时同步更新 `mkdocs.yml`（如需显式配置）。
