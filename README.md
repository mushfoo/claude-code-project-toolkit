# Claude Code Project Development Toolkit

**Problem**: Claude Code is incredibly powerful but has critical limitations that derail projects:

- 🧠 **Context Loss**: Each new session starts from scratch, losing project history and decisions
- ⚙️ **Over-Engineering**: Claude naturally creates complex solutions when simple ones work better  
- 📈 **Scope Creep**: Claude will happily build whatever you ask for without questioning necessity
- 🔀 **Inconsistent Patterns**: Without guidance, Claude uses different approaches across sessions
- 🧪 **Testing Gaps**: Claude focuses on making code work, not on real-world user validation

**Solution**: This toolkit provides systematic processes that work *with* Claude Code's strengths while compensating for its limitations. Transform vague ideas into structured requirements, maintain context across sessions, and ensure every development session builds toward shipping working software that solves real user problems.

> **Note**: These prompts are optimized and tested specifically for Claude Code. The principles may apply to other AI development tools, but effectiveness is only verified with Claude Code.

## 📁 Toolkit Files

```
claude-code-project-toolkit/
├── README.md                           # This guide
├── development-guidelines.md           # Reference doc - copy into projects
├── prd-prompts/
│   ├── initial-prd-creation.md        # Conversation starter: idea → comprehensive PRD (30-60 min)
│   └── prd-refinement.md              # Conversation starter: update PRDs based on feedback (15-30 min)
├── task-generation/
│   └── prd-to-tasks.md                # Conversation starter: PRD → detailed task breakdown (20-40 min)
└── claude-onboarding/
    └── onboarding-prompt-generator.md  # Conversation starter: PRD → project-specific onboarding prompt (10-15 min)
```

## 🚀 Quick Start Guide

### 1. **Create PRD** (30-60 minutes)
- Copy `prd-prompts/initial-prd-creation.md`
- Paste into Claude Code and answer questions about your project
- Get comprehensive PRD

### 2. **Generate Tasks** (20-40 minutes)  
- Copy `task-generation/prd-to-tasks.md`
- Paste into Claude Code with your completed PRD
- Get detailed task breakdown with priorities and timelines

### 3. **Setup Onboarding** (10-15 minutes)
- Copy `claude-onboarding/onboarding-prompt-generator.md` 
- Paste into Claude Code with your PRD and answer follow-up questions
- Get customized onboarding prompt for your project

### 4. **Development Setup** (5 minutes)
- Copy `development-guidelines.md` into your project repository
- Save your generated onboarding prompt for daily use
- Start developing with systematic task completion!

## 📋 Best Practices

### **All files are conversation starters** - copy from file, paste into Claude Code, no editing needed

### **For PRD Creation**
- Be specific with concrete examples and measurable success criteria
- Focus on real user problems, not theoretical features
- Include Claude Code development considerations for rapid iteration

### **For Task Breakdown**
- Each task should be completable in 1-4 hours
- Include testing requirements alongside feature development
- Make dependencies clear and realistic

### **For Development**
- Follow `development-guidelines.md` to prevent over-engineering
- Test every feature by actually using it as intended
- Always use feature branches, never commit directly to main
- Maintain >90% test coverage with meaningful tests

### **For Onboarding**
- Regenerate onboarding prompts when project context changes
- Include enough context for effective development continuation
- Reference guidelines file rather than duplicating content

## 📚 Example Usage

### **New Dashboard Project**
1. PRD Creation (45 min) → Task Breakdown (30 min) → Onboarding Setup (15 min)
2. Copy development guidelines into project repo
3. Daily development using onboarding prompt for each Claude Code session

### **Existing Project Evolution**  
1. PRD Refinement (20 min) with new requirements
2. Generate new tasks (15 min) for additional features
3. Regenerate onboarding prompt (10 min) with updated context

### **Team Handoff**
1. Ensure PRD and tasks are current
2. Verify onboarding prompt has complete project context  
3. Share development guidelines with new team members

## 🔄 Maintenance

**Weekly**: Update task progress, refine estimates based on actual velocity  
**At Milestones**: Update PRD for scope changes, regenerate onboarding prompt  
**Continuously**: Document lessons learned, improve templates based on experience

## 📞 Support

**Using the Toolkit**: Start with Quick Start Guide, reference individual files for detailed usage  
**Improving the Toolkit**: Document successful adaptations, suggest improvements based on real project experience

---

**Goal**: Systematic, repeatable project success through structured planning and consistent Claude Code development practices.