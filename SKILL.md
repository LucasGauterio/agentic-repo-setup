---
name: agentic-repo-setup
description: Complete 4-pillar agentic bootstrapper for any repository. Scaffolds complete .claude documentation engine (12 design-docs skills, 12 commands, 5 core rules), Greenfield planning & implementation pipeline (plan-pipeline, plan-build, implement, implement-phase), refactoring suite (refactor-arch), test coverage frameworks, and GitFlow workflows. Configured specifically for AI Agent execution without disable-model-invocation restrictions.
triggers:
  - /agentic-repo-setup
  - setup agentic repo
  - prepare repo for ai
  - agentic setup
---

# Agentic Repository Setup Skill (Full Greenfield & Refactoring Edition)

You are an expert AI software architect specializing in transforming any codebase into a fully autonomous, high-quality **AI Agentic Repository**.

> **Direct MBA Reference Standards**:
> - **Documentation Engine**: Instantiates the full `.claude` system from [`mba-ia-desafio-design-docs-com-ia`](file:///G:/Projects/MBA/mba-ia-desafio-design-docs-com-ia/DESIGN_DOCS_PROCESS.md) (12 design-docs skills, 12 commands, 5 core documentation rules, reference guides).
> - **Greenfield Planning & Implementation Pipeline**: Instantiates the complete development workflow from [`mba-ia-greenfield-project`](file:///G:/Projects/MBA/mba-ia-greenfield-project/CLAUDE.md) (`plan-pipeline`, `plan-build`, `plan-phase`, `implement`, `implement-phase`, `nestjs-best-practices`, `next-best-practices`, `vercel-react-best-practices`, `typeorm`).
> - **Refactoring Suite**: Instantiates the complete `refactor-arch` package from [`mba-ia-refactor-projects-skill`](file:///G:/Projects/MBA/mba-ia-refactor-projects-skill/DESAFIO_README.md) (`catalogo_antipatterns.md`, `guidelines_arquitetura.md`, `playbook_refatoracao.md`, `projeto_analise.md`, `template_relatorio.md`).
> - **AI Agent Invocation Ready**: All skills are configured with `disable-model-invocation: true` removed so that AI Agents (Antigravity, Claude Code, Cursor, Codex) can invoke and execute them directly and autonomously.

---

## 🏛 The 4-Pillar Execution Workflow

---

### Pillar 1: Reverse-Engineered Documentation Engine (`.claude/` Pipeline)
*Directly instantiates the `design-docs` workflow from `mba-ia-desafio-design-docs-com-ia`.*

1. **Scaffold Methodological References & Rules**:
   - Copies `templates/references/` $\rightarrow$ `.claude/references/` (`architecture/`, `documentation/`, `codebase/`, `INDEX.md`).
   - Copies `templates/guidelines/` $\rightarrow$ `.claude/guidelines/` (`ai-as-maestro.md`).
   - Copies `templates/requirements/` $\rightarrow$ `.claude/requirements/` (`deliverables.default.md`).
   - Copies `templates/rules/` $\rightarrow$ `.claude/rules/` and `.agents/rules/`:
     - `source-code-is-read-only.md`, `traceability-required.md`, `no-cross-document-duplication.md`, `honor-rejected-scope.md`, `repo-file-links.md`, `restricao_escopo.md`, `gitflow_conventions.md`.

2. **Scaffold Documentation Commands & Skills**:
   - Copies `templates/commands/` $\rightarrow$ `.claude/commands/` (all 12 `design-docs-*` commands).
   - Copies `templates/skills/` $\rightarrow$ `.claude/skills/` and `.agents/skills/`.

3. **Execute Reverse-Engineering Pipeline**:
   - **`design-docs-baseline`**: Generates `CLAUDE.md`, `context.md`, and `.claude/references/codebase/`.
   - **`design-docs-prd`**: Generates `docs/PRD.md` (Product Requirements Document).
   - **`design-docs-rfc`**: Generates `docs/RFC.md` (Request For Comments / Technical Proposal).
   - **`design-docs-fdd` & `design-docs-diagrams`**: Generates `docs/FDD.md` (Functional Design Document) with **embedded C4 & Mermaid diagrams**.
   - **`design-docs-adr`**: Generates `docs/adrs/ADR-001-*.md` (Architecture Decision Records).
   - **`design-docs-tracker`**: Generates `docs/TRACKER.md` (Traceability Matrix mapping requirements to code lines `file.ext#L10-L45`).
   - **`design-docs-validate`**: Generates mechanical validation report.

---

### Pillar 2: Greenfield Planning, Implementation & Refactoring Pipeline
1. **Scaffold Greenfield Planning & Execution Engine**:
   *Scaffolds the 23 development workflow skills from `mba-ia-greenfield-project` into `.agents/skills/` and `.claude/skills/`:*
   - **`plan-pipeline`**: Slicing implementation plan orchestrator.
   - **`plan-build`**: Architectural tech spec & SI plan builder (with templates for `api-contracts`, `auth-matrix`, `data-model`, `error-catalog`, `events-messages`, `frontend-runtime`, `traceability-matrix`, `ui-contracts`).
   - **`plan-phase`**, **`plan-context`**, **`plan-resolve`**, **`plan-rule-author`**, **`plan-test-specs`**, **`plan-validate`**, **`screen-inventory`**, **`decide`**, **`research`**.
   - **`implement` & `implement-phase`**: Step-by-step SI execution engine for turning technical specifications into tested working code without pausing model invocation.
   - **Framework Best Practices**: `nestjs-best-practices` (40+ NestJS rules), `next-best-practices` (20+ Next.js rules), `vercel-react-best-practices` (70+ React rendering rules), `typeorm` (15+ TypeORM rules), `playwright-cli`.
   - **Testing Guides**: `generate-test-guide`, `testing-guide-nestjs-project`, `testing-guide-next-frontend`.

2. **Scaffold Architectural Refactoring Suite (`refactor-arch`)**:
   - Master refactoring orchestrator executing Phase 1 (Project Analysis), Phase 2 (Architecture Audit & Severity Report), Phase 3 (MVC Refactoring & Boot Validation).
   - `catalogo_antipatterns.md`, `guidelines_arquitetura.md`, `playbook_refatoracao.md`, `projeto_analise.md`, `template_relatorio.md`.

3. **Root Entrypoint Generation**:
   - Read [`templates/AGENTS.md.template`](file:///templates/AGENTS.md.template) $\rightarrow$ [`AGENTS.md`](file:///AGENTS.md).
   - Read [`templates/CLAUDE.md.template`](file:///templates/CLAUDE.md.template) $\rightarrow$ [`CLAUDE.md`](file:///CLAUDE.md).

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
├── AGENTS.md                         # Universal master guide (Antigravity/Cursor/Codex)
├── CLAUDE.md                         # Native Claude Code CLI guide
├── context.md                        # High-level context map
├── docs/                             # Reverse-engineered documentation package
│   ├── PRD.md                        # Product Requirements Document
│   ├── RFC.md                        # Architecture Proposal & Trade-offs
│   ├── FDD.md                        # Functional Design Spec + Embedded Mermaid Diagrams
│   ├── TRACKER.md                    # Line-level Traceability Matrix (file.ext#Lnn)
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
