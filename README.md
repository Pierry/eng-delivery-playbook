# Engineering Delivery Playbook

A comprehensive collection of AI-powered engineering agents and knowledge bases designed to standardize and elevate software engineering practices across teams.

---

## The Philosophy: Context-Driven AI Usage

<p align="center">
  <img src="context-vs-onboarding.png" alt="Context vs Onboarding - AI Usage Model" width="600">
</p>

**AI effectiveness scales with business context.** The more you understand the "why" behind the code, the better you can leverage AI for the "how".

| Stage | Days | Context | AI Role |
|-------|------|---------|---------|
| **Onboarding** | 0-30 | Low | Learning assistant - explore, ask questions |
| **Ramping** | 30-60 | Medium | Pair programmer - implement with supervision |
| **Contributing** | 60-90 | High | Accelerator - complex tasks, light review |
| **Established** | 90+ | Expert | Force multiplier - full leverage |

```
Without Context: AI generates → Code that "works" → Tech debt
With Context:    Human guides → AI generates → Value delivered
```

---

## Quick Navigation

### [Agents](agents/)

AI agent definitions with expertise and behavioral guidelines.

#### Backend
| Agent | Description | Link |
|-------|-------------|------|
| **Backend Engineer** | Java, Go, Node, Python, Kotlin. Design patterns, SOLID, system design. | [View](agents/backend.md) |
| **Backend Reviewer** | PR standards, Conventional Comments, CI/CD quality gates. | [View](agents/backend-reviewer.md) |

#### Frontend
| Agent | Description | Link |
|-------|-------------|------|
| **Frontend Engineer** | React, Vue.js, TypeScript, Next.js, Nuxt. State management, a11y. | [View](agents/frontend.md) |
| **Frontend Reviewer** | Accessibility, Core Web Vitals, UX, security (XSS). | [View](agents/frontend-reviewer.md) |

#### Mobile
| Agent | Description | Link |
|-------|-------------|------|
| **Mobile Engineer** | Flutter, Android (Kotlin), iOS (Swift). MVVM, Clean Architecture. | [View](agents/mobile.md) |
| **Mobile Reviewer** | Platform guidelines, performance, accessibility. | [View](agents/mobile-reviewer.md) |

### [Knowledge Base](agents/knowledge/)

Reference materials for engineering best practices.

| Topic | Description | Link |
|-------|-------------|------|
| **Design Patterns** | GoF 23 + modern patterns (CQRS, Saga, Event Sourcing) | [View](agents/knowledge/design-patterns.md) |
| **Engineering Principles** | SOLID, KISS, DRY, YAGNI, GRASP, Clean Architecture | [View](agents/knowledge/engineering-principles.md) |
| **System Design** | Big O, architectures, distributed systems, CAP theorem | [View](agents/knowledge/system-design.md) |
| **Testing Strategies** | Unit, mutation, integration testing by language | [View](agents/knowledge/testing-strategies.md) |
| **Frontend Development** | React/Vue patterns, state management, performance | [View](agents/knowledge/frontend-development.md) |
| **Mobile Development** | Flutter/Android/iOS patterns, MVVM, MVI | [View](agents/knowledge/mobile-development.md) |
| **Code Review Guidelines** | Conventional Comments, checklists, feedback | [View](agents/knowledge/code-review-guidelines.md) |
| **PR Templates** | Standard, bug fix, feature, refactor, hotfix | [View](agents/knowledge/pr-templates.md) |
| **Labels Conventions** | GitHub label taxonomy with colors | [View](agents/knowledge/labels-conventions.md) |
| **CI/CD Quality Gates** | Pipeline checks, branch protection, SonarQube | [View](agents/knowledge/cicd-quality-gates.md) |

### [Resources](resources/)

Curated learning materials for AI-assisted development.

| Category | Description | Link |
|----------|-------------|------|
| **Newsletters** | THE CODE, Every, JP, Joe Njenga | [View](resources/#newsletters) |
| **Courses** | Claude Code structured learning paths | [View](resources/#long-courses) |
| **GitHub Repos** | Cheat sheets, templates, awesome lists | [View](resources/#github-repositories) |
| **YouTube** | Setup guides, workflows, tutorials | [View](resources/#youtube-tutorials) |
| **Creators** | Industry experts to follow | [View](resources/#creators-to-follow) |

---

## Project Structure

```
eng-delivery-playbook/
├── README.md                    # You are here
├── context-vs-onboarding.png    # AI usage philosophy
│
├── agents/                      # AI Agent Definitions
│   ├── README.md                # Agents overview
│   │
│   │   # Backend
│   ├── backend.md               # Backend Engineer
│   ├── backend-reviewer.md      # Backend Reviewer
│   │
│   │   # Frontend
│   ├── frontend.md              # Frontend Engineer
│   ├── frontend-reviewer.md     # Frontend Reviewer
│   │
│   │   # Mobile
│   ├── mobile.md                # Mobile Engineer
│   ├── mobile-reviewer.md       # Mobile Reviewer
│   │
│   └── knowledge/               # Reference Materials
│       ├── index.md
│       ├── design-patterns.md
│       ├── engineering-principles.md
│       ├── system-design.md
│       ├── testing-strategies.md
│       ├── frontend-development.md
│       ├── mobile-development.md
│       ├── code-review-guidelines.md
│       ├── pr-templates.md
│       ├── labels-conventions.md
│       └── cicd-quality-gates.md
│
└── resources/                   # Learning Resources
    └── README.md                # Curated AI/Claude Code resources
```

---

## Key Standards

| Standard | Threshold |
|----------|-----------|
| PR Size | < 400 lines |
| Code Coverage | >= 80% (new code) |
| Review Response | < 4 hours |
| Security Scan | No critical/high vulnerabilities |
| Accessibility | WCAG AA compliance |
| Performance | Core Web Vitals green |

---

## Context Maturity Matrix

Assess your AI readiness:

| Dimension | Low | Medium | High |
|-----------|-----|--------|------|
| **Codebase** | Can navigate | Understands patterns | Knows history |
| **Domain** | Basic terms | Business rules | Edge cases |
| **Architecture** | Component names | Data flow | Trade-offs |
| **Team** | Names/roles | Responsibilities | Communication |
| **Process** | Basic workflow | Quality gates | Why they exist |

**Score**: 4-5 High = Full AI leverage | 2-3 High = Supervised AI | 0-1 High = AI for learning

---

## Getting Started

### For AI Systems
```
You are a Senior [Backend/Frontend/Mobile] Engineer.
Follow the guidelines in agents/[specialty].md.
```

### For Teams
1. Clone this repository
2. Copy [PR templates](agents/knowledge/pr-templates.md) to `.github/`
3. Configure [labels](agents/knowledge/labels-conventions.md)
4. Set up [CI/CD gates](agents/knowledge/cicd-quality-gates.md)

### For Engineers
1. Review the [context model](#the-philosophy-context-driven-ai-usage)
2. Study the [knowledge base](agents/knowledge/)
3. Check the [resources](resources/) to level up

---

## Contributing

1. Follow existing structure and formatting
2. Include code examples in multiple languages
3. Update relevant README files
4. Keep content practical and actionable

## License

MIT License - Use and adapt freely.

---

*AI is a tool, not a replacement for understanding. The best results come from humans with context guiding AI with capabilities.*
