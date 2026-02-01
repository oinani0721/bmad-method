# BMad Method

Agile AI-driven planning and development methodology for Claude Code and AI-assisted IDEs.

## Overview

BMad (Business-Minded Agile Development) is a structured methodology for AI-assisted software development that combines agile principles with AI agent orchestration.

## Features

### 12 Specialized Agents

| Agent | Role |
|-------|------|
| **PM** | Project Manager - PRD creation and planning |
| **PO** | Product Owner - Story validation and prioritization |
| **Architect** | Technical architecture and ADR decisions |
| **Dev** | Development implementation |
| **QA** | Quality assurance and testing |
| **SM** | Scrum Master - Sprint coordination |
| **Analyst** | Research and analysis |
| **UX Expert** | User experience design |
| **BMad Master** | Methodology orchestration |
| **BMad Orchestrator** | Workflow automation |
| **Iteration Validator** | Quality gate validation |
| **Parallel Dev** | Parallel development coordination |

### 49 Task Templates

Standardized workflows for common development tasks including:
- Story creation and validation
- Epic development
- Architecture decisions (ADR)
- Behavior specifications
- Quality gates
- Documentation

### 21 Document Templates

- PRD (Product Requirements Document)
- Architecture documents
- Story templates (v3 enhanced)
- ADR templates
- QA gate reports
- And more...

### 6 Workflow Templates

| Workflow | Use Case |
|----------|----------|
| `greenfield-fullstack.yaml` | New full-stack projects |
| `greenfield-service.yaml` | New backend services |
| `greenfield-ui.yaml` | New frontend applications |
| `brownfield-fullstack.yaml` | Existing full-stack projects |
| `brownfield-service.yaml` | Existing backend services |
| `brownfield-ui.yaml` | Existing frontend applications |

### 12 Quality Checklists

- Architect checklist
- Code review checklist
- Story Definition of Done (DoD)
- SDD verification
- And more...

## Installation

### For Claude Code Projects

1. Copy the contents to your project's `.bmad-core/` directory:

```bash
git clone https://github.com/oinani0721/bmad-method.git
cp -r bmad-method/* your-project/.bmad-core/
```

2. Create your project configuration:

```bash
cd your-project/.bmad-core
cp core-config.yaml.example core-config.yaml
# Edit core-config.yaml for your project
```

3. Reference in your CLAUDE.md:

```markdown
## BMad Integration
See `.bmad-core/` for methodology configuration.
```

## Quick Start

### Invoking Agents

Use slash commands in Claude Code:

```
/pm        - Start project planning
/architect - Design technical architecture
/dev       - Begin development
/qa        - Run quality checks
```

### Running Tasks

```
/create-next-story  - Create a new user story
/qa-gate           - Run quality gate validation
/correct-course    - Handle scope changes
```

## Documentation

- [User Guide](user-guide.md) - Complete methodology guide
- [Brownfield Projects](working-in-the-brownfield.md) - Working with existing codebases
- [IDE Workflow](enhanced-ide-development-workflow.md) - Development workflow details

## Directory Structure

```
bmad-method/
├── agent-teams/          # Pre-configured team setups
├── checklists/           # Quality verification checklists
├── data/                 # Knowledge base and reference data
├── decisions/            # Decision frameworks
├── schemas/              # Data validation schemas
├── tasks/                # Reusable task definitions
├── templates/            # Document templates
├── utils/                # Utility documentation
├── validators/           # Validation rules
├── workflows/            # End-to-end workflow templates
├── core-config.yaml.example  # Example configuration
└── user-guide.md         # Main documentation
```

## 4-Phase Workflow

BMad follows a structured 4-phase approach:

1. **Phase 1: Analysis** - Requirements gathering and research
2. **Phase 2: Planning** - Story creation and prioritization
3. **Phase 3: Solutioning** - Architecture and design decisions
4. **Phase 4: Implementation** - Development and quality assurance

## License

MIT License - see [LICENSE](LICENSE)

## Contributing

Contributions welcome! Please read the contributing guidelines before submitting PRs.

## Author

[@oinani0721](https://github.com/oinani0721)

## Acknowledgments

Based on the BMad methodology for AI-assisted software development.
