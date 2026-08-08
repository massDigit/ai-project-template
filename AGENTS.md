# AI PROJECT ENTRYPOINT (AGENTS.md)

This repository uses a structured **AI Development Operating System** (AI Dev OS).

## 🚨 Mandatory Startup

Before working on any task, read:

1. `.ai/CONTEXT.md` (Stable project identity)
2. `.ai/STATE.md` (Current snapshot & active focus)
3. `.ai/RULES.md` (Non-negotiable engineering rules)
4. `.ai/CODING_STANDARDS.md` (Style & code conventions)

## ⚡ Context Economy Principle

**Do NOT read the entire repository.**  
Load the minimum amount of context necessary to safely complete the current task.

## 🗺️ Documentation Routing

Inspect **only** the documentation relevant to the current task:

- **Architecture & Data Flow** ➔ `docs/ARCHITECTURE.md`
- **Tech Stack & Dependencies** ➔ `docs/STACK.md`
- **Business Rules & Logic** ➔ `docs/BUSINESS_RULES.md`
- **Database Schemas & Models** ➔ `docs/DATABASE.md`
- **API Contracts & Endpoints** ➔ `docs/API.md`
- **Security & Secrets** ➔ `docs/SECURITY.md`
- **Testing Strategy** ➔ `docs/TESTING.md`
- **CI/CD & Deployment** ➔ `docs/DEPLOYMENT.md`

## 🔍 Before Coding

Search the existing codebase using grep / file view tools.

**Never assume:**
- A function or utility exists
- An API signature or payload format
- A database table or field name
- A dependency or package version
- An architectural pattern

*Verify first.*

## ✅ Before Declaring Completion

Follow `.ai/WORKFLOW.md`.

Run the relevant validation commands:
- Typecheck
- Linter
- Unit tests
- Integration tests
- Production build

*A task is not complete when code is written. A task is complete when it has been empirically verified.*

## 📝 Documentation Maintenance

- **When architecture changes**: Update `docs/ARCHITECTURE.md` and append an entry to `.ai/DECISIONS.md`.
- **When project state changes**: Update `.ai/STATE.md` and `.ai/TASKS.md`.
