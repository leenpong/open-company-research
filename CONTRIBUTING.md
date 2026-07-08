# 贡献指南

感谢你对 **Open Company Research** 的关注！本项目是一个长期维护的开源知识库，
任何形式的贡献都非常欢迎——从修正一个错别字，到补充一篇完整的公司研究。

## 目录

- [行为准则](#行为准则)
- [我可以贡献什么](#我可以贡献什么)
- [开始之前](#开始之前)
- [本地环境搭建](#本地环境搭建)
- [贡献流程](#贡献流程)
- [写作与格式规范](#写作与格式规范)
- [Commit 规范](#commit-规范)
- [Pull Request 规范](#pull-request-规范)
- [免责声明](#免责声明)

## 行为准则

参与本项目即表示你同意遵守我们的 [行为准则](./CODE_OF_CONDUCT.md)。

## 我可以贡献什么

- 📝 **内容**：撰写或完善公司研究、行业专题、方法论。
- 🐛 **纠错**：修正错别字、数据错误、失效链接。
- 🎨 **图表**：绘制 Mermaid 图、思维导图、时间线。
- 🧩 **模板**：改进 `templates/` 下的研究模板。
- 🛠️ **工具**：优化脚本、CI 流程、站点配置。

## 开始之前

- 提交较大改动前，请先创建一个 Issue 与维护者讨论方向。
- 检索现有 Issue / PR，避免重复工作。
- 所有内容必须 **中立、可验证、注明来源**，严禁投资建议或荐股。

## 本地环境搭建

```bash
# 1. Fork 并克隆仓库
git clone https://github.com/<your-name>/open-company-research.git
cd open-company-research

# 2. 创建虚拟环境并安装依赖
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# 3. 启用 pre-commit 钩子
pip install pre-commit
pre-commit install

# 4. 本地预览
mkdocs serve
```

## 贡献流程

1. **Fork** 本仓库并克隆到本地。
2. 从 `main` 切出特性分支：`git checkout -b feat/your-topic`。
3. 进行修改，并遵循 [写作规范](./STYLE_GUIDE.md)。
4. 本地运行 `pre-commit run --all-files` 与 `mkdocs build` 确保通过。
5. 提交并推送分支，发起 Pull Request。
6. 等待 CI 通过与维护者评审。

## 写作与格式规范

请务必阅读 [STYLE_GUIDE.md](./STYLE_GUIDE.md)，其中包含 Markdown、标题、命名、
图片、Mermaid、引用、文件组织等完整规范。

## Commit 规范

本项目采用 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/)：

```text
<type>(<scope>): <subject>
```

常用 `type`：

- `feat` — 新增内容或功能
- `fix` — 修正错误
- `docs` — 文档改动
- `style` — 格式调整（不影响含义）
- `refactor` — 结构重构
- `chore` — 构建 / 工具链 / 杂项
- `ci` — CI 配置变更

示例：`docs(case-study): add NVIDIA business model analysis`

## Pull Request 规范

- 一个 PR 只做一件事，保持聚焦。
- 标题遵循 Conventional Commits 格式。
- 填写 PR 模板中的全部字段。
- 关联相关 Issue（如 `Closes #123`）。
- 确保所有 CI 检查通过。

## 免责声明

本项目仅用于教育与研究目的。所有贡献内容均不构成投资建议。请勿提交任何荐股、
内幕信息或未经证实的市场传闻。
