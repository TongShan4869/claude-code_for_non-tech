# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

A guide for non-technical knowledge workers to use Claude Code as an AI-assisted project and document management tool. The repository itself is the proof of concept — built entirely with Claude Code using the workflow it advocates.

## Core Arguments

1. Claude Code does far more than coding — it manages documents, projects, workflows, and is available to non-developers
2. Claude Code is the full version of what Desktop Projects and Cowork offer in simplified form — local-first, with version control, deep customization, and full transparency
3. Effective document management = AI agent with memory + project folder context + version control (git) + markdown format
4. Provide curated must-have skills/plugins, then let readers explore independently

## Framing Rules

- **Acknowledge Desktop Projects and Cowork honestly.** Don't argue against a straw man. Desktop Projects has basic memory/context. Cowork has local file access and autonomous task execution. Our argument is that Claude Code is the full system — version control, ecosystem, transparency — not that the others are useless.
- **Position as a spectrum, not a rivalry.** Desktop = conversation. Cowork = task runner. Claude Code = workspace/system.
- **Address the name head-on.** "Claude Code" sounds like it's for developers. It isn't. Say so directly.

## Writing Guidelines

- **Audience is non-technical.** Avoid jargon or explain it plainly when unavoidable (e.g., define "terminal", "Node.js", "slash command").
- **All content is in Markdown.** This is both the subject matter and the format we use.
- **Frame everything around document/project management,** not software engineering.
- **Tone: conversational, confident, not preachy.** "Here's what I discovered" not "you should do this."
- **Explain Claude Code concepts in practical terms** — what they do for the user, not how they work internally.

## Repository Structure

- `README.md` — Main article (works as GitHub landing page and standalone blog post)
- `skills-guide.md` — Supplementary deep-dive on Skills
- `git-for-docs.md` — Supplementary deep-dive on git for document management
- `docs/superpowers/specs/` — Design spec
- `docs/superpowers/plans/` — Implementation plan
- No build system, no tests, no dependencies — this is a documentation project
