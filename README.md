# Viso AI Development Workspace

This is the central workspace designed for AI-assisted development across multiple source code repositories. It provides the tooling, standards, and structured workflows necessary to build, plan, and review code using AI agents.

## Getting Started

1. Clone this workspace repository.
2. Ensure you have the required AI Agent integrations (such as OpenCode or Claude) configured.
3. Your agent automatically has access to the specialized `speckit` skills defined in `.agents/skills`.

## Recommended Workflow

To ensure high-quality and consistent outputs, we recommend using the `speckit` tools in the following sequence:

### Setup Phase
Run these initially to configure your project context:
1. **Constitution** (`speckit-constitution`): Establish core project principles and templates.
2. **Brownfield Scan** (`speckit-brownfield-scan`): Auto-discover project structure, frameworks, and architecture.

### Development Phase
Run these sequentially for any new feature or fix:
1. **Specify** (`speckit-specify`): Generate a feature specification (`spec.md`).
2. **Clarify** (`speckit-clarify`): Identify and resolve any underspecified areas in the spec.
3. **Plan** (`speckit-plan`): Generate a technical implementation blueprint (`plan.md`).
4. **Tasks** (`speckit-tasks`): Break the plan into an actionable `tasks.md` checklist.
5. **Blueprint Generate** (`speckit-blueprint-generate`): Scaffold required files based on the specs.
6. **Implement** (`speckit-implement`): Execute the codebase changes systematically.
7. **Review** (`speckit-review-run`): Perform an automated code quality review.
8. **Commit** (`speckit-git-commit`): Auto-commit your verified changes.

---
*For behavioral rules governing AI agents in this workspace, refer to `AGENTS.md` / `CLAUDE.md`.*
