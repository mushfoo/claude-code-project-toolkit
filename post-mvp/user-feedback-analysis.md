# User Feedback Analysis for External Users

Use this prompt when you have external users and need to systematically analyze their feedback to inform post-MVP feature prioritization.

---

**PROMPT:**

I need to systematically analyze user feedback and usage data from my external users to inform post-MVP feature prioritization decisions. This analysis will feed into the feature evaluation process.

## Current User Data Inventory

**User Base Overview:**
```
Total Active Users: [Number]
User Acquisition Period: [Duration since MVP launch]
User Types/Segments: [Describe different user categories if any]
Geographic Distribution: [If relevant]
Usage Frequency Distribution: [Daily/Weekly/Monthly users]
```

**Available Feedback Sources:**
```
- [ ] Direct user emails/messages
- [ ] Support tickets or help requests  
- [ ] Feature requests submitted through [method]
- [ ] User interviews or conversations
- [ ] Analytics data showing user behavior
- [ ] Churn/retention patterns
- [ ] User onboarding completion rates
- [ ] Social media mentions or reviews
- [ ] Other: [Specify any other sources]
```

## Feedback Collection and Organization

### Direct User Communications
**Paste all relevant user feedback below:**

```
[PASTE USER EMAILS, MESSAGES, SUPPORT TICKETS, FEATURE REQUESTS]

Format each piece of feedback like this:
---
Date: [Date]
User ID/Type: [Anonymous identifier or user category]
Source: [Email, support ticket, conversation, etc.]
Content: [Full feedback content]
Category: [Bug, Feature Request, Praise, Complaint, Question]
---
```

### Usage Analytics Data
**If available, provide usage data:**

```
Most Used Features: [List top 3-5 features by usage]
Least Used Features: [Features with low adoption]
Drop-off Points: [Where users stop using the app]
Session Length Patterns: [How long users spend]
Feature Adoption Rates: [What % of users use each feature]
User Flow Analytics: [Common paths through the application]
```

### User Behavior Observations
**Document patterns you've noticed:**

```
Common User Workflows: [How users actually use the app]
Unexpected Use Cases: [Users doing things you didn't anticipate]
Workarounds: [Users creating their own solutions to limitations]
Support Request Patterns: [Recurring themes in help requests]
```

## Systematic Feedback Analysis

### Feedback Categorization
Please categorize all feedback into:

#### Feature Requests
- **High Demand** (3+ users requested): [List features]
- **Medium Demand** (2 users requested): [List features]  
- **Single Requests**: [List features requested by 1 user]

#### Pain Points and Friction
- **Critical Issues** (blocking user success): [List issues]
- **Moderate Friction** (annoying but workable): [List issues]
- **Minor Annoyances**: [List issues]

