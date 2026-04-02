# Claude Code for Non-Tech Knowledge Workers — Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Write a compelling guide (README.md + two supplementary files) that persuades non-technical knowledge workers to adopt Claude Code as their AI-assisted project/document management tool.

**Architecture:** Single long-form README.md as the main article (works as both GitHub landing page and publishable blog post), with two supplementary markdown files linked from the main article for deeper dives on skills and git.

**Format:** Markdown only. No code, no build system, no dependencies. Conversational tone — "here's what I discovered" not "you should do this."

---

### Task 1: README.md — Hook, Problem, and Formula (Sections 1-3)

**Files:**
- Create: `README.md`

- [ ] **Step 1: Write the Hook (Section 1)**

Open with the gap between chatbot and workspace. Target: 3-5 sentences.

Key points:
- Address the reader directly — you already use Claude (or ChatGPT, etc.)
- Pose the question: what if your AI could manage your projects, not just answer questions?
- Create curiosity, not a sales pitch

- [ ] **Step 2: Write The Problem (Section 2)**

Describe the ceiling of chatbot-style AI. Target: 1-2 short paragraphs.

Key points:
- Every conversation starts from scratch — no memory of yesterday
- You copy-paste context in, hope it fits, lose it next session
- The AI can't see your actual files, your project structure, your history
- It's powerful but disconnected from your real work

- [ ] **Step 3: Write The Formula (Section 3)**

Introduce the four ingredients. Target: 4 short subsections, 2-4 sentences each.

- **Memory** — AI remembers your preferences, project context, past decisions across sessions. You stop repeating yourself.
- **Project folder as context** — AI sees your whole project. Every file, always available. No more pasting snippets.
- **Git (version control)** — Every change is tracked. Undo anything. See what changed and when. Frame as a life skill for document management.
- **Markdown** — Lightweight, readable by both human and AI, works everywhere, no vendor lock-in. Your documents aren't trapped in proprietary formats.

Each ingredient explained in terms of what it does for the reader's workflow.

- [ ] **Step 4: Commit**

```bash
git add README.md
git commit -m "docs: add hook, problem statement, and formula sections"
```

---

### Task 2: README.md — Claude Code vs Desktop (Section 4)

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Write Claude Code vs. Claude Desktop (Section 4)**

Not a feature comparison table. A reframing. Target: 2-3 short paragraphs.

