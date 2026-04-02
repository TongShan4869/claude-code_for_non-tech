# Design Spec: Claude Code for Non-Tech Knowledge Workers

## Overview

A guide that persuades non-technical knowledge workers — who already use Claude Desktop or similar chatbots — to adopt Claude Code as their AI-assisted project and document management tool. Distributed as a GitHub repo (README.md as the main article) and publishable as a standalone blog post.

## Audience

Curious professionals who already use AI chatbots. They're comfortable with technology but not developers. They don't use terminals, git, or markdown in their daily work — yet. They're open to upgrading their workflow if the case is compelling.

## Deliverables

### README.md — Main Article

A single long-form article that works both as a GitHub landing page and as a publishable blog post. Conversational, confident tone — "here's what I discovered" not "you should do this."

#### Structure

**1. Hook**
Open with the gap: "You use Claude to chat. But what if your AI could actually manage your projects?" Frame the shift from chatbot to workspace.

**2. The Problem**
Chatbots are stateless and disconnected. Every conversation starts from scratch. You copy-paste context in. The AI can't see your actual files. It's powerful but limited by the interface.

**3. The Formula**
The four ingredients that turn a chatbot into a workspace:
- **Memory** — Claude remembers preferences, project context, and past decisions across sessions.
- **Project folder as context** — Claude sees your whole project. No more pasting snippets.
- **Git (version control)** — Every change is tracked. Undo anything. See what changed and when. A life skill for document management, not just coding.
- **Markdown** — Lightweight, readable by both human and AI, works everywhere, no vendor lock-in.

Each ingredient explained in terms of what it does for the reader's workflow, not how it works technically.

**4. Claude Code vs. Claude Desktop**
Not a feature comparison table. A reframing: Claude Desktop is a chatbot you visit. Claude Code is an agent that lives in your workspace. Same brain, fundamentally different relationship to your work.

**5. The Mental Model**
Conceptual framework for the Claude Code ecosystem. Enough to understand the architecture and explore independently. Ordered from foundational to extensible:

- **Agent** — Claude Code isn't answering questions — it's taking actions. It reads files, creates documents, searches your project, runs multi-step tasks. You describe what you want; it figures out the steps. Can spin up **sub-agents** to handle parts of a task in parallel — like delegating "you research this, you draft that, I'll put it together."
- **Context Management** — How Claude Code handles what it knows: large conversation window, automatic compression of earlier messages, reads files on demand rather than needing you to paste them in. Your whole project is accessible, but Claude is smart about what it holds in focus at any moment.
- **Memory** — Persists across conversations. Preferences, project context, decisions — so you don't repeat yourself every session.
- **CLAUDE.md** — A file you write that tells Claude how to behave in your project. Standing instructions. Like onboarding a new team member.
- **Skills** — Pre-written instructions that teach Claude specific abilities. Like hiring a specialist instead of a generalist.
- **Plugins** — Bundles of skills, commands, and tools. Like apps on your phone — each adds a set of related capabilities.
- **MCP Servers** — Bridges connecting Claude to external services (Gmail, Calendar, Notion, Slack, etc.). Doors you open so Claude can reach outside your project.
- **Hooks** — Automated triggers. "When Claude does X, also do Y." Like email rules — automation that runs without you asking.

Framing: "You don't need all of these on day one. But knowing they exist means you'll recognize when one solves a problem you're having."

**6. Getting Started (Walkthrough)**
Teach the pattern, not a specific project. The reader fills in their own content.

- **Install Claude Code** — Brief, link to official docs. Acknowledge this is the one slightly technical step (terminal, Node.js).
- **Create your project folder** — Just a folder. Everything for one project goes here.
- **Start Claude Code in that folder** — `claude` in terminal. The "aha moment": no more copy-pasting context.
- **Start working** — Example interactions: "Summarize everything in this folder," "Create a meeting notes template," "What did I write last week about X?"
- **Save your progress with git** — Light intro. Git takes snapshots. Ask Claude to do it ("commit my changes"). Emphasize: this is a life skill for document management, valuable beyond Claude Code.
- **Make it yours** — Write a CLAUDE.md with your preferences. This is where it becomes *your* tool.

**7. My Use Case**
Meta-example: this very guide was built using Claude Code. Walk through what that looked like — the brainstorming, version control, memory, skills — all happening in the repo the reader is currently reading. Self-demonstrating argument.

**8. Recommended Tools**
Curated short list of must-have skills/plugins for non-technical users. Not exhaustive. Brief description of what each does and why. (Specific tools to be filled in by the author.)

**9. Go Explore**
Short closing. The point is to internalize the pattern (folder + markdown + git + agent) and make it your own. Links to resources for finding more skills/plugins. Encouraging, not prescriptive.

### Supplementary Files

**`skills-guide.md`**
Deeper explanation of what Skills are, where to find them, how to install and manage them. For readers who want to go beyond the curated list.

**`git-for-docs.md`**
Git as a life skill for document management. The conceptual pitch (tracked history, undo, sync) plus the minimal commands that matter. Emphasize that Claude Code handles most git operations for you.

## Design Principles

- **Conversational tone** — "Here's what I discovered" not "you should do this"
- **Non-technical audience** — Avoid jargon or explain it plainly when unavoidable
- **Teach the pattern, not a project** — Generic enough for any knowledge worker's use case
- **Self-demonstrating** — The repo itself is an example of the workflow being advocated
- **YAGNI** — No features, sections, or concepts that don't directly serve the argument

## What This Is Not

- Not a Claude Code tutorial for developers
- Not a comprehensive reference manual
- Not a comparison of AI tools
- Not a technical deep-dive into how any of this works internally
