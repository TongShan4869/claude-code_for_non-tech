## Content Summary

This is a guide/article arguing that Claude Code — despite its developer-sounding name — is a powerful project and document management tool for non-technical knowledge workers. The core argument has three pillars:

1. Claude Code does far more than coding — it manages documents, projects, workflows
2. Claude Code is the "full version" of what Desktop Projects and Cowork offer in simplified form — with version control, extensibility, and full transparency
3. The formula: AI agent + project folder context + git + markdown = an actual collaborator, not just a chatbot

The author is a researcher who uses both code and documents, writing from firsthand experience. The article serves as both guide and proof of concept — the guide itself was built using the workflow it advocates. Tone is conversational and confident, addressed to non-technical readers who already use AI chatbots but haven't explored Claude Code.

## Terminology

| English | Chinese | Notes |
|---------|---------|-------|
| Claude Code | Claude Code | Product name, keep English |
| Claude Desktop | Claude Desktop | Product name |
| Projects | Projects | Claude Desktop feature |
| Cowork | Cowork | Claude Desktop feature |
| CLAUDE.md | CLAUDE.md | Filename |
| Skills | Skills | Claude Code concept |
| Plugins | 插件 | |
| Hooks | Hooks | Claude Code concept, explain on first use |
| MCP Servers | MCP 服务器 | Model Context Protocol, explain on first use |
| Markdown | Markdown | |
| Git | Git | Explain as version control on first use |
| GitHub | GitHub | |
| Terminal | 终端 | |
| Node.js | Node.js | |
| Knowledge Worker | 知识工作者 | |
| Version Control | 版本控制 | |
| Commit | 提交 | Git concept |
| Push | 推送 | Git concept |
| Stage | 暂存 | Git concept |
| Sub-agents | 子智能体 | |
| Context window | 上下文窗口 | |
| Slash command | 斜杠命令 | e.g., /init, /brainstorm |
| Workflow | 工作流 | |
| Repository / repo | 仓库 | Git concept |
| Snapshot | 快照 | Git metaphor used in the article |

## Tone & Style

- Conversational, confident, first-person where applicable
- "Here's what I discovered" attitude, not preachy or instructional
- Uses direct address ("you") throughout
- Metaphors drawn from everyday life: "sealing an envelope", "like email filters", "like apps on your phone"
- Short paragraphs, punchy sentences
- Mixes explanation with opinion — editorial voice, not documentation voice
- The article explicitly avoids jargon or explains it when unavoidable

Target register: 同样的对话式风格，自信而不说教。用"你"直接称呼读者。保持短段落和有力的句子。

## Translation Challenges

- **"Claude Code" name paradox**: The article repeatedly plays on the irony that "Code" in the name scares non-developers away. This irony works in English but needs careful handling in Chinese — the reader must feel the same "wait, this isn't just for coders?" moment.
- **Product name hierarchy**: Projects, Cowork, Claude Desktop, Claude Code — these are all Anthropic product names that should stay in English but need enough context so Chinese readers can follow the relationships.
- **Git metaphors**: The article uses accessible metaphors for git concepts (snapshots, envelopes, safety net). These metaphors need to feel natural in Chinese, not translated-English.
- **"Formula" framing**: Section 3 calls the four ingredients a "formula" — this conceptual metaphor should carry over naturally.
- **Mermaid diagram labels**: The flowchart in Section 6 has emoji + English labels. These should be translated to Chinese labels.
- **Inline code/commands**: `/init`, `/brainstorm`, `/clear`, `/compact`, `/rewind`, `claude` — keep as-is (they are literal commands).
- **Tone calibration**: The original walks a fine line between enthusiasm and credibility. Overselling in Chinese would feel like marketing copy (营销文); under-selling would lose the article's energy. Match the "colleague sharing a discovery" register.
- **"Knowledge workers"**: 知识工作者 is the standard translation but less commonly used in casual Chinese. May need to contextualize or use 非技术岗位的职场人 in places.
