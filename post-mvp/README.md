# Post-MVP Feature Development Toolkit

**Extension to the Claude Code Project Development Toolkit**

This directory contains prompts and examples for systematically growing your product after successful MVP completion.

## 📋 Prerequisites

Before using this post-MVP toolkit:
- ✅ Completed original toolkit workflow (PRD → UI → Tasks → Development → Launch)
- ✅ MVP successfully deployed and used for 1+ months
- ✅ Have 10+ Phase 2/3 features from original PRD to evaluate
- ✅ Some form of usage data, user feedback, or personal experience available

## 🎯 The Post-MVP Challenge

After successful MVP launch, you face new challenges:
- **Feature Request Overload**: Which of your 10+ Phase 2/3 features should you build?
- **Priority Confusion**: How do you balance personal interest vs. user needs vs. business impact?
- **Data Gaps**: How do you systematically evaluate features without enterprise processes?
- **Context Loss**: How do you preserve decision rationale for future reference?

## 📁 Files in This Directory

### **Core Prompts** (Conversation Starters)
- **`context-assessment.md`** - Determine evaluation approach based on user context
- **`feature-prioritization.md`** - Main systematic evaluation → PRD v2.0 creation
- **`user-feedback-analysis.md`** - Analyze external user feedback systematically
- **`success-metrics-framework.md`** - Establish measurable success criteria