#### Praise and Satisfaction
- **Most Loved Features**: [What users specifically praise]
- **Workflow Successes**: [Where the app clearly helps users]
- **Unexpected Benefits**: [Value users found that you didn't anticipate]

#### Confusion and Usability Issues
- **Onboarding Problems**: [Where new users struggle]
- **Feature Discovery**: [Features users don't find or understand]
- **Interface Confusion**: [UI elements that confuse users]

### User Segmentation Analysis
If you have different user types, analyze feedback by segment:

#### User Segment 1: [Name/Description]
- **Primary Use Case**: [How this segment uses the app]
- **Key Pain Points**: [Their specific problems]
- **Feature Requests**: [What they're asking for]
- **Success Patterns**: [What works well for them]

#### User Segment 2: [Name/Description]
[Same structure as above]

### Feedback Validation and Prioritization

#### High-Confidence Insights
- **Consistent Patterns** (mentioned by 3+ users): [List patterns]
- **Critical Workflow Gaps**: [Missing functionality that blocks user success]
- **Clear Feature Demand**: [Features with strong user evidence]

#### Medium-Confidence Insights  
- **Emerging Patterns** (mentioned by 2 users): [List patterns]
- **Potential Improvements**: [Areas with some user evidence]
- **Speculative Needs**: [Things users might want but haven't clearly articulated]

#### Low-Confidence Insights
- **Single User Feedback**: [Isolated requests or issues]
- **Conflicting Feedback**: [Where users disagree]
- **Unclear Requests**: [Feedback that's hard to interpret]

### User Journey Mapping
Based on feedback, map the actual user experience:

#### Current User Journey
1. **Discovery**: [How users find the app]
2. **Onboarding**: [First experience, common issues]
3. **Initial Use**: [First real usage, success/failure points]
4. **Regular Use**: [Ongoing usage patterns, friction points]
5. **Advanced Use**: [Power user behaviors, feature requests]
6. **Churn Points**: [Where/why users stop using the app]

#### Ideal User Journey (Based on Feedback)
1. **Improved Discovery**: [How users wish they found it]
2. **Smoother Onboarding**: [What would help new users succeed]
3. **Better Initial Use**: [Removing early friction]
4. **Enhanced Regular Use**: [Features that would improve daily usage]
5. **Advanced Capabilities**: [Power user feature requests]
6. **Retention Improvements**: [What would keep users engaged]

## Feature Request Validation

### Demand vs. Effort Analysis
For each significant feature request:

```markdown
## Feature Request: [Feature Name]

### User Demand Evidence
- **Request Count**: [Number of users who requested this]
- **User Urgency**: [How critical users say this is]
- **Workaround Evidence**: [Are users creating manual solutions?]
- **Churn Connection**: [Do users leave without this feature?]

### Use Case Clarity
- **Primary Use Case**: [Main problem this solves]
- **User Story**: As a [user type], I want [feature] so that [benefit]
- **Success Criteria**: [How would users measure success?]
- **Edge Cases**: [Complications or variations mentioned]

### Business Impact Potential
- **User Retention**: [Would this help keep users?]
- **User Acquisition**: [Would this attract new users?]
- **User Satisfaction**: [How much would this improve experience?]
- **Competitive Advantage**: [Does this differentiate from competitors?]
```

## Integration with Original PRD Features

### Phase 2/3 Feature Validation
Compare user feedback against original PRD features:

#### Strong User Validation
- **Original Feature**: [Feature from PRD]
- **User Evidence**: [How user feedback supports this]
- **Priority Adjustment**: [Should this move up in priority?]

#### Weak User Validation  
- **Original Feature**: [Feature from PRD]
- **User Evidence**: [Limited or no user support]
- **Priority Adjustment**: [Should this move down or be reconsidered?]

#### New Features Discovered
- **Feature Not in Original PRD**: [New feature from user feedback]
- **User Evidence**: [Why users want this]
- **PRD Integration**: [How this fits with original vision]

## Actionable Insights Summary

### Top 5 User-Driven Priorities
1. **[Priority 1]**: [Brief description] - [Evidence level]
2. **[Priority 2]**: [Brief description] - [Evidence level]
3. **[Priority 3]**: [Brief description] - [Evidence level]
4. **[Priority 4]**: [Brief description] - [Evidence level]
5. **[Priority 5]**: [Brief description] - [Evidence level]

### Critical User Experience Fixes
- **[Fix 1]**: [Problem and proposed solution]
- **[Fix 2]**: [Problem and proposed solution]
- **[Fix 3]**: [Problem and proposed solution]

### Strategic Feature Opportunities
- **[Opportunity 1]**: [Feature with high user impact potential]
- **[Opportunity 2]**: [Feature with competitive advantage]
- **[Opportunity 3]**: [Feature with user retention impact]

## User Feedback Integration Strategy

### Ongoing Feedback Collection
- **Regular Check-ins**: [How to systematically gather ongoing feedback]
- **Feature Validation**: [How to test new features with users before building]
- **Success Measurement**: [How to know if changes are working]

### User Communication Plan
- **Acknowledgment**: [How to let users know their feedback was heard]
- **Feature Updates**: [How to communicate new features to users]
- **Expectation Management**: [How to handle requests that won't be implemented]

## Output for Feature Prioritization

**Key Data Points for PRD v2.0:**
- **High-confidence user demands**: [List with evidence]
- **Critical user experience gaps**: [Problems to solve first]
- **User segment priorities**: [Which users to focus on]
- **Feature validation data**: [Evidence for/against original PRD features]

**Recommended Adjustments to Original PRD:**
- **Promote to higher priority**: [Features with strong user evidence]
- **Demote or reconsider**: [Features with weak user evidence]
- **Add to consideration**: [New features discovered through feedback]

This analysis will feed directly into the feature prioritization scoring, where user demand and validation will be weighted according to your user context category.

---

**Next Step:** Use this feedback analysis as input to the Post-MVP Feature Prioritization prompt, ensuring that real user needs drive your PRD v2.0 decisions.