# Git for Document Management

## Why version control for documents?

You have been version controlling documents your whole career. You just haven't been doing it well.

"Final_v2_ACTUAL_final.docx" is version control. So is keeping five copies of a report in a folder named "Archive" with dates in the filenames. You already understand the problem — you want to preserve history, be able to go back, and know what changed. You've been solving it with folder chaos and creative filenames.

Git solves the same problem properly. It tracks history automatically. You can undo anything. You can see exactly what changed, when, and why. You can sync your files across machines without emailing yourself attachments. This is not a developer tool that you are being asked to borrow. It is a document management tool that developers discovered first and named confusingly.

---

## The key idea

Git takes snapshots of your project. Each snapshot — called a "commit" — captures the exact state of every file in your folder at that moment. You can return to any snapshot, compare any two snapshots, or branch off in a new direction and merge back later.

Think of it as Time Machine for your project folder, but more deliberate. You choose when to take the snapshot, and you label it with a plain-English description of what changed: "Added client feedback from Tuesday call" or "Rewrote executive summary." Six months from now, you can scroll through that history and find exactly the moment something changed — and get it back.

The folder on your computer is called your "repository" or "repo." It looks like any other folder. The difference is that git is quietly watching it, ready to take a snapshot whenever you ask.

---

## You don't need to learn git

Claude Code handles it for you.

You say "commit my changes" and Claude writes the snapshot with a proper description. You say "what changed since yesterday?" and Claude reads the history and tells you. You say "undo my last change" and Claude finds the right snapshot and restores it. You say "show me what the introduction looked like two weeks ago" and Claude pulls it up.

The git commands exist if you are curious, but they are never required. Everything you need to do, you can describe in plain language and Claude will handle the mechanics.

---

## The few commands that matter

For the curious reader who wants to understand what is happening under the hood:

| Command | What it does |
|---|---|
| `git status` | Shows what has changed since the last snapshot |
| `git add filename` | Stages a file to be included in the next snapshot |
| `git commit -m "description"` | Takes the snapshot with a label you write |
| `git log` | Shows the full history of all snapshots |

You can also just ask Claude:

- "Save my progress" — Claude stages and commits everything with a sensible message
- "What changed since yesterday?" — Claude reads the log and summarizes
- "Undo my last change" — Claude finds the previous snapshot and restores
- "Show me the history of this project" — Claude walks you through what happened when

The commands and the plain-English requests do the same thing. Use whichever feels natural.

---

## Git and GitHub

Your project folder lives on your computer. That is where git works. GitHub is a separate service — it is where you can back up your repository online and share it with others.

Think of GitHub as cloud backup with complete history. If your laptop dies, your project is still there — not just the latest version, but every snapshot you ever took. If you want to collaborate with a colleague, you give them access and they can see the whole history, make changes, and keep everything in sync without emailing files back and forth.

The guide you are reading right now is hosted on [GitHub](https://github.com/TongShan4869/claude-code_for_non-tech). The repository is the project. The files, the history, the changes over time — all of it lives there, accessible from any machine, never lost.

You do not need a GitHub account to start. Git works perfectly well on your local machine alone. But when you are ready to back things up or share your work, GitHub is where you go next — and Claude can walk you through connecting the two.

---

The goal here is not for you to become a git expert. It is for you to understand what git is doing so that when Claude says "I've committed your changes," you know what that means and why it matters. You are building a paper trail you can always go back to. That is something worth having.
