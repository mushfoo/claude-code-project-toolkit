# PRD Refinement Prompt

Use this prompt to refine and improve an existing PRD based on feedback, changing requirements, or new insights.

---

**PROMPT:**

You are an experienced product manager reviewing and refining an existing Product Requirements Document (PRD). Your goal is to improve the document based on new information, stakeholder feedback, or changed circumstances while maintaining the integrity of the original vision.

## Current PRD to Refine

**Existing PRD:**
```
[PASTE THE CURRENT PRD DOCUMENT HERE]
```

## Refinement Context

**Type of Refinement Needed:**
- [ ] Stakeholder feedback incorporation
- [ ] Scope adjustment (expansion or reduction)
- [ ] Technical constraint updates
- [ ] Timeline modifications
- [ ] Budget constraint changes
- [ ] User research insights
- [ ] Competitive analysis updates
- [ ] Post-MVP planning
- [ ] Other: [SPECIFY]

**Specific Changes Requested:**
```
[DESCRIBE THE SPECIFIC CHANGES, FEEDBACK, OR NEW REQUIREMENTS TO ADDRESS]
```

**New Constraints or Requirements:**
```
[LIST ANY NEW TECHNICAL, BUDGET, TIMELINE, OR BUSINESS CONSTRAINTS]
```

## Refinement Guidelines

### 1. Maintain Document Integrity
- **Preserve the core vision** unless explicitly changing project direction
- **Keep successful elements** that are working well
- **Maintain internal consistency** across all sections
- **Update version number and date** to reflect changes

### 2. Impact Analysis
Before making changes, analyze:
- **Scope Impact**: How do changes affect feature scope and timeline?
- **Technical Impact**: Do changes require architecture modifications?
- **Resource Impact**: How do changes affect budget, timeline, or team requirements?
- **User Impact**: Do changes affect user experience or target personas?
- **Risk Impact**: Do changes introduce new risks or mitigate existing ones?

### 3. Stakeholder Alignment
- **Address all feedback**: Ensure every piece of stakeholder input is considered
- **Document decisions**: Explain why certain feedback was or wasn't incorporated
- **Maintain traceability**: Show how changes relate to original requirements
- **Update success metrics**: Adjust KPIs if goals have changed

## Common Refinement Scenarios

### Scope Reduction (Budget/Timeline Constraints)
**Tasks:**
- Move features from MVP to Phase 2
- Identify minimum viable feature set
- Update timeline and resource estimates
- Revise success metrics to match reduced scope
- Update Definition of Done criteria

### Scope Expansion (New Requirements)
**Tasks:**
- Assess new features against current architecture
- Update timeline and resource requirements
- Identify new risks and mitigation strategies
- Revise user stories and acceptance criteria
- Update technical architecture if needed

### Technical Constraint Changes
**Tasks:**
- Revise technology stack recommendations
- Update integration strategies
- Modify performance requirements
- Adjust development timeline estimates
- Update Claude Code considerations

### User Research Insights
**Tasks:**
- Refine user personas based on new data
- Update problem statement with new insights
- Modify user stories and acceptance criteria
- Adjust UI/UX requirements
- Update success metrics and validation approaches

### Post-MVP Feedback
**Tasks:**
- Incorporate lessons learned from MVP
- Update Phase 2 and Phase 3 planning
- Revise architecture based on real-world usage
- Adjust user stories based on actual user behavior
- Update risk assessment with known issues

## Refinement Process

### Step 1: Document Current State
- **Version control**: Create a new version of the PRD
- **Change log**: Document what's being modified and why
- **Stakeholder review**: Note who requested changes and when

### Step 2: Analyze Requested Changes
- **Feasibility assessment**: Determine if requested changes are technically and practically possible
- **Trade-off analysis**: Identify what must be sacrificed to accommodate new requirements
- **Risk evaluation**: Assess new risks introduced by changes

### Step 3: Update Document Sections

#### Executive Summary Updates
- Revise success metrics if goals have changed
- Update timeline if scope has significantly changed
- Modify vision statement if direction has shifted

#### Problem Statement Refinements
- Incorporate new user research or market insights
- Update user personas based on feedback or data
- Refine pain points based on real user interactions

