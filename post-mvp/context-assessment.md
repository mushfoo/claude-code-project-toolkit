# Post-MVP Context Assessment

Use this prompt to determine the appropriate evaluation approach for prioritizing post-MVP features based on your user context and available data.

---

**PROMPT:**

I need to systematically evaluate and prioritize Phase 2/3 features from my completed PRD. Before diving into feature evaluation, I need to establish the right approach based on my user context and available data.

## Current State Analysis

**Original PRD:**
```
[PASTE YOUR COMPLETED ORIGINAL PRD HERE]
```

**MVP Status:**
- [ ] MVP completed and deployed
- [ ] MVP in active use for [TIME PERIOD]
- [ ] MVP has [NUMBER] active users (including yourself)

**Current Usage Context:**
```
[DESCRIBE WHO IS CURRENTLY USING THE APPLICATION]
- Am I the primary/only user? 
- Do I have external users? How many?
- What's the mix of my usage vs. others?
- How long has it been in use?
```

## Context Assessment Framework

Based on my responses, please determine my **User Context Category** and provide the appropriate evaluation approach:

### Context Category 1: Solo Developer as Primary User
**Characteristics:**
- I am the main/only user of the application
- I built it to solve my own problems
- Limited or no external user feedback
- Success is primarily personal productivity/satisfaction

**Examples**: Personal productivity tools, hobby trackers, workflow automation

### Context Category 2: Solo Developer with External Users  
**Characteristics:**
- I built it for others to use
- I may use it myself, but primarily serves external users
- Have user feedback, support requests, or usage analytics
- Success measured by user adoption and satisfaction

**Examples**: SaaS tools, consumer apps, business solutions for others

### Context Category 3: Mixed User Context
**Characteristics:**
- I am a significant user AND have external users
- Both personal usage and user feedback inform decisions
- Success measured by both personal satisfaction and user metrics
- Need to balance my needs with user needs

**Examples**: Tools I use professionally that I've shared with colleagues/community

## Data Availability Assessment

For the identified context category, analyze what data I currently have:

### Personal Usage Data
- [ ] Daily usage patterns and frequency
- [ ] Specific pain points I've encountered
- [ ] Features I find myself wishing existed
- [ ] Workflow inefficiencies I've noticed

### External User Data
- [ ] User feedback (support tickets, emails, conversations)
- [ ] Usage analytics (if implemented)
- [ ] Feature requests from users
- [ ] User behavior observations

### Technical/Development Data
- [ ] Development effort required for each Phase 2/3 feature
- [ ] Technical debt or architecture improvements needed
- [ ] Integration complexity with existing features
- [ ] Learning opportunities that interest me

## Context-Specific Evaluation Criteria

Based on my context category, establish the appropriate evaluation criteria weighting:

### Solo Developer as Primary User Criteria
- **Daily Friction Reduction** (40%): How much will this improve my daily usage?
- **Personal Interest/Learning** (30%): Will building this be engaging/educational?
- **Technical Foundation** (20%): Does this enable future features I want?
- **Broader User Potential** (10%): Could this help others with similar needs?

### Solo Developer with External Users Criteria  
- **User Impact/Demand** (40%): How many users want/need this feature?
- **Development Feasibility** (25%): Can I build this with available time/skills?
- **Business/Growth Impact** (20%): Will this drive adoption or retention?
- **Personal Interest/Learning** (15%): Will I enjoy building this?

### Mixed User Context Criteria
- **Combined User Impact** (35%): Weight personal + external user benefit
- **Personal Usage Improvement** (25%): How much will this help my workflow?
- **Development Feasibility** (25%): Realistic implementation timeline
- **Strategic Value** (15%): Long-term product direction alignment

## Data Gathering Strategy

Based on my context and available data, recommend specific data gathering approaches:

### For Missing Personal Usage Data
- **Usage Journal**: Track interactions with current app for 1 week
- **Pain Point Documentation**: List friction moments as they occur
- **Wishlist Capture**: Note features desired during actual usage
- **Workflow Analysis**: Map current process vs. ideal process

### For Missing External User Data
- **Direct User Outreach**: Email/message current users for feedback
- **Analytics Implementation**: Add basic usage tracking if missing
- **Feature Request Collection**: Systematic review of all user communications
- **Competitive Analysis**: Research similar products' feature sets

### For Technical Assessment
- **Architecture Review**: Analyze current codebase for extension points
- **Effort Estimation**: Rough complexity assessment for each feature
- **Dependency Mapping**: Identify prerequisite features or refactoring
- **Learning Goal Alignment**: Match features to skills I want to develop

## Next Steps Recommendation

Based on the context assessment, provide:

1. **Immediate Data Gathering Tasks** (if any missing data identified)
2. **Appropriate Feature Evaluation Prompt** to use next
3. **Success Measurement Framework** for this context
4. **Timeline Recommendations** for evaluation and implementation

## Output Requirements

**Create these planning documents:**
- `planning/post-mvp-context-assessment.md` - This analysis and conclusions
- Update the context assessment results as input for the feature prioritization prompt
- Identify which follow-up prompts from the post-MVP toolkit to use next

Please analyze my current state and provide a clear path forward for systematic post-MVP feature prioritization.

---

**After Context Assessment:** Use the recommended feature prioritization prompt with the context-specific evaluation criteria established here.