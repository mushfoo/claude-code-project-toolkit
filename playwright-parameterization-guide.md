# Playwright UI/UX Testing Parameterization Guide

This guide explains how to customize the Playwright testing templates in the Claude Code Project Toolkit for your specific project needs.

## Overview

The Playwright testing integration uses a parameterization system with placeholders that should be replaced with project-specific values. These placeholders are enclosed in curly braces `{placeholder_name}` throughout the templates.

## Core Parameters

### Project Identity
- `{project_name}` - Your project's name (e.g., "Puka Reading Tracker", "E-Commerce Platform")
- `{project_description}` - Brief description of what your project does
- `{project_status}` - Current development status (e.g., "MVP Development", "Production", "Beta")
- `{current_phase}` - Active development phase (e.g., "Epic 2: Core Features", "Phase 1: Authentication")

### Viewport and Mobile Testing
- `{primary_viewport_size}` - Primary mobile viewport width (e.g., "375px" for iPhone SE, "390px" for iPhone 14)
- `{mobile_specific_features}` - Mobile-specific UI elements to test (e.g., "filter tabs", "hamburger menu", "swipe gestures")
- `{mobile_interactive_elements}` - Touch-interactive components (e.g., "progress sliders", "toggle switches", "date pickers")
- `{mobile_ui_elements}` - Mobile UI components (e.g., "floating action button", "bottom navigation", "pull-to-refresh")
- `{mobile_critical_features}` - Essential mobile functionality (e.g., "one-handed operation", "offline mode", "camera integration")

### Performance Requirements
- `{performance_requirement}` - Maximum response time for interactions (e.g., "<100ms", "<200ms", "<50ms")
- `{data_volume_requirement}` - Data volume for testing (e.g., "100+ items", "1000+ records", "50+ concurrent users")
- `{performance_critical_features}` - Features requiring performance validation (e.g., "search results", "real-time updates", "data filtering")
- `{performance_sensitive_operations}` - Operations needing optimization (e.g., "bulk updates", "image uploads", "report generation")

### User Flows and Testing
- `{core_user_flows}` - Formatted list of main user journeys to test
- `{core_user_flows_list}` - Numbered list of specific workflows
- `{primary_user_flow}` - Most important user journey (e.g., "add item → edit → complete workflow")
- `{primary_user_flow_steps}` - Detailed steps for the primary workflow

### Development Environment
- `{dev_server_command}` - Command to start development server (e.g., "npm run dev", "yarn start", "pnpm dev")
- `{dev_server_url}` - Local development URL (e.g., "localhost:5173", "localhost:3000", "127.0.0.1:8080")
- `{install_command}` - Package installation command (e.g., "npm install", "yarn", "pnpm install")
- `{test_command}` - Test execution command (e.g., "npm test", "yarn test:unit", "pnpm test")
- `{lint_command}` - Linting command (e.g., "npm run lint", "yarn lint:fix")
- `{build_commands}` - Build process commands
- `{deploy_commands}` - Deployment commands

### Framework-Specific Testing
- `{framework_specific_testing}` - Additional testing considerations for your framework:
  - React: "Test React hooks, context providers, and component lifecycle"
  - Vue: "Validate Vue reactivity, computed properties, and watchers"
  - Angular: "Check Angular services, observables, and change detection"
  - Next.js: "Test SSR/SSG behavior, API routes, and middleware"

### Repository and Workflow
- `{repository_url}` - Full GitHub/GitLab repository URL
- `{current_branch}` - Active development branch
- `{protected_branches}` - Branches that shouldn't receive direct commits (e.g., "main, production")
- `{branch_pattern}` - Branch naming convention (e.g., "feature/", "bugfix/", "hotfix/")
- `{pr_process}` - Pull request workflow description

### Testing Standards
- `{coverage_requirement}` - Code coverage target (e.g., ">90%", ">80%", "100% for critical paths")
- `{test_philosophy}` - Testing approach (e.g., "User-focused integration tests", "TDD", "BDD")
- `{style_guide}` - Code style reference (e.g., "Airbnb JavaScript", "Google TypeScript", "Custom ESLint config")
- `{performance_standards}` - Performance benchmarks and requirements

### Project Structure
- `{file_structure}` - Project directory structure diagram
- `{key_components}` - List of main components/modules
- `{api_integration_details}` - API endpoints and integration notes
- `{environment_variables}` - Required environment variables
- `{deployment_details}` - Deployment process and platforms

