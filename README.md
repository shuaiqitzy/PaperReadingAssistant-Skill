# PaperReadingAssistant-Skill

`PaperReadingAssistant` 是一个面向医疗影像、机器学习和人工智能论文的 Codex skill。它可从本地 PDF、DOI、arXiv 链接、论文标题或网页链接出发，按 `0-8` 阶段递进式解释论文；仅在用户明确要求“深入 / follow”时，继续分析脆弱假设、最小复现、反例和非增量 follow-up idea。

## 文件说明

| 文件 | 作用 |
| --- | --- |
| `SKILL.md` | Skill 主入口：定义输入、检索优先级、`0-8` / `9-12` 运行门控、证据分级和输出风格。 |
| `Prompt.txt` | 用户提供的原始论文阅读 prompt，便于审阅、复用或二次修改。 |
| `agents/openai.yaml` | Codex 界面配置：显示名为 `PaperReadingAssistant`，并限制为显式调用 `$paper-reading-assistant`。 |
| `references/staged-reading-protocol.md` | 按 `0-12` 组织的完整递进式论文阅读协议与输出要求。 |