### **Real-World Examples**
- **`examples/solo-primary-user-example.md`** - Book tracker scenario (you're the main user)
- **`examples/external-users-example.md`** - SaaS app scenario (building for others)
- **`examples/mixed-users-example.md`** - Developer tool scenario (you + community)

## 🚀 Quick Start Process

### **Step 1: Context Assessment** (10-15 minutes)
```
"Using post-mvp/context-assessment.md, help me determine my post-MVP evaluation approach"
```
**Output**: Your user context category + evaluation criteria + data gathering strategy

### **Step 2: User Feedback Analysis** (15-30 minutes - if external users)
```
"Using post-mvp/user-feedback-analysis.md, help me analyze my user feedback systematically"
```
**Output**: Categorized feedback + feature demand validation + user journey insights

### **Step 3: Feature Prioritization** (30-45 minutes)
```
"Using post-mvp/feature-prioritization.md, help me evaluate my Phase 2/3 features and create PRD v2.0"
```
**Output**: Systematic feature evaluation + prioritized roadmap + comprehensive PRD v2.0

### **Step 4: Success Metrics** (15-20 minutes)
```
"Using post-mvp/success-metrics-framework.md, help me establish success measurement for my prioritized features"
```
**Output**: Context-appropriate success framework + measurement implementation plan

## 🎭 Three User Context Categories

### **Solo Developer as Primary User**
**When**: You built the app primarily for yourself (personal productivity, hobby tools)
**Evaluation Focus**: Daily friction reduction (40%), Personal interest (30%), Technical foundation (20%)
**Example**: Personal book tracker, development productivity tools, hobby project managers

### **Solo Developer with External Users**  
**When**: You built the app for others to use (SaaS, consumer apps, business tools)
**Evaluation Focus**: User demand (40%), Development feasibility (25%), Business impact (20%)
**Example**: Task management SaaS, consumer productivity apps, business workflow tools

### **Mixed User Context**
**When**: You use the app significantly AND have external users (developer tools, shared utilities)
**Evaluation Focus**: Combined user impact (35%), Personal usage (25%), Feasibility (25%), Strategic value (15%)
**Example**: Developer tools, open source projects, professional utilities shared with community

## 📊 Context-Specific Evaluation Criteria

### **Solo Primary User Scoring**
- **Daily Friction Reduction** (40%): How much will this improve your daily workflow?
- **Personal Interest/Learning** (30%): Will building this be engaging/educational?
- **Technical Foundation** (20%): Does this enable future features you want?
- **Broader User Potential** (10%): Could this help others with similar needs?

### **External Users Scoring**
- **User Impact/Demand** (40%): How many users want/need this feature?
- **Development Feasibility** (25%): Can you build this with available time/skills?
- **Business/Growth Impact** (20%): Will this drive adoption or retention?
- **Personal Interest/Learning** (15%): Will you enjoy building this?

### **Mixed Context Scoring**
- **Combined User Impact** (35%): Weight both personal + external user benefit
- **Personal Usage Improvement** (25%): How much will this help your workflow?
- **Development Feasibility** (25%): Realistic implementation timeline
- **Strategic Value** (15%): Long-term product direction alignment

## 🔄 Integration with Original Toolkit

### **File Output Structure**
```
your-project/
├── planning/
│   ├── prd.md                         # Original MVP PRD (preserved)
│   ├── prd-v2.md                      # Post-MVP expansion PRD
│   ├── prd-change-log.md              # Version history
│   ├── post-mvp-context-assessment.md # User context analysis
│   ├── feature-evaluation-matrix.md   # Systematic feature scoring
│   └── success-metrics-framework.md   # Measurement approach
```

### **Workflow Continuation**
```
Original: PRD → UI → Tasks → Development → Launch
Extended: PRD v2.0 → UI Updates → New Tasks → Development → Success Measurement
```

### **Git Integration**
```bash
# After MVP completion
git tag mvp-complete

# Post-MVP planning
git checkout -b post-mvp-planning
[complete post-MVP evaluation]
git tag post-mvp-planning-complete

# Feature development
git checkout -b feature/high-priority-feature
```

## 📈 Success Measurement Approaches

### **Personal Productivity Metrics** (Solo Primary User)
- Usage frequency changes
- Task completion efficiency
- Personal satisfaction scores
- Workflow friction reduction

### **User-Centered Metrics** (External Users)
- Feature adoption rates
- User retention impact
- Support request changes
- User satisfaction feedback

### **Balanced Metrics** (Mixed Context)
- Personal productivity + community health
- Usage pattern analysis across user types
- Feature success across different contexts
- Strategic product direction validation

## 🎯 Quality Gates

### **Before Starting Post-MVP Process**
- [ ] MVP successfully used for 1+ months
- [ ] Clear list of Phase 2/3 features from original PRD
- [ ] Some form of usage data or feedback available (even if just personal)
- [ ] Original PRD accessible for reference

### **After Post-MVP Evaluation**
- [ ] User context clearly identified with appropriate evaluation criteria
- [ ] All Phase 2/3 features systematically scored with rationale
- [ ] PRD v2.0 created with prioritized roadmap
- [ ] Success metrics established for prioritized features
- [ ] Change log documents decision rationale

## 📚 Usage Examples

### **Book Tracker (Solo Primary User)**
- Context: Personal reading productivity tool
- Process: Personal usage analysis → friction-based prioritization → productivity metrics
- Result: Features that eliminate daily reading workflow friction

### **Task Management SaaS (External Users)**
- Context: Small business productivity tool with 150 users
- Process: User feedback analysis → demand-based prioritization → business metrics
- Result: Features that improve user retention and business growth

### **Developer Tool (Mixed Context)**
- Context: Personal snippet manager shared with community
- Process: Balanced analysis → combined impact prioritization → dual metrics
- Result: Features serving both personal needs and community growth

## 🔧 Tips for Success

### **Data Collection**
- **Personal Use**: Track your own usage patterns and pain points objectively
- **External Users**: Systematically collect feedback, don't rely on memory
- **Mixed Context**: Balance both perspectives, don't let one dominate

### **Evaluation Discipline**
- **Use the scoring framework**: Don't skip systematic evaluation
- **Document rationale**: Your future self will thank you
- **Consider trade-offs**: Every feature choice means not choosing others

### **Implementation Focus**
- **Start with highest-scoring features**: Trust your systematic evaluation
- **Measure success**: Don't build features without knowing if they work
- **Iterate based on results**: Use success data to guide next evaluation cycle

## 📞 Getting Help

### **Common Questions**
- **"Which context am I?"** Use the context assessment prompt - it will help you decide
- **"What if I have no external users?"** Use Solo Primary User approach
- **"How many features should I prioritize?"** Typically 2-4 high-scoring features per phase
- **"When should I repeat this process?"** Every 3-6 months or after major milestones

### **Troubleshooting**
- **Low confidence in scoring**: Review examples directory for similar scenarios
- **Conflicting priorities**: Document trade-offs in change log
- **No clear winner**: Consider if MVP is complete enough, or if features need refinement

---

**Next Steps**: Start with `context-assessment.md` to determine your approach, then proceed through the systematic evaluation process to create your PRD v2.0.