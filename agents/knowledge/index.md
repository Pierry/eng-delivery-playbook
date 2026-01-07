# Engineering Agents Knowledge Base Index

This directory contains modular knowledge bases that support the Engineering Agents. Each file focuses on a specific domain for easier maintenance and evolution.

---

## Structure

```
agents/
├── backend.md                      # Backend Engineer Agent
├── backend-reviewer.md             # Code Review Agent
└── knowledge/
    ├── index.md                    # This file
    │
    │   # Backend Engineering
    ├── design-patterns.md          # GoF 23 + Modern patterns
    ├── engineering-principles.md   # SOLID, KISS, DRY, etc.
    ├── system-design.md            # Architecture & Big O
    ├── testing-strategies.md       # Unit, Mutation, Integration
    │
    │   # Code Review & Quality
    ├── code-review-guidelines.md   # Review process & feedback
    ├── pr-templates.md             # PR template standards
    ├── labels-conventions.md       # GitHub labels & naming
    └── cicd-quality-gates.md       # CI/CD pipeline checks
```

---

## Agent Files

### [backend.md](../backend.md)
**Senior Backend Engineer** - Handles backend development activities with expertise in:
- Languages: Java, Go, Node.js, TypeScript, Kotlin, Python
- Design patterns and system architecture
- Testing strategies and code quality

### [backend-reviewer.md](../backend-reviewer.md)
**Code Review Agent** - Enforces quality standards and review conventions:
- PR templates and standards
- Label conventions
- CI/CD quality gates
- Review comment conventions (Conventional Comments)

---

## Backend Engineering Knowledge

### [design-patterns.md](./design-patterns.md)
- All 23 Gang of Four (GoF) patterns
- Creational: Singleton, Factory Method, Abstract Factory, Builder, Prototype
- Structural: Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Proxy
- Behavioral: Chain of Responsibility, Command, Iterator, Mediator, Memento, Observer, State, Strategy, Template Method, Visitor, Interpreter
- Modern patterns: Repository, Unit of Work, CQRS, Event Sourcing, Saga

### [engineering-principles.md](./engineering-principles.md)
- SOLID principles with code examples
- KISS, DRY, YAGNI, WET
- Law of Demeter, Composition over Inheritance
- Separation of Concerns, Fail Fast
- GRASP principles
- Clean Architecture

### [system-design.md](./system-design.md)
- Big O notation and complexity analysis
- Data structure operations reference
- Sorting algorithms comparison
- Architectural patterns (Monolith, Microservices, Event-Driven, Serverless)
- Distributed systems patterns (Circuit Breaker, Saga, CQRS)
- Scalability patterns and database selection
- CAP theorem and trade-offs

### [testing-strategies.md](./testing-strategies.md)
- Unit testing principles and frameworks
- Test doubles (Mocks, Stubs, Spies, Fakes)
- Mutation testing with tools per language
- Integration testing with Test Containers
- Contract testing (Pact)
- Performance testing (k6)

---

## Code Review & Quality Knowledge

### [code-review-guidelines.md](./code-review-guidelines.md)
- Review philosophy and principles
- Conventional Comments system (labels and formatting)
- Review checklist (correctness, security, performance, etc.)
- Review process workflow
- Feedback techniques and templates

### [pr-templates.md](./pr-templates.md)
- Standard PR template
- Specialized templates: Bug fix, Feature, Refactor, Migration, Hotfix
- Template best practices
- GitHub template setup instructions

### [labels-conventions.md](./labels-conventions.md)
- Label categories: Type, Priority, Size, Status, Review
- Color conventions and naming
- Automation setup (GitHub Actions, labeler)
- Label sync across repositories

### [cicd-quality-gates.md](./cicd-quality-gates.md)
- Build gates
- Testing gates (unit, integration, E2E)
- Code quality gates (lint, type check, SonarQube)
- Security gates (SAST, dependency scan, secrets)
- Performance and documentation gates
- Branch protection configuration

---

## Maintenance Guidelines

### Adding New Knowledge
1. Identify the appropriate category file
2. Add content following existing format
3. Include code examples in multiple languages where applicable
4. Update this index if adding new files

### Code Examples
- Java: Primary enterprise language
- Go: Systems and cloud-native
- TypeScript/JavaScript: Node.js ecosystem
- Kotlin: Modern JVM alternative
- Python: Scripting and data

### Version Control
- Keep commits atomic (one concept per commit)
- Document significant changes
- Review for accuracy periodically

---

## Usage Guide

### For Backend Development
1. Reference `backend.md` for identity and behavior
2. Use `design-patterns.md` for pattern implementation
3. Use `engineering-principles.md` for best practices
4. Use `testing-strategies.md` for test implementation

### For Code Reviews
1. Reference `backend-reviewer.md` for review standards
2. Use `code-review-guidelines.md` for comment conventions
3. Use `pr-templates.md` for PR structure
4. Use `cicd-quality-gates.md` for pipeline requirements

### Cross-Referencing
Agents can reference each other's knowledge:
- Backend agent follows reviewer's conventions when creating PRs
- Reviewer uses backend knowledge to assess code quality
