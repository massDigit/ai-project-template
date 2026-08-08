# AI Project Template

Universal AI-native development structure for:
- Antigravity
- Claude Code
- Gemini CLI
- other `AGENTS.md`-compatible coding agents

## 📌 Overview
This repository provides a standardized **AI-Native Development Operating System** enabling optimal collaboration between human developers and AI coding agents.

## 🗂️ Documentation & Memory Structure

- **`AGENTS.md`** : Master entry point, documentation routing, decision rules, and non-negotiable agent contracts.
- **`docs/`** : Domain documentation (architecture, stack, business rules, API, database).
- **`.ai/`** : Active project memory:
  - `CONTEXT.md` → Project identity & vision
  - `STATE.md` → Current snapshot & active focus
  - `TASKS.md` → Backlog & active tasks
  - `RULES.md` → Non-negotiable engineering rules
  - `DECISIONS.md` → Approved Architectural Decision Records (ADRs)
  - `ASSUMPTIONS.md` → Unconfirmed assumptions awaiting user validation
- **`.agents/skills/`** : Automated workflows & agent procedures (including `project-bootstrap`).

## 🚀 Getting Started

### 1. Bootstrap a New Project
Clone this repository into your new project directory, then use the `project-bootstrap` skill with your high-level project description:

```bash
git clone git@github.com:massDigit/ai-project-template.git my-new-project
cd my-new-project
```

Ask your AI assistant:
> "Bootstrap this project: [Describe your project vision, target audience, and key requirements]"

The `project-bootstrap` procedure will systematically generate all initial documentation (`docs/` and `.ai/`) before any code is written.

### 2. Daily Workflow
```bash
# Check current project snapshot
cat .ai/STATE.md

# Run validation suite
npm test
```
