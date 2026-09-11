---
name: agentic-repo-setup
description: Complete 4-pillar agentic bootstrapper for any repository. Scaffolds complete .claude documentation engine (12 design-docs skills, 12 commands, 5 core rules, references, guidelines, requirements), refactoring suite (refactor-arch, antipattern catalog, severity audit, MVC playbook), test coverage frameworks, and GitFlow workflows. Built from mba-ia-desafio-design-docs-com-ia & mba-ia-refactor-projects-skill.
triggers:
  - /agentic-repo-setup
  - setup agentic repo
  - prepare repo for ai
  - agentic setup
---

# Agentic Repository Setup Skill (Full Architectural Refactoring Edition)

You are an expert AI software architect specializing in transforming any codebase into a fully autonomous, high-quality **AI Agentic Repository**.

> **Direct MBA Reference Standards**:
> - **Documentation Engine**: Instantiates the full `.claude` system from [`mba-ia-desafio-design-docs-com-ia`](file:///G:/Projects/MBA/mba-ia-desafio-design-docs-com-ia/DESIGN_DOCS_PROCESS.md) (12 design-docs skills, 12 commands, 5 core documentation rules, reference guides).
> - **Refactoring Suite**: Instantiates the complete `refactor-arch` package from [`mba-ia-refactor-projects-skill`](file:///G:/Projects/MBA/mba-ia-refactor-projects-skill/DESAFIO_README.md) (`catalogo_antipatterns.md`, `guidelines_arquitetura.md`, `playbook_refatoracao.md`, `projeto_analise.md`, `template_relatorio.md`).

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
     - `source-code-is-read-only.md` (Guarantees zero code mutations during documentation generation)
     - `traceability-required.md` (Requires every requirement/decision to map to real code in `TRACKER.md`)
     - `no-cross-document-duplication.md` (Enforces strict document taxonomy)
     - `honor-rejected-scope.md` (Prevents rejected/deferred items from becoming requirements)
     - `repo-file-links.md` (Formats file references with line anchors `#Lnn`)
     - `restricao_escopo.md` (Workspace scope boundary)
     - `gitflow_conventions.md` (GitFlow branching & commit rules)

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

### Pillar 2: Architectural Refactoring & Agent Setup
1. **Scaffold Architectural Refactoring Suite (`refactor-arch`)**:
   *Scaffolds the 6-file refactoring package from `mba-ia-refactor-projects-skill` into `.agents/skills/refactor-arch/` and `.claude/skills/refactor-arch/`:*
   - **`SKILL.md`**: Master refactoring orchestrator executing Phase 1 (Project Analysis), Phase 2 (Architecture Audit & Severity Report), Phase 3 (MVC Refactoring & Boot Validation).
   - **`catalogo_antipatterns.md`**: Severity classification catalog (CRITICAL, HIGH, MEDIUM, LOW) for MVC & SOLID violations (God Classes, hardcoded credentials, SQL injection, tight coupling, N+1 queries, magic numbers).
   - **`guidelines_arquitetura.md`**: Architectural guidelines for MVC layered separation (Controllers, Services, Models/Repositories, DTOs).
   - **`playbook_refatoracao.md`**: Step-by-step refactoring playbook for dependency extraction and boot verification.
   - **`projeto_analise.md`**: Technology-agnostic stack and file analysis rules.
   - **`template_relatorio.md`**: Audit report template.

2. **Root Entrypoint Generation**:
   - Read [`templates/AGENTS.md.template`](file:///templates/AGENTS.md.template) $\rightarrow$ [`AGENTS.md`](file:///AGENTS.md).
   - Read [`templates/CLAUDE.md.template`](file:///templates/CLAUDE.md.template) $\rightarrow$ [`CLAUDE.md`](file:///CLAUDE.md).

3. **Workflow Skills**:
   - `add-feature` (5-step feature development workflow).
   - `code-reviewer` (Code review for style, security, and test coverage).

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
├── docs/
│   ├── PRD.md                        # Product Requirements Document
│   ├── RFC.md                        # Architecture Proposal & Trade-offs
│   ├── FDD.md                        # Functional Design Spec + Embedded Mermaid Diagrams
│   ├── TRACKER.md                    # Line-level Traceability Matrix (file.ext#Lnn)
│   └── adrs/                         # Architecture Decision Records
│       ├── ADR-001-*.md
│       └── README.md
├── .claude/
│   ├── commands/                     # 12 design-docs-* commands
│   ├── skills/                       # 12 design-docs-* skills + refactor-arch + add-feature
│   ├── rules/                        # 5 core doc rules + scope + gitflow rules
│   ├── references/                   # architecture/, documentation/, codebase/ guides
│   ├── guidelines/                   # ai-as-maestro.md
│   └── requirements/                 # deliverables.default.md
└── .agents/
    ├── rules/                        # Mirrored rules
    └── skills/
        ├── refactor-arch/            # 6-file Refactoring Suite
        │   ├── SKILL.md
        │   ├── catalogo_antipatterns.md
        │   ├── guidelines_arquitetura.md
        │   ├── playbook_refatoracao.md
        │   ├── projeto_analise.md
        │   └── template_relatorio.md
        └── add-feature/              # Workflow skill
```
