# Post-MVP Feature Prioritization

Use this prompt to systematically evaluate and prioritize Phase 2/3 features from your original PRD, creating a comprehensive PRD v2.0 with implementation roadmap.

---

**PROMPT:**

I need to create a systematic evaluation of my post-MVP features and generate a prioritized PRD v2.0 that builds on my successful MVP implementation.

## Input Information

**Original PRD:**
```
[PASTE YOUR COMPLETED ORIGINAL PRD HERE]
```

**Context Assessment Results:**
```
[PASTE RESULTS FROM POST-MVP CONTEXT ASSESSMENT OR PROVIDE:]

User Context Category: [Solo Dev as Primary User / Solo Dev with External Users / Mixed User Context]

Available Data:
- Personal usage data: [Yes/No - describe]
- External user feedback: [Yes/No - describe] 
- Usage analytics: [Yes/No - describe]
- Feature requests: [List any specific requests]

Evaluation Criteria Weighting:
[The criteria weightings determined in context assessment]
```

**Current Application Status:**
```
MVP Deployment Date: [Date]
Active Usage Period: [Duration] 
Current User Base: [Number and type of users]
Key Success Metrics Achieved: [List any measures of MVP success]
```

**Phase 2/3 Features from Original PRD:**
```
[LIST ALL FEATURES FROM PHASE 2 AND PHASE 3 OF YOUR ORIGINAL PRD]
Feature 1: [Brief description]
Feature 2: [Brief description]
...
[Continue for all 10+ features]
```

## Systematic Feature Evaluation Process

For each Phase 2/3 feature, provide a comprehensive evaluation:

### Feature Evaluation Template

```markdown
## Feature Evaluation: [Feature Name]

### Original PRD Context
- **Phase**: [2 or 3 from original PRD]
- **Original Description**: [Copy from original PRD]
- **Original Rationale**: [Why this was included in original PRD]

### Current Relevance Assessment
- **User Context Fit**: [How well does this serve my identified user context?]
- **Data-Driven Evidence**: [What usage data/feedback supports or contradicts this feature?]
- **Personal Experience**: [If I'm a user, how much would this improve my experience?]

### Evaluation Scoring
Using the context-specific criteria weighting:

**Criterion 1** ([Weight]%): [Score 1-5] - [Justification]
**Criterion 2** ([Weight]%): [Score 1-5] - [Justification]  
**Criterion 3** ([Weight]%): [Score 1-5] - [Justification]
**Criterion 4** ([Weight]%): [Score 1-5] - [Justification]

**Total Weighted Score**: [Calculate weighted average]

### Implementation Considerations
- **Development Complexity**: [High/Medium/Low with brief explanation]
- **Architecture Impact**: [Does this require significant changes to existing code?]
- **Prerequisites**: [Any other features or refactoring required first?]
- **Risk Assessment**: [What could go wrong with this feature?]

### User Impact Prediction
- **Primary User Type Served**: [Which users benefit most?]
- **Usage Frequency Expected**: [Daily/Weekly/Monthly/Occasional]
- **Success Measurement**: [How will I know this feature succeeded?]
```

## Feature Prioritization Matrix

After evaluating all features, create a prioritization matrix:

### High Priority Features (Score 4.0+)
[List features with scores above 4.0]
- **Recommended for Next Development Phase**
- **Implementation Order**: [Suggest sequence based on dependencies]

### Medium Priority Features (Score 2.5-3.9)
[List features in this range]
- **Consider for Future Phases**
- **Re-evaluate After High Priority Completion**

### Low Priority Features (Score <2.5)
[List features below 2.5]
- **Archive or Significantly Modify**
- **Document Decision Rationale**

