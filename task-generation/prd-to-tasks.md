# PRD to Tasks Breakdown Prompt

Use this prompt to convert a completed PRD into a detailed, actionable task breakdown for development.

---

**PROMPT:**

You are a technical project manager creating a detailed task breakdown from a completed Product Requirements Document (PRD). Your goal is to transform the PRD into specific, actionable development tasks with clear priorities, dependencies, and acceptance criteria.

## PRD to Analyze

**PRD Document:**

```
[PASTE THE COMPLETE PRD DOCUMENT HERE]
```

**UI Prototypes** (if available):

```
[PASTE DETAILS ABOUT UI PROTOTYPES FROM planning/ui-prototypes/ OR STATE "No UI prototypes available"]
```

## Task Breakdown Structure to Create

### 1. Project Setup & Foundation Tasks

Break down initial setup into specific tasks:

- **Repository Setup**: Git repository, branch strategy, initial commit
- **Development Environment**: Docker, local development setup, tooling configuration
- **CI/CD Pipeline**: GitHub Actions, testing automation, deployment pipeline
- **Documentation Structure**: README, contributing guidelines, project documentation

### 2. Architecture & Infrastructure Tasks

Convert technical architecture into implementation tasks:

- **Core Architecture**: Project structure, configuration management, core services
- **Database/Storage Setup**: Data layer implementation, migration strategy
- **API Foundation**: Route structure, middleware, authentication framework
- **Frontend Foundation**: Component library, routing, state management setup

### 3. Feature Development Tasks

Break each PRD feature into granular development tasks:

#### For Each Major Feature:

- **Backend Implementation**: API endpoints, business logic, data models
- **Frontend Implementation**: UI components, user interactions, data integration
- **UI Implementation** (if prototypes available): Convert UI prototypes to functional components
- **Testing Implementation**: Unit tests, integration tests, E2E tests
- **Documentation**: API docs, user guides, inline code documentation

### 4. Integration & Testing Tasks

Convert testing requirements into specific tasks:

- **Unit Testing**: Individual component and function tests
- **Integration Testing**: API integration, database integration, third-party service integration
- **End-to-End Testing**: Complete user workflow tests
- **Performance Testing**: Load testing, response time validation
- **Security Testing**: Input validation, authentication, authorization tests

### 5. Deployment & Operations Tasks

Transform deployment requirements into actionable tasks:

- **Production Environment**: Server setup, domain configuration, SSL certificates
- **Monitoring Setup**: Logging, metrics, alerting, health checks
- **Backup Strategy**: Data backup, recovery procedures, backup testing
- **Documentation**: Deployment guides, operational runbooks

## Task Format Requirements

For each task, provide:

### Task Template:

```markdown
## Task [ID]: [Clear, Action-Oriented Title]

**Epic**: [Which major feature/epic this belongs to]
**Priority**: [High/Medium/Low]
**Estimated Effort**: [Hours or Story Points]
**Dependencies**: [List any tasks that must be completed first]

### Description

[Clear description of what needs to be accomplished]

### Acceptance Criteria

- [ ] [Specific, testable criterion 1]
- [ ] [Specific, testable criterion 2]
- [ ] [Specific, testable criterion 3]

### Technical Notes

[Any technical implementation details, gotchas, or considerations]

### Testing Requirements

- [ ] [Unit tests written and passing]
- [ ] [Integration tests implemented]
- [ ] [Manual testing checklist completed]

### Definition of Done

- [ ] [Code written and reviewed]
- [ ] [Tests passing with >90% coverage]
- [ ] [Documentation updated]
- [ ] [Feature deployed and validated]
```

## Git Workflow Integration

Each task should include git workflow requirements:

- **Branch naming convention**: `feature/task-[id]-[short-description]`
- **Commit message format**: `Task [ID]: [Clear description of changes]`
- **Pull request requirements**: What must be included in PR description
- **Review criteria**: What reviewers should check

## Prioritization Guidelines

### High Priority (Week 1-2):

- Foundation and setup tasks that other work depends on
- Core MVP features that deliver immediate user value
- Critical path items that block other development

### Medium Priority (Week 3-4):

- Important features that enhance user experience
- Nice-to-have functionality within MVP scope
- Performance optimizations and polish

### Low Priority (Future Phases):

- Advanced features for later phases
- Optimizations that don't impact core functionality
- Documentation improvements and tooling enhancements

## Task Dependencies Management

Create a clear dependency chain:

1. **Foundation Tasks**: Must be completed before any feature work
2. **Core Features**: Can be developed in parallel once foundation is ready
3. **Integration Tasks**: Require multiple components to be complete
4. **Polish Tasks**: Final testing, documentation, and deployment preparation

## Development Workflow Integration

Each task should specify:

- **Development environment requirements**
- **Testing approach and tools to use**
- **Code review checklist items**
- **Deployment considerations**
- **User validation approach**

## Instructions for Task Creation

1. **Review the entire PRD**: Understand all requirements, constraints, and success criteria

2. **Check for UI prototypes**: If UI prototypes are available, include specific UI implementation tasks

3. **Identify major epics**: Group related functionality into logical development phases

4. **Break down each epic**: Create granular tasks that can be completed in 1-4 hours

5. **Establish dependencies**: Ensure tasks are ordered logically and dependencies are clear

6. **Assign realistic estimates**: Base effort estimates on similar tasks and team capabilities

7. **Include testing requirements**: Every feature task should have corresponding testing tasks

8. **Consider Claude Code workflow**: Optimize task breakdown for rapid development with comprehensive testing

9. **Validate completeness**: Ensure all PRD requirements are covered by tasks

## Special Considerations for Claude Code Development

- **Detailed specifications**: Each task should have enough detail for Claude to implement without additional clarification
- **Testing emphasis**: Include specific testing requirements and user validation steps
- **Integration focus**: Ensure tasks validate real-world functionality, not just code completion
- **Documentation parity**: Include documentation tasks alongside feature development
- **Simplicity reminders**: Reference development guidelines to prevent over-engineering

## Output Format

Please create:

1. **Executive Summary**: Overview of total tasks, estimated timeline, and major milestones
2. **Epic Breakdown**: High-level grouping of tasks by major functionality
3. **Detailed Task List**: Complete task breakdown with all required information
4. **Dependency Graph**: Visual or textual representation of task dependencies
5. **Sprint Planning Suggestions**: Recommended grouping of tasks for development sprints

Analyze the provided PRD and create a comprehensive task breakdown following this structure.
