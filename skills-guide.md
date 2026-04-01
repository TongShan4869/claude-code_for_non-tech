# Understanding Skills

Skills are the mechanism that lets Claude Code go beyond general assistance and work like a trained specialist in a specific domain. This guide explains what they are, how to find them, and how to use them — without any technical background required.

---

## What Are Skills?

Think of Skills as pre-written instruction sets that reshape how Claude approaches a task. When a skill is active, Claude doesn't just know more — it works differently. It follows a structured process, asks the right questions in the right order, and produces output that fits a recognized standard.

A good analogy: the difference between asking a generalist assistant to "plan a client presentation" versus handing the same request to someone who has run hundreds of client presentations and has a tested process for it. The information they draw on might overlap, but the specialist brings method, not just knowledge.

Skills cover things like structured brainstorming, systematic debugging, step-by-step planning, writing workflows, commit message conventions, and more. Each one is a set of guidance tuned to a specific kind of work.

The key distinction: Skills change **how** Claude works, not just what it knows. That's why they're worth understanding separately from general prompting.

---

## Where to Find Skills

Skills come packaged inside **plugins**. A plugin is a bundle that may contain one skill or many. You don't need to know anything about how plugins are built to use them — you just need to know where to find them.

There are three main sources:

- **The official Claude Code plugins registry** — a curated list of plugins maintained by Anthropic. These are vetted and ready to use.
- **Community-built plugins on GitHub** — the broader Claude Code community publishes plugins publicly. Quality varies, but many are excellent and cover niche use cases the official registry doesn't.
- **Asking Claude directly** — if you're not sure what's available, just ask: "What plugins are available?" Claude can surface options relevant to what you're trying to do.

---

## How to Install a Plugin

Installation is straightforward. You don't need to touch any configuration files or run any commands yourself.

1. **Find a plugin you want.** Either browse the registry, search GitHub, or ask Claude for a recommendation.
2. **Ask Claude to install it.** You can say something like "Install the superpowers plugin" or paste in a GitHub URL: "Install this plugin: github.com/example/plugin-name."
3. **Claude handles the rest.** It fetches and installs the plugin without any further input from you.
4. **The skills are now available.** From that point on in your sessions, the skills that came with the plugin are active and ready to use.

That's it. No settings menus, no configuration steps.

---

## How to Use a Skill

Once installed, skills work in two ways:

**Automatic activation.** Many skills are designed to detect when they're relevant and activate on their own. If you start describing a brainstorming problem, a brainstorming skill may kick in without you doing anything. Claude recognizes the pattern of what you're doing and applies the appropriate method.

**Manual invocation.** You can also call a skill directly by name using a slash command. For example:
- `/commit` — triggers a commit skill
- `/brainstorm` — triggers a brainstorming skill

This is useful when you want to be deliberate about which approach you're using, or when the automatic detection doesn't fire.

---

## Three Examples in Practice

**Brainstorming a structural change.** You say: "I have an idea for restructuring how we format our client reports." With a brainstorming skill active, Claude doesn't just riff — it walks you through a structured process. It surfaces assumptions, identifies what you're actually trying to solve, explores alternative framings, and helps you pressure-test the idea before you commit to it. The output is clearer thinking, not just a list of bullet points.

**Committing code changes.** You type `/commit`. Claude reviews everything that's changed in your working files, groups related changes together, writes a commit message that explains the "why" rather than just the "what," and creates a clean git commit. For someone new to version control, this turns a confusing manual process into a one-word command.

**Turning a vague goal into a plan.** You say: "I want to overhaul how our team handles client onboarding." A writing plans skill takes that and builds it out into a concrete, step-by-step plan with clear phases, ownership suggestions, and defined deliverables. Instead of an open-ended conversation, you get a structured document you can act on immediately.

---

## The Bottom Line

Skills are what separate Claude Code from a general-purpose chat assistant. They bring process and structure to the kinds of knowledge work that benefit most from it. Once you know they exist and how to invoke them, they become one of the more reliable tools in the toolkit.

If you haven't explored the plugins registry yet, that's the natural next step.
