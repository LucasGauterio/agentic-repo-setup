---
name: agentic-repo-setup
description: Complete 4-pillar agentic bootstrapper for any repository. Scaffolds complete .claude documentation engine (12 design-docs skills, 12 commands, 5 core rules), Greenfield planning & implementation pipeline (plan-pipeline, plan-build, implement, implement-phase, project-plan.md, phase docs with line-anchored file links), refactoring suite (refactor-arch), test coverage frameworks, and GitFlow workflows. Generates identical master AGENTS.md, CLAUDE.md, and context.md files for universal AI Agent compatibility.
triggers:
  - /agentic-repo-setup
  - setup agentic repo
  - prepare repo for ai
  - agentic setup
---

# Agentic Repository Setup Skill (Identical Master Entrypoints Edition)

You are an expert AI software architect specializing in transforming any codebase into a fully autonomous, high-quality **AI Agentic Repository**.

> **Identical Master Entrypoints Guarantee**: When this skill runs, it generates [`AGENTS.md`](file:///AGENTS.md), [`CLAUDE.md`](file:///CLAUDE.md), and [`context.md`](file:///context.md) with **identical contents**. This ensures that Claude Code CLI, Antigravity/AGY, Cursor, Windsurf, Codex, and all AI tools receive the exact same master reference instructions, guaranteeing universal compatibility.

---

## 🏛 The 4-Pillar Execution Workflow

---

### Pillar 1: Reverse-Engineered Documentation Engine (`.claude/` Pipeline)
*Directly instantiates the `design-docs` workflow from `mba-ia-desafio-design-docs-com-ia`.*

1. **Deep Codebase Inspection (Read-Only Guarantee)**:
   - Perform a comprehensive codebase scan across all directories (`src/`, `lib/`, `services/`, `components/`, `composables/`, `locales/`, `tests/`, `configs/`).
   - Discover ALL subsystems, calculation engines, storage repositories, security layers, and UI components.
2. **Scaffold Methodological References & Rules**:
   - Copies `templates/references/` $\rightarrow$ `.claude/references/` (`architecture/`, `documentation/`, `codebase/`, `INDEX.md`).
   - Copies `templates/guidelines/` $\rightarrow$ `.claude/guidelines/` (`ai-as-maestro.md`).
   - Copies `templates/requirements/` $\rightarrow$ `.claude/requirements/` (`deliverables.default.md`).
   - Copies `templates/rules/` $\rightarrow$ `.claude/rules/` and `.agents/rules/`:
     - `source-code-is-read-only.md`, `traceability-required.md`, `no-cross-document-duplication.md`, `honor-rejected-scope.md`, `repo-file-links.md`, `restricao_escopo.md`, `gitflow_conventions.md`.
3. **Execute Reverse-Engineering Pipeline**:
   - **`design-docs-baseline`**: Generates identical [`AGENTS.md`](file:///AGENTS.md), [`CLAUDE.md`](file:///CLAUDE.md), [`context.md`](file:///context.md), and `.claude/references/codebase/`.
   - **`design-docs-prd`**: Generates `docs/PRD.md` (Product Requirements Document).
   - **`design-docs-rfc`**: Generates `docs/RFC.md` (Request For Comments / Technical Proposal).
   - **`design-docs-fdd` & `design-docs-diagrams`**: Generates `docs/FDD.md` (Functional Design Document) with **embedded C4 & Mermaid diagrams**.
   - **`design-docs-adr`**: Generates `docs/adrs/ADR-001-*.md` (Architecture Decision Records).
   - **`design-docs-tracker`**: Generates `docs/TRACKER.md` (Traceability Matrix mapping requirements to code lines `file.ext#L10-L45`).
   - **`design-docs-validate`**: Generates mechanical validation report.

---

### Pillar 2: Greenfield Planning, Implementation & Refactoring Pipeline
1. **Scaffold Greenfield Project Plan & Line-Anchored Phase Roadmap**:
   - **`docs/project-plan.md`**: Master Greenfield project plan detailing executive summary, repository structure/subprojects, and Phased Implementation Roadmap with explicit file links (`file.ext#Lnn-Lmm`).
   - **`docs/phases/`**: Scaffold sequential phase plan documents (`docs/phases/phase-01-*/phase-01-*.md` to `docs/phases/phase-NN-*/phase-NN-*.md`) detailing `## Objective`, `## Dependency Map`, `## Step Implementations (SIs)` with **exact target file links (`file.ext#Lnn-Lmm`)**, and `## Deliverables`.

2. **Scaffold Greenfield Planning & Execution Engine**:
   *Scaffolds the 23 development workflow skills from `mba-ia-greenfield-project` into `.agents/skills/` and `.claude/skills/`:*
   - **`plan-pipeline`**: Slicing implementation plan orchestrator.
   - **`plan-build`**: Architectural tech spec & SI plan builder (with templates for `api-contracts`, `auth-matrix`, `data-model`, `error-catalog`, `events-messages`, `frontend-runtime`, `traceability-matrix`, `ui-contracts`).
   - **`plan-phase`**, **`plan-context`**, **`plan-resolve`**, **`plan-rule-author`**, **`plan-test-specs`**, **`plan-validate`**, **`screen-inventory`**, **`decide`**, **`research`**.
   - **`implement` & `implement-phase`**: Step-by-step SI execution engine for turning technical specifications into tested working code without pausing model invocation.
   - **Framework Best Practices**: `nestjs-best-practices`, `next-best-practices`, `vercel-react-best-practices`, `typeorm`, `playwright-cli`.
   - **Testing Guides**: `generate-test-guide`, `testing-guide-nestjs-project`, `testing-guide-next-frontend`.

3. **Scaffold Architectural Refactoring Suite (`refactor-arch`)**:
   - Master refactoring orchestrator executing Phase 1 (Project Analysis), Phase 2 (Architecture Audit & Severity Report), Phase 3 (MVC Refactoring & Boot Validation).
   - `catalogo_antipatterns.md`, `guidelines_arquitetura.md`, `playbook_refatoracao.md`, `projeto_analise.md`, `template_relatorio.md`.

4. **Identical Root Entrypoint Generation**:
   - Read [`templates/AGENTS.md.template`](file:///templates/AGENTS.md.template) $\rightarrow$ Write **IDENTICAL MASTER CONTENTS** to [`AGENTS.md`](file:///AGENTS.md), [`CLAUDE.md`](file:///CLAUDE.md), and [`context.md`](file:///context.md).

---

### Pillar 3: Test Coverage & Quality Gate Setup
1. **Testing Infrastructure Inspection**:
   - Detect test framework (Vitest, Jest, PyTest, Go test, JUnit). Define non-watch test execution command in `AGENTS.md` / `CLAUDE.md`.
2. **Scaffold Initial Coverage**:
   - Identify untested calculation/service modules and scaffold unit test files.
3. **Quality Gates**:
   - Configure coverage thresholds in project configuration files.

---

### Pillar 4: GitFlow & Release Management Setup
1. **Git Branching Strategy**:
   - Enforce GitFlow (`main`, `dev`, `feature/*`, `bugfix/*`) via `rules/gitflow_conventions.md`.
2. **Commit & PR Conventions**:
   - Enforce Conventional Commits (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`).
   - Generate `.github/PULL_REQUEST_TEMPLATE.md` if missing.
3. **Release Automation**:
   - Document CHANGELOG generation and semantic versioning rules.

---

## 🛠 Complete `.claude` & `.agents` Artifact Tree

When `/agentic-repo-setup` finishes running on a project, the target repository will have:

```
{{PROJECT_ROOT}}/
├── AGENTS.md                         # Universal master guide (Antigravity/Cursor/Codex) — IDENTICAL TO CLAUDE.md
├── CLAUDE.md                         # Native Claude Code CLI guide — IDENTICAL TO AGENTS.md
├── context.md                        # High-level context map pointing to AGENTS.md / CLAUDE.md
├── docs/                             # Greenfield & Reverse-engineered documentation package
│   ├── project-plan.md               # Master Greenfield Project Plan & Roadmap
│   ├── PRD.md                        # Product Requirements Document
│   ├── RFC.md                        # Architecture Proposal & Trade-offs
│   ├── FDD.md                        # Functional Design Spec + Embedded Mermaid Diagrams
│   ├── TRACKER.md                    # Line-level Traceability Matrix (file.ext#Lnn)
│   ├── phases/                       # Greenfield Phased Implementation Plans
│   │   ├── phase-01-core-setup/
│   │   ├── phase-02-data-and-persistence/
│   │   ├── phase-03-domain-logic-services/
│   │   ├── phase-04-components-and-ui/
│   │   └── phase-05-i18n-and-release/
│   └── adrs/                         # Architecture Decision Records (ADR-001..ADR-NNN)
├── .claude/
│   ├── agents/                       # Greenfield plan & decision reader agents
│   ├── commands/                     # 12 design-docs-* commands
│   ├── skills/                       # 35+ skills (design-docs-*, plan-pipeline, implement, refactor-arch, etc.)
│   ├── rules/                        # 23+ rules (5 core doc rules, NestJS, Next.js, TypeORM, scope, gitflow)
│   ├── references/                   # architecture/, documentation/, codebase/ guides
│   ├── guidelines/                   # ai-as-maestro.md
│   └── requirements/                 # deliverables.default.md
└── .agents/
    ├── rules/                        # Mirrored rules
    └── skills/                       # Mirrored skills (agent invocation ready)
```
