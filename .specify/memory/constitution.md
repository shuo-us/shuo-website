<!--
  Sync Impact Report
  ==================
  Version change: 0.0.0 → 1.0.0 (initial ratification)
  Modified principles: N/A (first version)
  Added sections:
    - Core Principles (5 principles)
    - Technology Stack
    - Development Workflow
    - Governance
  Removed sections: N/A
  Templates requiring updates:
    - .specify/templates/plan-template.md ✅ aligned
    - .specify/templates/spec-template.md ✅ aligned
    - .specify/templates/tasks-template.md ✅ aligned
  Follow-up TODOs: none
-->

# Shuo Voice Input Method Website Constitution

## Core Principles

### I. BDD-Driven Development (NON-NEGOTIABLE)

All features MUST follow Behavior-Driven Development methodology:

- Write user stories in Given-When-Then format before implementation
- Acceptance scenarios MUST be defined and approved before coding begins
- Tests derived from BDD scenarios MUST be written and fail before implementation
- Red-Green-Refactor cycle is strictly enforced
- Every feature MUST have independently testable acceptance criteria

**Rationale**: BDD ensures features align with user needs and provides living documentation of system behavior.

### II. Static-First Architecture

Leverage Astro's static site generation as the primary rendering strategy:

- Pages MUST be statically generated (SSG) by default
- Server-side rendering (SSR) ONLY when dynamic content is absolutely required
- Islands architecture for interactive components - minimize client-side JavaScript
- Content MUST be pre-rendered at build time whenever possible
- Static assets MUST be optimized and cached appropriately

**Rationale**: Static-first ensures maximum performance, security, and reliability for the official website.

### III. Accessibility Standards

The website MUST meet WCAG 2.1 AA compliance minimum:

- All interactive elements MUST be keyboard navigable
- ARIA labels and roles MUST be properly implemented
- Color contrast ratios MUST meet AA standards (4.5:1 for normal text)
- Voice input demonstrations MUST have text alternatives
- Screen reader compatibility MUST be verified for all pages

**Rationale**: As a voice input method product, accessibility is core to the brand identity and user trust.

### IV. Performance Budget

Page performance MUST meet defined thresholds:

- Largest Contentful Paint (LCP) < 2.5 seconds
- First Input Delay (FID) < 100 milliseconds
- Cumulative Layout Shift (CLS) < 0.1
- Total page weight < 500KB (excluding media assets)
- Time to Interactive (TTI) < 3.5 seconds on 4G connections

**Rationale**: The official website represents the product - poor performance undermines user confidence.

### V. Content Integrity

All product information and documentation MUST be accurate:

- Feature descriptions MUST match actual product capabilities
- Version information MUST be current and accurate
- Download links and installation instructions MUST be tested before publication
- Multilingual content (if applicable) MUST maintain semantic equivalence
- Broken links MUST be detected and fixed before deployment

**Rationale**: The official website is the primary source of truth for users - accuracy builds trust.

## Technology Stack

**Framework**: Astro (latest stable version)

**Language**: TypeScript for all interactive components

**Styling**: Tailwind CSS with design token system

**Testing**:
- BDD: Playwright for end-to-end acceptance tests
- Unit: Vitest for component and utility testing
- Visual: Chromatic or Percy for visual regression testing

**Deployment**: Static hosting (Vercel, Netlify, or Cloudflare Pages)

**CI/CD**: GitHub Actions for automated testing and deployment

## Development Workflow

### Feature Development Process

1. **Specify**: Write feature specification with BDD scenarios in `/specs/`
2. **Plan**: Create implementation plan with technical approach
3. **Test First**: Write acceptance tests from BDD scenarios - ensure they fail
4. **Implement**: Build feature to make tests pass
5. **Refactor**: Clean up while maintaining passing tests
6. **Review**: Code review with constitution compliance check
7. **Deploy**: Automated deployment after CI passes

### Quality Gates

- All BDD acceptance tests MUST pass before merge
- Lighthouse performance score MUST be >= 90
- Accessibility audit MUST show zero critical issues
- TypeScript strict mode MUST be enabled with no type errors
- All static links MUST be validated

## Governance

This constitution is the supreme governing document for the Shuo Voice Input Method Website project. All development decisions, code reviews, and architectural choices MUST comply with these principles.

### Amendment Process

1. Proposed changes MUST be documented with rationale
2. Impact analysis MUST be conducted across all principles
3. Version MUST be incremented following semantic versioning:
   - MAJOR: Principle removal or incompatible governance changes
   - MINOR: New principle or material expansion of guidance
   - PATCH: Clarifications, wording fixes, non-semantic refinements
4. All dependent templates and documentation MUST be updated
5. Changes take effect upon ratification date

### Compliance Review

- All pull requests MUST verify constitution compliance
- Architectural decisions MUST reference applicable principles
- Complexity MUST be justified against Simplicity principle
- Performance budgets MUST be validated before deployment

**Version**: 1.0.0 | **Ratified**: 2026-05-25 | **Last Amended**: 2026-05-25
