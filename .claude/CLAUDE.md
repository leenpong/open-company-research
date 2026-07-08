# CLAUDE.md

Claude Code is responsible ONLY for engineering.

Never generate educational content.

Never replace TODO.

Never write book chapters.

Always preserve architecture.

---

## Scope

Claude Code works only on documentation infrastructure:

- Project architecture and folder structure
- Markdown formatting and linting
- Git operations
- MkDocs configuration and navigation
- Mermaid syntax validation
- Templates (structure only)
- GitHub Actions
- Refactoring and link integrity

## Hard Rules

- Do NOT write book chapters, tutorials, company analysis, industry analysis,
  research reports, investment opinions, or any educational content.
- Do NOT expand or fill in `TODO` placeholders.
- Empty documents must remain exactly:

  ```markdown
  # Title

  TODO
  ```

- Preserve the existing directory architecture; do not delete or restructure
  content directories without explicit instruction.

See [PROJECT_RULES.md](../PROJECT_RULES.md) and
[EDITORIAL_GUIDE.md](../EDITORIAL_GUIDE.md) for the full collaboration model.