#### Requirements Modifications
- Add, remove, or modify features based on feedback
- Adjust MVP scope to meet new constraints
- Update future phase planning with new priorities

#### Technical Architecture Adjustments
- Modify technology choices based on new constraints
- Update integration strategies for new requirements
- Revise performance targets based on real-world data

#### Timeline and Resource Updates
- Adjust development phases based on scope changes
- Update effort estimates with new information
- Revise risk mitigation strategies

### Step 4: Validate Changes
- **Internal consistency check**: Ensure all sections align with changes
- **Stakeholder review**: Confirm changes address original feedback
- **Technical feasibility**: Validate that updated requirements are achievable

## Change Documentation Template

For each major change, document:

```markdown
### Change [ID]: [Change Title]

**Section Affected**: [Which PRD section is being modified]
**Requested By**: [Stakeholder or trigger for change]
**Date**: [When change was requested]

**Original Requirement**:
[What the PRD previously specified]

**Updated Requirement**:
[What the PRD now specifies]

**Rationale**:
[Why this change is being made]

**Impact Assessment**:
- **Scope**: [How this affects project scope]
- **Timeline**: [How this affects development timeline]
- **Resources**: [How this affects budget/team requirements]
- **Risk**: [New risks or risk mitigations]

**Dependencies**:
[Other PRD sections that need updates due to this change]
```

## Version Control Standards

### Version Numbering
- **Major changes** (scope, timeline, architecture): Increment major version (v1.0 → v2.0)
- **Minor changes** (feature adjustments, refinements): Increment minor version (v1.0 → v1.1)
- **Editorial changes** (typos, clarifications): Increment patch version (v1.0 → v1.0.1)

### Change Tracking
- Maintain a **change log** at the top of the PRD
- Use **track changes** or **comments** for stakeholder review
- **Archive previous versions** for reference
- **Document decision rationale** for major changes

## Quality Assurance Checklist

Before finalizing refinements, verify:

### Consistency Checks
- [ ] All sections reflect the same updated requirements
- [ ] Timeline estimates align with updated scope
- [ ] Success metrics match updated goals
- [ ] Technical architecture supports all updated requirements
- [ ] User stories align with updated personas and pain points

### Completeness Checks  
- [ ] All requested feedback has been addressed
- [ ] All new requirements have clear acceptance criteria
- [ ] Updated risks have mitigation strategies
- [ ] Changed timelines include all necessary tasks
- [ ] Resource requirements reflect actual scope

### Stakeholder Alignment
- [ ] Changes address original concerns that triggered refinement
- [ ] Trade-offs are clearly documented and justified
- [ ] Updated success metrics are achievable and measurable
- [ ] All stakeholders understand impact of changes

## Communication Strategy

### Change Summary Document
Create a separate summary for stakeholders:
- **What changed**: High-level overview of modifications
- **Why it changed**: Business rationale for updates
- **Impact summary**: Timeline, budget, and scope implications
- **Next steps**: How changes affect immediate development plans

### Stakeholder Review Process
- **Review period**: Allow appropriate time for stakeholder feedback
- **Review criteria**: Specify what feedback is needed
- **Decision timeline**: Set deadlines for final approval
- **Communication channels**: Specify how feedback should be provided

## Instructions for Refinement

1. **Analyze the current PRD thoroughly**: Understand the existing requirements, constraints, and decisions

2. **Categorize requested changes**: Group similar changes together for efficient processing

3. **Assess change impact**: Evaluate how each change affects other parts of the project

4. **Prioritize changes**: Some changes may be more critical than others

5. **Update systematically**: Work through the PRD section by section to ensure consistency

6. **Document all decisions**: Maintain clear rationale for why changes were made

7. **Validate the updated PRD**: Ensure the refined document still serves its purpose as a development guide

Please analyze the provided PRD and refinement requirements, then create an updated version that addresses all requested changes while maintaining document quality and internal consistency.

## Output Requirements

**Update the existing PRD file**: `planning/prd.md`
- Modify the existing file in place
- Use git commits to track changes and versions
- Include a clear commit message describing the refinements made
- Consider creating a git tag for major version milestones
