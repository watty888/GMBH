# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

This is an **Obsidian vault** (knowledge base), not a software project. It serves as the internal knowledge system for an AI consulting company focused on building reliable AI agents — prompt engineering, test harnesses, and agent QA.

Git syncing is handled by the `obsidian-git` plugin.

## Vault Structure

| Folder | Purpose |
|---|---|
| `00_Inbox/` | Raw captures; triage into other folders |
| `10_Permanent/` | Atomic, timeless knowledge notes |
| `20_Company/` | Company strategy, services, pricing, ICP |
| `40_Playbooks/` | Repeatable delivery processes and specs |
| `50_Experiments/` | Hypothesis → test → result logs |
| `60_Client-Work/` | Per-client deliverables and decisions |
| `70_Case-Library/` | Domain-specific pattern write-ups |

## Conventions

- **MOC files** (`MOC - *.md`) are Maps of Content — index pages that link related notes. Each major folder has one.
- **Template files** (`Template - *.md`) define the structure for new notes in their folder.
- **YAML frontmatter** uses `type` and `status` fields for metadata.
- Internal links use Obsidian `[[wikilink]]` syntax with relative paths from vault root.
- Notes should be atomic (one idea per note) in `10_Permanent/`.

## When Editing This Vault

- Preserve `[[wikilink]]` syntax — do not convert to standard markdown links.
- Keep YAML frontmatter intact when editing existing notes.
- When creating new notes, use the corresponding `Template -` file from that folder.
- When adding a new note, also add a link to it from the relevant MOC file.
