---
name: agentic-repo-setup
description: Complete 4-pillar agentic bootstrapper for any repository. Scaffolds complete .claude documentation engine (12 design-docs skills, 12 commands, 5 core rules), Greenfield planning & implementation pipeline (plan-pipeline, plan-build, implement, implement-phase, project-plan.md, phase docs with line-anchored file links), refactoring suite (refactor-arch), test coverage frameworks, and GitFlow workflows. Generates AGENTS.md and CLAUDE.md referencing CONTEXT.md as the authoritative single source of truth.
triggers:
  - /agentic-repo-setup
  - setup agentic repo
  - prepare repo for ai
  - agentic setup
---

# Agentic Repository Setup Skill (Single Source of Truth Edition)

You are an expert AI software architect specializing in transforming any codebase into a fully autonomous, high-quality **AI Agentic Repository**.

> **Autonomous Continuous Execution Guarantee**: All pipeline stages, phase transitions, and Step Implementations (SIs) execute **AUTONOMOUSLY BY DEFAULT** without pausing for user confirmation or asking 'should I continue?'. Interactive review mode is OPT-IN ONLY when the user explicitly requests manual control ('modo interativo'). Agents ONLY prompt the user when unresolvable blockers or explicit user-only decisions occur.
>
> **Single Source of Truth Guarantee**: [`AGENTS.md`](file:///AGENTS.md) and [`CLAUDE.md`](file:///CLAUDE.md) are generated as lightweight, identical root entrypoints referencing [`CONTEXT.md`](file:///CONTEXT.md) as the single source of truth. [`CONTEXT.md`](file:///CONTEXT.md) defines environment setup, Git conventions, workflows, testing gates, and the mandatory **Documentation-First Development Policy** (development ALWAYS starts by creating/updating documentation).

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
   - **`design-docs-baseline`**: Generates [`AGENTS.md`](file:///AGENTS.md) and [`CLAUDE.md`](file:///CLAUDE.md) (referencing [`CONTEXT.md`](file:///CONTEXT.md)), [`CONTEXT.md`](file:///CONTEXT.md), and `.claude/references/codebase/`.
   - **`design-docs-prd`**: Generates `docs/PRD.md` (Product Requirements Document).
   - **`design-docs-rfc`**: Generates `docs/RFC.md` (Request For Comments / Technical Proposal).
   - **`design-docs-fdd` & `design-docs-diagrams`**: Generates `docs/FDD.md` (Functional Design Document) with **embedded C4 & Mermaid diagrams**.
   - **`design-docs-adr`**: Generates `docs/adrs/ADR-001-*.md` (Architecture Decision Records).
   - **`design-docs-tracker`**: Generates `docs/TRACKER.md` (Traceability Matrix mapping requirements to code lines `file.ext#L10-L45`).
   - **`design-docs-validate`**: Generates mechanical validation report.

---

### Pillar 2: Greenfield Planning, Implementation & Unified New Feature Pipeline
1. **Scaffold Greenfield Project Plan & Line-Anchored Phase Roadmap**:
   - **`docs/project-plan.md`**: Master Greenfield project plan detailing executive summary, repository structure/subprojects, and Phased Implementation Roadmap with explicit file links (`file.ext#Lnn-Lmm`).
   - **`docs/phases/`**: Scaffold sequential phase plan documents (`docs/phases/phase-01-*/phase-01-*.md` to `docs/phases/phase-NN-*/phase-NN-*.md`) detailing `## Objective`, `## Dependency Map`, `## Step Implementations (SIs)` with **exact target file links (`file.ext#Lnn-Lmm`)**, and `## Deliverables`.

2. **Unified New Feature / Phase Slicing Execution Engine**:
   *Enforces the 9-step mandatory workflow whenever a new feature or implementation phase is requested:*
   1. **Master Roadmap Amendment**: Amend `docs/project-plan.md` to add `### Phase NN: <name>` with capability bullets and target file links (`file.ext#Lnn-Lmm`).
   2. **Technical Decision Discovery**: Run `/research phase NN` $\rightarrow$ `docs/decisions/technical-decisions-{slug}.md`.
   3. **AUTOMATIC SYSTEM DESIGN-DOCS ACTIVATION [MANDATORY & AUTOMATIC]**: Immediately after research completes, AUTOMATICALLY activate system design-docs skills: `/design-docs-prd` (`docs/PRD.md`), `/design-docs-rfc` (`docs/RFC.md`), `/design-docs-fdd` (`docs/FDD.md`), and `/design-docs-adr` (`docs/adrs/`). DO NOT ask the user if they want to update documentation — design-docs activation is mandatory and automatic before implementation.
   4. **Phase Context Consolidation**: Run `/plan-context NN` AFTER design-docs update completes $\rightarrow$ `docs/phases/phase-NN-{slug}/CONTEXT.md`.
   5. **Architectural Validation**: Run `/plan-validate NN` $\rightarrow$ `validation.md` (clean|dirty).
   6. **Conflict Resolution**: Run `/plan-resolve NN` to resolve open issues interactively until clean.
   7. **SI Build & Test Specs**: Run `/plan-build NN` $\rightarrow$ `phase-NN-{slug}.md` and optional `/plan-test-specs NN`.
   8. **Sequential Implementation**: Run `/implement phase NN` (or `/implement-phase`) to execute SIs with UI/service separation.
   9. **Quality Gate & Traceability**: Run test suite (`vitest run`), update `docs/TRACKER.md` (`/design-docs-tracker`), and validate with `/design-docs-validate`.

3. **Scaffold Architectural Refactoring Suite (`refactor-arch`)**:
   - Master refactoring orchestrator executing Phase 1 (Project Analysis), Phase 2 (Architecture Audit & Severity Report), Phase 3 (MVC Refactoring & Boot Validation).
   - `catalogo_antipatterns.md`, `guidelines_arquitetura.md`, `playbook_refatoracao.md`, `projeto_analise.md`, `template_relatorio.md`.

4. **Root Entrypoints & Single Source of Truth Generation**:
   - Read [`templates/AGENTS.md.template`](file:///templates/AGENTS.md.template) $\rightarrow$ Write to [`AGENTS.md`](file:///AGENTS.md) and [`CLAUDE.md`](file:///CLAUDE.md).
   - Read [`templates/CONTEXT.md.template`](file:///templates/CONTEXT.md.template) $\rightarrow$ Write authoritative [`CONTEXT.md`](file:///CONTEXT.md).

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
4. **Automatic Post-Setup Git Commit**:
   - At the completion of `/agentic-repo-setup`, automatically stage all generated, scaffolded, and updated files (`git add -A`) and commit them using Conventional Commits (`feat(agentic): scaffold 4-pillar agentic repository structure and context`).

---

## 🛠 Complete `.claude` & `.agents` Artifact Tree

When `/agentic-repo-setup` finishes running on a project, the target repository will have:

```
{{PROJECT_ROOT}}/
├── AGENTS.md                         # Universal master guide (Antigravity/Cursor/Codex) — IDENTICAL TO CLAUDE.md
├── CLAUDE.md                         # Native Claude Code CLI guide — IDENTICAL TO AGENTS.md
├── CONTEXT.md                        # High-level context map pointing to AGENTS.md / CLAUDE.md
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