### Additional Context
- `{technology_stack}` - Complete technology stack listing
- `{architecture_overview}` - High-level architecture description
- `{target_users}` - Target user demographics and needs
- `{core_functionality}` - Main features and capabilities
- `{active_tasks}` - Current sprint tasks
- `{next_priorities}` - Upcoming development priorities
- `{current_focus}` - What's being worked on right now

### Documentation Locations
- `{ui_prototypes_location}` - Path to UI/UX designs (e.g., "planning/ui-prototypes/", "design/figma-exports/")
- `{task_tracking_location}` - Where tasks are tracked (e.g., "planning/task-breakdown.md", "GitHub Issues", "Jira board")

### Project Principles
- `{principle_1}` through `{principle_5}` - Core development principles (e.g., "Mobile-first design", "Performance over features", "Accessibility by default")

### Troubleshooting
- `{common_issues_and_solutions}` - Known issues and their solutions

## Example Parameterization

### For a React/Vite Project (like Puka):
```
{project_name} = "Puka Reading Tracker"
{primary_viewport_size} = "375px"
{performance_requirement} = "<100ms"
{dev_server_command} = "npm run dev"
{dev_server_url} = "localhost:5173"
{core_user_flows} = "- **Core User Flow**: Add book → update progress → filter by status → search
- **Progress Management**: Test +10%, +25%, Done ✓ buttons for responsiveness
- **Filter Functionality**: Verify All/Want to Read/Reading/Finished tabs work correctly"
```

### For a Next.js E-commerce Project:
```
{project_name} = "ShopFlow E-commerce"
{primary_viewport_size} = "390px"
{performance_requirement} = "<200ms"
{dev_server_command} = "npm run dev"
{dev_server_url} = "localhost:3000"
{core_user_flows} = "- **Shopping Flow**: Browse products → add to cart → checkout → payment
- **User Account**: Register → login → view orders → manage addresses
- **Product Search**: Search → filter → sort → view details"
```

### For a Vue.js Dashboard:
```
{project_name} = "Analytics Dashboard"
{primary_viewport_size} = "768px"
{performance_requirement} = "<150ms"
{dev_server_command} = "yarn serve"
{dev_server_url} = "localhost:8080"
{core_user_flows} = "- **Data Visualization**: Load dashboard → interact with charts → export data
- **Report Generation**: Select metrics → configure → generate → download
- **Real-time Updates**: Monitor live data → receive alerts → take actions"
```

## Usage Instructions

1. **Copy the templates** from the Claude Code Project Toolkit
2. **Search and replace** all placeholders with your project-specific values
3. **Remove any sections** that don't apply to your project
4. **Add framework-specific sections** as needed
5. **Save the customized files** in your project:
   - Development guidelines → `development-guidelines.md`
   - Onboarding prompt → `planning/onboarding-prompt.md`

## Best Practices

1. **Be Specific**: Replace placeholders with exact values, not generic descriptions
2. **Keep It Real**: Use actual user workflows from your PRD
3. **Measure First**: Set performance requirements based on actual user needs
4. **Mobile Priority**: Choose viewport size based on your target users' devices
5. **Iterate**: Update parameters as your project evolves

## Validation Checklist

After parameterization, verify:
- [ ] All placeholders have been replaced
- [ ] Commands work in your environment
- [ ] User flows match your PRD
- [ ] Performance requirements are measurable
- [ ] Mobile viewport matches target devices
- [ ] Framework-specific needs are addressed

## Common Mistakes to Avoid

1. **Leaving placeholders**: Search for `{` to ensure all are replaced
2. **Generic flows**: Use specific user journeys, not abstract ones
3. **Unrealistic performance**: Set achievable performance targets
4. **Wrong viewport**: Research your actual users' devices
5. **Missing context**: Include all project-specific requirements

## Framework-Specific Additions

### React Projects
Add testing for:
- Component state management
- Hook behavior
- Context providers
- Suspense boundaries

### Vue Projects
Add testing for:
- Vuex/Pinia store
- Component reactivity
- Computed properties
- Lifecycle hooks

### Angular Projects
Add testing for:
- Service injection
- RxJS observables
- Route guards
- Form validation

### Next.js Projects
Add testing for:
- SSR/SSG behavior
- API routes
- Dynamic imports
- Image optimization

## Getting Help

If you need help with parameterization:
1. Review your PRD for project-specific details
2. Check your existing development setup
3. Look at similar projects for examples
4. Test with minimal parameters first
5. Iterate based on actual testing results

Remember: The goal is to create a testing framework that ensures your users have a great experience with your specific application.