### Deferred/Archived Features
[Any features that should be removed or significantly changed]
- **Rationale**: [Why these don't fit current context]
- **Future Consideration**: [Conditions under which to revisit]

## PRD v2.0 Creation

Based on the feature evaluation, create a comprehensive PRD v2.0:

### PRD v2.0 Structure

```markdown
# [Project Name] PRD v2.0 - Post-MVP Feature Expansion

## Document Information
- **Version**: 2.0
- **Date**: [Current Date]
- **Status**: Post-MVP Feature Planning
- **Based On**: [Original PRD] v1.0 - MVP (Completed [Date])

## Executive Summary - Evolution
- **MVP Success Summary**: [Brief recap of MVP achievements]
- **Version 2.0 Vision**: [What this expansion aims to achieve]
- **Key Feature Additions**: [3-4 most important new features]
- **Updated Success Metrics**: [How success will be measured for v2.0]

## User Context and Learnings
- **User Base Evolution**: [How users/usage have evolved since MVP]
- **Key Insights**: [What was learned from MVP usage]
- **Pain Points Identified**: [Friction discovered in real usage]
- **Opportunity Areas**: [Where the most value can be added]

## Feature Roadmap

### Phase 2A: Immediate Enhancements (Next 1-2 months)
[High priority features that address current pain points]

**Feature 2A.1: [Feature Name]**
- **User Story**: As a [user type], I want [capability] so that [benefit]
- **Acceptance Criteria**: [Specific, testable requirements]
- **Success Metrics**: [How to measure success]
- **Implementation Notes**: [Key technical considerations]

[Repeat for each Phase 2A feature]

### Phase 2B: Value Expansion (Months 3-4)
[Medium-high priority features that add significant value]

### Phase 3: Advanced Capabilities (Future)
[Lower priority features for later consideration]

## Updated Technical Architecture
- **Architecture Changes**: [Any modifications needed for new features]
- **Integration Points**: [How new features connect to existing system]
- **Performance Considerations**: [Impact on existing performance]
- **Security Updates**: [Any security implications of new features]

## Success Measurement Framework
- **Feature-Specific Metrics**: [How to measure each feature's success]
- **Overall Product Health**: [Metrics for overall product direction]
- **User Satisfaction Indicators**: [How to track user benefit]
- **Development Velocity**: [Tracking implementation efficiency]

## Risk Assessment and Mitigation
- **Feature Scope Creep**: [How to prevent over-engineering]
- **User Experience Degradation**: [Ensuring new features don't hurt existing UX]
- **Technical Debt**: [Managing complexity as features are added]
- **Maintenance Burden**: [Ensuring sustainable feature set]

## Implementation Timeline
- **Phase 2A Timeline**: [Realistic schedule for immediate features]
- **Dependency Management**: [How features depend on each other]
- **Milestone Checkpoints**: [When to evaluate progress and adjust]
- **Success Gates**: [Criteria for proceeding to next phase]
```

## Change Documentation

Create a comprehensive change log documenting the evolution:

### PRD Change Log Entry

```markdown
# PRD Change Log

## v2.0 - Post-MVP Feature Expansion
**Date**: [Current Date]
**Trigger**: MVP completed successfully, evaluating Phase 2/3 features
**Development Context**: [User context category and available data]

### Changes Made
- **Added to Phase 2A**: [List high priority features moved up]
- **Modified Features**: [Any features changed from original conception]
- **Archived Features**: [Features removed or significantly delayed]
- **New Features**: [Any entirely new features identified]

### Decision Rationale
**Data Sources Used**:
- [List data sources that informed decisions]

**Key Decision Factors**:
- [Primary reasons for prioritization choices]

**Trade-offs Made**:
- [What was sacrificed for what gains]

### Success Criteria Changes
- **Original MVP Metrics**: [How these evolved]
- **New Success Measures**: [Additional metrics for v2.0]

### Risk Mitigation Updates
- **New Risks Identified**: [Risks that emerged from evaluation]
- **Updated Mitigation Strategies**: [How risks will be addressed]

## v1.0 - Original MVP
**Date**: [Original Date]  
**Status**: ✅ Completed and Successfully Deployed
**Usage Period**: [Duration] with [User base description]
**Key Achievements**: [Primary MVP successes]
```

## Integration with Development Workflow

### Next Steps After PRD v2.0
1. **UI/UX Updates**: Extend existing prototypes for new features
2. **Task Breakdown**: Convert prioritized features to development tasks
3. **Development Guidelines**: Apply simplicity principles to new features
4. **Testing Strategy**: Plan validation approach for each new feature

### Onboarding Prompt Updates
- **Update project context** with v2.0 vision
- **Add Phase 2A features** to current development focus
- **Include success metrics** for new features
- **Update Playwright testing** for enhanced user flows

## Output Requirements

**Save completed documents as:**
- `planning/prd-v2.md` - Complete PRD v2.0 document
- `planning/prd-change-log.md` - Version history and change documentation
- `planning/feature-evaluation-matrix.md` - Detailed scoring for all features

**Git workflow:**
- Commit original PRD as historical record
- Create feature branch for v2.0 planning: `git checkout -b planning/prd-v2`
- Commit all new planning documents
- Tag the v2.0 planning completion: `git tag v2.0-planning`

## Instructions for Implementation

1. **Complete systematic evaluation** of all Phase 2/3 features using context-appropriate criteria
2. **Create prioritization matrix** with clear scoring rationale
3. **Generate comprehensive PRD v2.0** that builds logically on MVP success
4. **Document all decisions** with clear reasoning for future reference
5. **Establish success measurement** framework appropriate for user context
6. **Create actionable roadmap** with realistic timelines for solo development

Please analyze my features systematically and create a comprehensive PRD v2.0 that will guide the next phase of development with the same rigor as the original PRD guided the MVP.

---

**After PRD v2.0 Creation:** Use the UI/UX design extension prompts to update prototypes for new features, then use task breakdown prompts to convert prioritized features into actionable development tasks.