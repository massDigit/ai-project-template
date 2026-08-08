---
name: project-bootstrap
description: Procedure for initializing a new project documentation and architecture from a user prompt before writing code
---

# Project Bootstrap Procedure

## Overview
This procedure transforms a high-level project description into a complete, structured, AI-native documentation and architecture baseline **before any code is written**.

---

## 🔄 Bootstrap Workflow

```
User Project Description
         ↓
 1. Requirements Extraction & Classification
         ↓
 2. Initial Documentation Generation (`docs/` & `.ai/`)
         ↓
 3. Architecture & Tech Stack Proposal
         ↓
 4. User Review & Explicit Validation
         ↓
 5. State & Memory Lock (`STATE.md`)
         ↓
 6. Ready for Development
```

---

## Step 1: Requirements Extraction & Classification

Analyze the user's project request and separate input into four distinct categories:
- **USER REQUIREMENT**: Explicit user request (non-negotiable).
- **ASSUMPTION**: Agent-inferred technical choice requiring validation.
- **PROPOSAL**: Architectural or tech stack option submitted for user feedback.
- **VALIDATED DECISION**: Choice explicitly confirmed by the user.

---

## Step 2: Populate Domain Documentation (`docs/`)

Fill in the specification files in `docs/` based on the project description:

1. **`docs/PROJECT.md`**: Project overview, core purpose, problem solved, target personas.
2. **`docs/FEATURES.md`**: List target features categorized by priority (MVP vs V2).
3. **`docs/BUSINESS_RULES.md`**: Core business domain rules, validations, and constraints.
4. **`docs/STACK.md`**: Proposed technology stack (frontend, backend, database, deployment).
5. **`docs/ARCHITECTURE.md`**: System architecture, data flow, component breakdown.

---

## Step 3: Populate Project Memory (`.ai/`)

Fill in the operational memory files in `.ai/`:

1. **`.ai/CONTEXT.md`**:
   - Stable project vision, problem statement, target audience, founding principles.
2. **`.ai/STATE.md`**:
   - Phase: *Bootstrap & Architecture Validation*
   - Current Focus: *Awaiting user validation on proposed architecture and tech stack*
   - Completed: Initial documentation baseline generated via `project-bootstrap`.
3. **`.ai/TASKS.md`**:
   - Initial backlog categorized by phase (Bootstrap, Setup, Core Features).
4. **`.ai/DECISIONS.md`**:
   - Record **ONLY** explicitly validated user choices as `[ACCEPTED]`.
   - 🚨 **DO NOT** record unapproved proposals or agent hypotheses here!
5. **`.ai/ASSUMPTIONS.md`**:
   - Document all unconfirmed technical proposals, stack suggestions, or architectural assumptions awaiting user confirmation.

---

## Step 4: Present Proposal for User Validation

Present a clear, structured synthesis to the user:
1. **Executive Summary** (Project vision & target audience)
2. **Proposed Tech Stack**
3. **Core Features Breakdown (MVP vs V2)**
4. **List of Open Assumptions (`.ai/ASSUMPTIONS.md`) awaiting confirmation**

> ⚠️ **CRITICAL RULE**: Do not generate application source code or mark decisions as final until the user confirms or adjusts the proposal.

---

## Step 5: Lock Baseline & Transition to Development

Upon user approval:
1. Move validated items from `.ai/ASSUMPTIONS.md` to `.ai/DECISIONS.md` as ADRs.
2. Update `.ai/STATE.md` to reflect Phase *MVP Development*.
3. Proceed to initial project setup and component development.
