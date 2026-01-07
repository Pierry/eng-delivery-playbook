# Engineering Delivery Playbook

A comprehensive collection of AI-powered engineering agents and knowledge bases designed to standardize and elevate software engineering practices across teams.

## Overview

This playbook provides structured guidelines, best practices, and reusable knowledge for backend engineering and code review processes. It's designed to be used as a reference for AI agents, development teams, and individual engineers seeking to maintain high-quality standards.

## Purpose

- **Standardize Engineering Practices**: Establish consistent patterns across teams
- **Accelerate Onboarding**: New team members can quickly learn established conventions
- **Enable AI Assistance**: Provide context for AI agents to give accurate, consistent guidance
- **Reduce Cognitive Load**: Pre-defined templates, checklists, and conventions reduce decision fatigue
- **Improve Code Quality**: Systematic review processes catch issues early

## Structure

```
eng-delivery-playbook/
├── README.md                         # This file
└── agents/
    ├── backend.md                    # Backend Engineer Agent
    ├── backend-reviewer.md           # Code Review Agent
    └── knowledge/
        ├── index.md                  # Knowledge base navigation
        │
        │   # Backend Engineering
        ├── design-patterns.md        # GoF 23 + Modern patterns
        ├── engineering-principles.md # SOLID, KISS, DRY, GRASP
        ├── system-design.md          # Architecture & Big O
        ├── testing-strategies.md     # Unit, Mutation, Integration
        │
        │   # Code Review & Quality
        ├── code-review-guidelines.md # Review process & feedback
        ├── pr-templates.md           # Pull request templates
        ├── labels-conventions.md     # GitHub labels system
        └── cicd-quality-gates.md     # CI/CD pipeline checks
```

## Agents

### Backend Engineer Agent (`agents/backend.md`)

A senior backend engineer persona with deep expertise in:

| Area | Coverage |
|------|----------|
| **Languages** | Java, Go, Node.js, TypeScript, Kotlin, Python |
| **Patterns** | All 23 GoF design patterns + modern patterns |
| **Principles** | SOLID, KISS, DRY, YAGNI, GRASP, Clean Architecture |
| **System Design** | Microservices, Event-Driven, Serverless, Distributed Systems |
| **Testing** | Unit, Integration, Mutation, Contract, Performance |
| **Complexity** | Big O analysis, data structures, algorithms |

### Backend Reviewer Agent (`agents/backend-reviewer.md`)

A code review specialist focused on maintaining quality standards:

| Area | Coverage |
|------|----------|
| **Comment Conventions** | Conventional Comments (blocker, issue, suggestion, nit) |
| **PR Standards** | Templates, size limits, required sections |
| **Labels** | Type, Priority, Size, Status, Review categories |
| **CI/CD Gates** | Build, Test, Security, Coverage thresholds |
| **Checklists** | Security, Performance, Architecture, Testing |

## Knowledge Base

### Backend Engineering

#### Design Patterns (`knowledge/design-patterns.md`)
- **Creational**: Singleton, Factory Method, Abstract Factory, Builder, Prototype
- **Structural**: Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Proxy
- **Behavioral**: Chain of Responsibility, Command, Iterator, Mediator, Memento, Observer, State, Strategy, Template Method, Visitor, Interpreter
- **Modern**: Repository, Unit of Work, CQRS, Event Sourcing, Saga, Circuit Breaker

#### Engineering Principles (`knowledge/engineering-principles.md`)
- SOLID principles with detailed code examples
- KISS, DRY, YAGNI, WET explained with practical guidance
- Law of Demeter, Composition over Inheritance
- GRASP principles for responsibility assignment
- Clean Architecture layers and dependencies

#### System Design (`knowledge/system-design.md`)
- Big O complexity reference tables
- Data structure operations cheat sheet
- Architectural patterns comparison (Monolith vs Microservices vs Serverless)
- Distributed systems patterns (Circuit Breaker, Saga, CQRS)
- CAP theorem and database selection guide
- Scalability patterns and caching strategies

#### Testing Strategies (`knowledge/testing-strategies.md`)
- Testing pyramid and philosophy
- Unit testing with AAA pattern and frameworks per language
- Mutation testing concepts and tools (PIT, Stryker, mutmut)
- Integration testing with Test Containers
- Contract testing with Pact
- Performance testing with k6

### Code Review & Quality

#### Code Review Guidelines (`knowledge/code-review-guidelines.md`)
- Conventional Comments system with label prefixes
- Review checklist (correctness, security, performance, architecture)
- Feedback techniques and anti-patterns
- Response templates for common scenarios

#### PR Templates (`knowledge/pr-templates.md`)
- Standard PR template with all required sections
- Specialized templates: Bug Fix, Feature, Refactor, Migration, Hotfix
- GitHub template setup instructions

#### Labels Conventions (`knowledge/labels-conventions.md`)
- Complete label taxonomy with colors
- Categories: Type, Priority, Size, Status, Review
- Automation setup with GitHub Actions
- Label sync across repositories

#### CI/CD Quality Gates (`knowledge/cicd-quality-gates.md`)
- Build, lint, and type check gates
- Testing gates (unit, integration, E2E)
- Security gates (SAST, dependency scan, secrets detection)
- Quality metrics (SonarQube integration)
- Branch protection configuration
- Complete GitHub Actions pipeline example

## Usage

### For AI Agents
Reference the agent files to establish persona and behavioral guidelines:
```
You are a Senior Backend Engineer. Follow the guidelines in agents/backend.md...
```

### For Development Teams
1. Copy relevant templates to your repository's `.github/` directory
2. Configure labels using the provided color scheme
3. Set up CI/CD quality gates in your pipeline
4. Reference checklists during code reviews

### For Individual Engineers
- Use as a learning resource for design patterns and principles
- Reference during code reviews
- Consult for architecture decisions

## Key Standards

| Standard | Threshold |
|----------|-----------|
| PR Size | < 400 lines (soft limit) |
| Code Coverage | >= 80% (new code) |
| Review Response | < 4 hours |
| Security Scan | No critical/high vulnerabilities |
| Build Time | < 5 minutes |

## Contributing

1. Follow the existing structure and formatting
2. Include code examples in multiple languages where applicable
3. Update the index when adding new files
4. Keep content practical and actionable

## License

MIT License - Feel free to use and adapt for your organization.

---

**Built with expertise from industry best practices and modern engineering standards.**