Key points:
- Claude Desktop is a chatbot you visit. Claude Code is an agent that lives in your workspace.
- Same brain (same Claude model), fundamentally different relationship to your work.
- Desktop: you bring context to it. Code: it has your context already.
- This isn't "better chatbot" — it's a different category entirely.

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "docs: add Claude Code vs Desktop comparison"
```

---

### Task 3: README.md — The Mental Model (Section 5)

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Write the Mental Model intro**

Brief framing paragraph: "Here's the conceptual framework for Claude Code. You don't need all of these on day one. But knowing they exist means you'll recognize when one solves a problem you're having."

- [ ] **Step 2: Write the Agent concept**

Target: 1 short paragraph.

Key points:
- Claude Code isn't answering questions — it's taking actions
- It reads files, creates documents, searches your project, runs multi-step tasks
- You describe what you want; it figures out the steps
- A chatbot waits for your next message. An agent goes and does the work.
- **Sub-agents**: it can spin up smaller agents that handle parts of a task in parallel — like delegating "you research this, you draft that, I'll put it together"

- [ ] **Step 3: Write Context Management**

Target: 1 short paragraph.

Key points:
- Large conversation window — much bigger than typical chatbots
- Automatic compression of earlier messages so the conversation can keep going
- Reads files on demand rather than needing you to paste them in
- Your whole project is accessible, but Claude is smart about what it holds in focus

- [ ] **Step 4: Write Memory**

Target: 2-4 sentences.

Key points:
- Persists across conversations — preferences, project context, decisions
- You stop repeating yourself every session
- Claude learns how you work over time

- [ ] **Step 5: Write CLAUDE.md**

Target: 2-4 sentences.

Key points:
- A file you write that tells Claude how to behave in your project
- Standing instructions — like onboarding a new team member
- "Here's how we do things here"

- [ ] **Step 6: Write Skills**

Target: 2-4 sentences.

Key points:
- Pre-written instructions that teach Claude specific abilities
- Like hiring a specialist instead of a generalist
- You install them, Claude gains new capabilities

- [ ] **Step 7: Write Plugins**

Target: 2-4 sentences.

Key points:
- Bundles of skills, commands, and tools packaged together
- Like apps on your phone — each adds related capabilities

- [ ] **Step 8: Write MCP Servers**

Target: 2-4 sentences.

Key points:
- Bridges connecting Claude to external services (Gmail, Calendar, Notion, Slack)
- Doors you open so Claude can reach outside your project folder

- [ ] **Step 9: Write Hooks**

Target: 2-4 sentences.

Key points:
- Automated triggers: "When Claude does X, also do Y"
- Like email rules — automation that runs without you asking each time

- [ ] **Step 10: Commit**

```bash
git add README.md
git commit -m "docs: add mental model section — agent, context, memory, skills, plugins, MCP, hooks"
```

---

### Task 4: README.md — Getting Started Walkthrough (Section 6)

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Write the walkthrough intro**

Brief framing: this teaches the pattern, not a specific project. The reader fills in their own content.

- [ ] **Step 2: Write Install Claude Code**

Brief directions + link to official docs. Acknowledge this is the one slightly technical step (need a terminal, Node.js). Keep it short — don't reproduce the official install guide.

- [ ] **Step 3: Write Create Your Project Folder**

Just a folder on your computer. Everything for one project goes here. Simple but foundational.

- [ ] **Step 4: Write Start Claude Code**

`claude` in terminal, pointed at your folder. This is the "aha moment" — Claude can now see everything. No more copy-pasting.

- [ ] **Step 5: Write Start Working**

Show 3-5 example interactions a knowledge worker would actually use:
- "Summarize everything in this folder"
- "Create a meeting notes template"
- "What did I write last week about X?"
- "Draft a response to this email based on the project brief"

Demonstrate it's conversational — same as chatting with Claude Desktop, but now with full context.

- [ ] **Step 6: Write Save Your Progress with Git**

Light git intro:
- Git takes snapshots of your project
- You can ask Claude to do it: "commit my changes"
- You can undo anything, see what changed and when
- Emphasize: this is a life skill for document management, valuable beyond Claude Code — tracked history, undo, sync across machines
- Link to `git-for-docs.md` for more

- [ ] **Step 7: Write Make It Yours**

Write a CLAUDE.md with your preferences. Claude now knows how you work. This is where it stops being a generic tool and becomes *your* tool.

- [ ] **Step 8: Commit**

```bash
git add README.md
git commit -m "docs: add getting started walkthrough"
```

---

### Task 5: README.md — Use Case, Tools, Closing (Sections 7-9)

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Write My Use Case (Section 7)**

Meta-example: this very guide was built using Claude Code. Walk through what that looked like:
- Started with a project folder and CLAUDE.md
- Brainstormed the structure through conversation (the reader just read the result)
- Claude managed context, remembered decisions, used skills for structured brainstorming
- Git tracked every draft, every revision
- The repo they're reading IS the proof of concept

Keep it concrete and personal. Show, don't tell.

- [ ] **Step 2: Write Recommended Tools (Section 8)**

Curated short list of must-have skills/plugins. For each:
- Name
- One sentence: what it does
- One sentence: why it's useful for a non-technical user

(Author to fill in specific tools — leave structure ready with 1-2 examples if known.)

- [ ] **Step 3: Write Go Explore (Section 9)**

Short closing. 3-5 sentences:
- The point is to internalize the pattern: folder + markdown + git + agent
- Make it your own — apply to whatever you manage
- Link to resources for finding more skills/plugins
- Encouraging, not prescriptive

- [ ] **Step 4: Commit**

```bash
git add README.md
git commit -m "docs: add use case, recommended tools, and closing"
```

---

### Task 6: Supplementary File — skills-guide.md

**Files:**
- Create: `skills-guide.md`

- [ ] **Step 1: Write skills-guide.md**

Deeper explanation of Skills for readers who want to go beyond the curated list. Target: ~500-800 words.

Sections:
- **What are Skills?** — Expand on the mental model definition. Skills are instructions that teach Claude how to approach specific tasks with expertise.
- **Where to find them** — Official plugin registry, community plugins, how to discover what's available.
- **How to install them** — Step by step, in plain language.
- **How to use them** — They activate automatically when relevant, or you can invoke them with `/skillname`.
- **Examples** — 2-3 concrete examples of skills in action for non-technical use cases.

- [ ] **Step 2: Commit**

```bash
git add skills-guide.md
git commit -m "docs: add skills guide supplementary file"
```

---

### Task 7: Supplementary File — git-for-docs.md

**Files:**
- Create: `git-for-docs.md`

- [ ] **Step 1: Write git-for-docs.md**

Git as a life skill for document management. Target: ~500-800 words.

Sections:
- **Why version control for documents?** — The pitch: tracked history, undo anything, sync across machines, see what changed and when. Not just for code.
- **The key idea** — Git takes snapshots (commits) of your project. Each snapshot is a moment in time you can return to.
- **You don't need to learn git** — Claude Code handles it for you. But understanding the concept is powerful.
- **The few commands that matter** — For the curious: `git status`, `git add`, `git commit`, `git log`. Or just ask Claude: "save my progress", "what changed since yesterday", "undo my last change."
- **Git + GitHub** — Your project, backed up and shareable. Brief mention of GitHub as the remote backup / sharing layer.

- [ ] **Step 2: Commit**

```bash
git add git-for-docs.md
git commit -m "docs: add git for docs supplementary file"
```

---

### Task 8: Final Review and Polish

**Files:**
- Modify: `README.md`
- Modify: `skills-guide.md`
- Modify: `git-for-docs.md`

- [ ] **Step 1: Read through all three files end to end**

Check for:
- Consistent tone (conversational, confident, not preachy)
- No jargon left unexplained
- Links between files work (README links to supplementary files)
- No repetition across files
- Flow of the main article reads naturally as a single piece

- [ ] **Step 2: Fix any issues found**

- [ ] **Step 3: Final commit**

```bash
git add README.md skills-guide.md git-for-docs.md
git commit -m "docs: final review and polish"
```
