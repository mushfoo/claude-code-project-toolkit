# Playwright Testing Examples

This directory contains framework-specific examples showing how to customize the Playwright UI/UX testing templates for different types of projects.

## Available Examples

### 1. [React/Vite Example](./react-vite-example.md)
- **Project Type**: Reading tracker application (like Puka)
- **Key Features**: Mobile-first, state management, quick interactions
- **Performance Target**: <100ms response time
- **Primary Viewport**: 375px (iPhone SE)

### 2. [Next.js Example](./nextjs-example.md)
- **Project Type**: E-commerce platform
- **Key Features**: SSR/SSG, API routes, shopping cart, payments
- **Performance Target**: <200ms response time
- **Primary Viewport**: 390px (iPhone 14)

### 3. [Vue.js Example](./vuejs-example.md)
- **Project Type**: Analytics dashboard
- **Key Features**: Data visualization, real-time updates, reporting
- **Performance Target**: <150ms response time
- **Primary Viewport**: 768px (iPad Mini)

### 4. [Full-Stack API Example](./fullstack-api-example.md)
- **Project Type**: Task management system with API backend
- **Key Features**: Authentication, CRUD operations, offline mode, real-time collaboration
- **Performance Target**: <100ms frontend, <500ms API
- **Primary Viewport**: 375px (iPhone SE)

## How to Use These Examples

1. **Choose the example** that most closely matches your project type
2. **Copy the relevant sections** into your project
3. **Replace the example values** with your project-specific details
4. **Customize further** based on your unique requirements
5. **Remove sections** that don't apply to your project

## Common Patterns Across Examples

### Task Agent Delegation
All examples emphasize using Claude's Task agents for systematic testing rather than manual processes.

### Mobile-First Approach
Each example prioritizes mobile testing with specific viewport sizes based on target users.

### Performance Requirements
Every example includes measurable performance targets appropriate to the project type.

### Quality Gates
All examples enforce testing requirements before PR creation.

### Framework-Specific Considerations
Each example includes testing considerations unique to that framework.

## Customization Tips

1. **Viewport Selection**: Choose based on your analytics data of actual user devices
2. **Performance Targets**: Set based on user research and competitive analysis
3. **User Flows**: Define based on your PRD and user stories
4. **Data Volumes**: Use realistic amounts that match production usage
5. **Error Scenarios**: Include your API's specific error responses

## Getting Started

1. Review the [Parameterization Guide](../playwright-parameterization-guide.md)
2. Choose the most relevant example
3. Copy sections into your project's documentation
4. Customize with your project-specific values
5. Test the commands and agent prompts
6. Iterate based on testing results

Remember: These are starting points. Your project's specific needs should drive the final testing approach.