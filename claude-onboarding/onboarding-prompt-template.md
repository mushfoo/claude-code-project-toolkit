# {project_name} - Onboarding Prompt

## Project Context

**Project**: {project_name}
**Description**: {project_description}
**Status**: {project_status}
**Current Phase**: {current_phase}
**Repository**: {repository_url}

### Technology Stack
{technology_stack}

### Architecture Overview
{architecture_overview}

### Target Users
{target_users}

### Core Functionality
{core_functionality}

## Getting Started

### Step 1: Repository Setup
1. **Current branch**: `{current_branch}`
2. **Never commit directly to**: `{protected_branches}`
3. **Feature branch pattern**: `{branch_pattern}`

### Step 2: Read Key Documents
Essential reading order:
1. **PRD**: `planning/prd.md` - Full project requirements and vision
2. **UI Prototypes**: `{ui_prototypes_location}` - Visual designs and user flows
3. **Task Breakdown**: `planning/task-breakdown.md` - Development tasks and priorities
4. **Development Guidelines**: `development-guidelines.md` - Coding standards and best practices

### Step 3: Development Environment
```bash
# Install dependencies
{install_command}

# Start development server
{dev_server_command}

# Run tests
{test_command}

# Run linting
{lint_command}
```

### Step 4: Current Sprint/Tasks
**Current Focus**: {current_focus}
**Active Tasks**: 
{active_tasks}

**Next Priorities**:
{next_priorities}

### Step 5: UI/UX Validation with Playwright
**Critical validation step using Task agents for systematic testing before PR creation.**

#### 5.1 Setup and Environment
1. **Start Development Server**: `{dev_server_command}` ({dev_server_url})
2. **Verify Test Environment**: Ensure all implemented features are accessible

#### 5.2 Core User Experience Validation
Delegate comprehensive testing to Task agents for systematic coverage:

```bash
# Primary user flow testing
claude "Create a Task agent to comprehensively test {project_name} at {dev_server_url}:

CORE WORKFLOWS TO TEST:
{core_user_flows_list}

VALIDATION REQUIREMENTS:
- Take screenshots at each major step
- Test with realistic data ({data_volume_requirement})
- Verify all interactive elements respond within {performance_requirement}
- Document any broken workflows or UX friction points
- Report completion rates for each workflow"
```

#### 5.3 Mobile-First Testing ({primary_viewport_size} Viewport)
**Primary testing target - mobile experience is critical:**

```bash
# Mobile-first validation agent
claude "Create a Task agent for mobile UX testing on {project_name}:

MOBILE TESTING PROTOCOL:
1. Set viewport to {primary_viewport_size} width
2. Test one-handed operation patterns:
   - Thumb reach zones for all interactive elements
   - {mobile_specific_features}
   - Touch targets (minimum 44x44px)
   - {mobile_ui_elements} positioning and accessibility

MOBILE-SPECIFIC VALIDATIONS:
- Touch interactions feel responsive and natural
- No accidental taps due to element proximity
- Content remains readable without horizontal scrolling
- {mobile_critical_features} work effectively in mobile layout
- All animations smooth at 60fps on mobile

DELIVERABLES:
- Mobile screenshot documentation
- Touch interaction performance report
- Recommendations for mobile UX improvements"
```

#### 5.4 Performance and Responsiveness Validation
**Validate against strict performance requirements:**

```bash
# Performance testing agent
claude "Create a Task agent for performance validation on {project_name}:

PERFORMANCE TESTING SCOPE:
1. Interaction Response Times:
   - {performance_critical_features}
   - All interactions must complete within {performance_requirement}
   - {performance_sensitive_operations} with immediate visual feedback

2. Data Volume Testing:
   - Test with {data_volume_requirement}
   - Verify smooth scrolling and rendering
   - Check memory usage patterns

3. Animation Performance:
   - Ensure 60fps for all transitions
   - No janky animations or stuttering
   - Smooth state changes

DELIVERABLES:
- Performance metrics for each interaction type
- Bottleneck identification
- Optimization recommendations if needed"
```

#### 5.5 Quality Gates Before PR
All UI changes must pass these criteria:
- [ ] Core user flows complete successfully on mobile and desktop
- [ ] All interactions respond within {performance_requirement}
- [ ] Mobile experience tested at {primary_viewport_size} viewport
- [ ] No accessibility issues identified
- [ ] Screenshots documented for key workflows
- [ ] Task agents report no blocking issues

## Development Workflow

### Git Workflow
1. **Create feature branch**: `git checkout -b {branch_pattern}/description`
2. **Regular commits**: Clear, descriptive commit messages
3. **Before PR**: Run all tests, lint, and Playwright validation
4. **PR process**: {pr_process}

### Testing Standards
- **Coverage requirement**: {coverage_requirement}
- **Test philosophy**: {test_philosophy}
- **Manual testing**: Always test features as a real user would
- **Playwright validation**: Required for all UI changes

### Code Quality
- **Style guide**: {style_guide}
- **Complexity**: Keep it simple, avoid over-engineering
- **Performance**: {performance_standards}
- **Documentation**: Clear comments explaining "why" not "what"

## Project-Specific Details

### File Structure
```
{file_structure}
```

### Key Components/Modules
{key_components}

### API/Service Integration
{api_integration_details}

### Environment Variables
{environment_variables}

### Deployment
{deployment_details}

## Quick Reference

### Common Commands
```bash
# Development
{dev_commands}

# Testing
{test_commands}

# Building
{build_commands}

# Deployment
{deploy_commands}
```

### Important Links
- **Repository**: {repository_url}
- **PRD**: `planning/prd.md`
- **Task Tracking**: {task_tracking_location}
- **Development Guidelines**: `development-guidelines.md`

### Key Principles
1. {principle_1}
2. {principle_2}
3. {principle_3}
4. {principle_4}
5. {principle_5}

### Troubleshooting
{common_issues_and_solutions}

---

**Remember**: 
- Follow the development guidelines strictly
- Test everything from a user's perspective
- Keep solutions simple and maintainable
- Always validate UI/UX with Playwright before PR
- When in doubt, refer to the PRD for project vision