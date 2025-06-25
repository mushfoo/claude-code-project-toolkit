# UI/UX Design Generator

Use this prompt to create functional UI prototypes from a completed PRD using Claude Code's design capabilities, with focus on the specific user flows documented in your PRD.

---

**PROMPT:**

You are a senior UX designer with expertise in user-centered design and rapid prototyping. Your goal is to translate the completed PRD into functional UI prototypes that demonstrate the specific user journeys documented in the PRD and validate how well different design approaches serve those flows.

## Input: Completed PRD

**PRD Document:**

```
[PASTE YOUR COMPLETED PRD HERE]
```

## Your Process

### Step 0: Adapt This Generator to Your Domain (Required - 15-30 minutes)

Generic UI patterns rarely capture domain-specific requirements effectively. Before proceeding, you must adapt this generator to your specific application domain.

#### Domain Adaptation Process

1. **Identify Your Domain's Key Elements**
   - What are the 3-5 most critical user actions in your domain?
   - What domain-specific UI patterns do users expect?
   - What performance constraints are non-negotiable?
   - What device/platform considerations are essential?

2. **Document Domain-Specific Requirements**
   - List the primary user flows unique to your domain
   - Note expected interaction patterns (e.g., swipe for dating apps, drag-drop for kanban)
   - Define performance benchmarks (e.g., sub-30s for reading trackers, sub-3s for e-commerce)
   - Identify domain conventions users will expect

3. **Customize Your Design Variations**
   Replace the generic design options in Step 4 with domain-specific approaches. For example:
   
   **Reading Tracker Domain:**
   - Option 1: Timer-focused (quick session logging)
   - Option 2: Progress-focused (visual achievement tracking)
   - Option 3: Social-focused (community reading features)
   
   **E-commerce Domain:**
   - Option 1: Browse-focused (discovery and exploration)
   - Option 2: Search-focused (quick find and purchase)
   - Option 3: Curated-focused (recommendations and collections)

4. **Save Your Adapted Version**
   - Create: `planning/ui-design-prompt.md`
   - Include all your domain customizations
   - Use this adapted version for generating prototypes

### Step 1: Extract & Map User Flows from PRD

Systematically analyze the PRD to identify:

#### Primary User Flows

For each user story/workflow in the PRD, extract:

- **Flow Name**: [Extract from user stories/acceptance criteria]
- **User Type**: [Which persona performs this flow]
- **Entry Point**: [How users discover and start this flow]
- **Success Criteria**: [What constitutes completion per PRD]
- **Steps**: [Detailed step-by-step breakdown from PRD]
- **Decision Points**: [Where users make choices or branch]
- **Error Scenarios**: [What can go wrong per PRD requirements]

#### Flow Complexity Analysis

- **Linear Flows**: Onboarding, checkout, setup wizards from PRD
- **Branching Flows**: Different paths based on user type/choices from PRD
- **Cyclical Flows**: Dashboard usage, content creation cycles from PRD
- **Exception Flows**: Error recovery, edge cases defined in PRD

#### Flow Interdependencies

- Which PRD flows connect to each other?
- Where do users transition between flows?
- What are the common entry/exit points defined in PRD?

### Step 2: Choose UI Approach Based on PRD Flow Types

Based on your flow analysis:

- **Linear Flow-Heavy PRD** → Wizard-style, step-by-step designs
- **Dashboard/Data-Heavy PRD** → Multi-panel, information-rich designs
- **Task-Switching PRD** → Contextual, flexible navigation designs
- **Mixed Flow PRD** → Progressive disclosure, adaptive designs

### Step 3: Create Boilerplate Setup for Flow-Based Testing

Generate the complete setup structure for flow validation:

```
planning/ui-prototypes/
├── README.md              # Flow testing guide and options comparison
├── assets/
│   ├── style.css          # Shared custom styles
│   └── script.js          # Flow interactions and state management
├── flows/
│   ├── [flow-name-1]/     # Complete flow demonstration
│   ├── [flow-name-2]/     # Complete flow demonstration
│   └── [flow-name-3]/     # Complete flow demonstration
├── options/
│   ├── option-1-flows.html # All PRD flows in Design Option 1
│   ├── option-2-flows.html # All PRD flows in Design Option 2
│   └── option-3-flows.html # All PRD flows in Design Option 3
└── [after selection]
    └── complete-prototype/ # Full prototype in selected style
        ├── [flow-pages]/
        └── [supporting-pages]/
```

### Step 4: Generate 3 Flow-Focused Design Approaches

Create **3 distinct approaches** for handling the PRD user flows:

#### Option 1: Step-by-Step Flow Design

- **File**: `options/option-1-flows.html`
- **Philosophy**: One clear action per screen, guided progression through PRD flows
- **Flow Treatment**: Wizard-style, progress indicators, linear progression
- **Page Structure**: Focused single-purpose pages for each flow step
- **Navigation**: Sequential with clear back/next, progress tracking
- **Best for**: Complex PRD flows, first-time users, high-stakes actions from PRD

#### Option 2: Contextual Flow Design

- **File**: `options/option-2-flows.html`
- **Philosophy**: Show context and options, let users choose their path through PRD flows
- **Flow Treatment**: Dashboard-style, multiple actions visible, flexible navigation
- **Page Structure**: Dense, multi-action pages that surface multiple PRD flows
- **Navigation**: Contextual menus, tabs, always-visible flow options
- **Best for**: Expert users from PRD, repeated tasks, efficiency-focused workflows

#### Option 3: Progressive Flow Design

- **File**: `options/option-3-flows.html`
- **Philosophy**: Start simple, reveal complexity as needed for PRD flows
- **Flow Treatment**: Expandable sections, in-place editing, contextual reveals
- **Page Structure**: Adaptive pages that grow based on user needs and PRD flow complexity
- **Navigation**: Smart defaults with progressive enhancement
- **Best for**: Mixed user types from PRD, learning workflows, scalable complexity

### Step 5: Generate Flow-Specific Pages for Each Option

For each user flow identified in the PRD, create pages covering:

#### Flow Entry Pages

- **Discovery/Landing**: How users find this flow (per PRD user journey)
- **Authentication Gates**: Login/signup if required by PRD
- **Context Setting**: Orientation for flow per PRD requirements

#### Flow Progress Pages

- **Data Collection**: Forms, inputs matching PRD data requirements
- **Decision Points**: Choice pages matching PRD business logic
- **Review/Confirmation**: Validation steps per PRD acceptance criteria
- **Processing States**: Loading, waiting states per PRD technical requirements

#### Flow Completion Pages

- **Success Confirmation**: Task completed per PRD success criteria
- **Next Steps**: Follow-up actions defined in PRD
- **Error Recovery**: Error handling per PRD error scenarios

### Step 6: Create PRD Flow Validation Framework

#### Flow Completion Testing

For each design option, create linked demonstrations of:

- **[Primary PRD Flow 1]**: Complete clickable walkthrough
- **[Primary PRD Flow 2]**: Complete clickable walkthrough
- **[Error Recovery Flow]**: How PRD error scenarios are handled
- **[Cross-Flow Navigation]**: Moving between PRD flows

#### User Story Validation

Map each PRD user story to specific UI elements:

- **As a [PRD user type]**: Which design persona does this serve?
- **I want to [PRD action]**: Is this action clearly available and intuitive?
- **So that [PRD benefit]**: Does the design deliver the intended value?

#### PRD Acceptance Criteria Check

- [ ] Each PRD acceptance criterion has corresponding UI element
- [ ] Error conditions from PRD are handled in design
- [ ] Success conditions are clearly communicated
- [ ] All PRD user inputs/outputs are accounted for

### Step 7: Generate PRD-Specific Realistic Content

Use actual PRD content, not generic placeholders:

- **Actual Data Fields**: Use field names and types from PRD
- **Business Domain**: Use terminology and concepts from PRD
- **User Roles**: Create realistic user personas from PRD
- **Workflow Context**: Use actual business scenarios described in PRD
- **Error Messages**: Use specific error conditions mentioned in PRD

### Step 8: Create Flow Performance Comparison

#### Selection Guide (`planning/ui-prototypes/README.md`):

```markdown
# PRD Flow-Based UI Design Options

## How to Review

1. Test each option by walking through the PRD flows
2. Complete the primary user journeys from our PRD
3. Try the error scenarios documented in our PRD
4. Consider which best serves our specific user types from PRD

## Flow Performance Comparison

### [Primary PRD Flow Name]

- **Option 1**: [Steps required, ease of completion, user type fit]
- **Option 2**: [Steps required, ease of completion, user type fit]
- **Option 3**: [Steps required, ease of completion, user type fit]

### [Secondary PRD Flow Name]

- **Option 1**: [Performance for this specific PRD flow]
- **Option 2**: [Performance for this specific PRD flow]
- **Option 3**: [Performance for this specific PRD flow]

## Selection Criteria Based on PRD

- **User Type Effectiveness**: Which option best serves [PRD User Type 1] vs [PRD User Type 2]?
- **Flow Efficiency**: Which reduces steps/effort for our most important PRD flows?
- **Error Prevention**: Which handles PRD edge cases most gracefully?
- **Business Goal Achievement**: Which best supports PRD business objectives?

## PRD Flow Testing Results

- **Task Completion**: Click count and page count for each PRD flow
- **Error Recovery**: How well each option handles PRD error scenarios
- **Cross-Flow Navigation**: Ease of moving between PRD workflows
- **User Type Fit**: Which PRD personas succeed with each option
```

### Step 9: Document PRD Flow Implementation

In each option file, add HTML comments explaining:

```html
<!-- 
OPTION [X]: [Name] - PRD Flow Implementation
PRD Flows Demonstrated:
- [Flow 1 from PRD]: [How this option handles it]
- [Flow 2 from PRD]: [How this option handles it]
- [Flow 3 from PRD]: [How this option handles it]

PRD User Type Fit:
- [User Type 1 from PRD]: [Strengths/weaknesses for this user type]
- [User Type 2 from PRD]: [Strengths/weaknesses for this user type]

PRD Requirements Coverage:
- [Requirement 1]: [How UI addresses this]
- [Requirement 2]: [How UI addresses this]

Trade-offs for Our PRD:
- Optimizes: [Which PRD flows/users this prioritizes]
- Sacrifices: [Which PRD flows/users this deprioritizes]
-->
```

## After Design Generation: PRD Flow-Driven Selection

### Selection Prompt:

```
I've tested the PRD flows in all three options:

**Flow Performance Results:**
- [Primary PRD Flow 1]: Option [X] was most efficient because...
- [Primary PRD Flow 2]: Option [Y] worked best for [PRD User Type] because...
- [Error Recovery]: Option [Z] handled PRD edge cases best because...

**Selected Option**: Option [X]
**Reason**: Best serves our [specific PRD user types] for [specific PRD flows]

**PRD-Specific Modifications needed**:
- Combine [specific element] from Option [Y] for [specific PRD flow step]
- Adjust [specific interaction] to better match [PRD requirement]
- Enhance [flow transition] to handle [PRD business rule]

Please create the complete prototype set optimized for our PRD flows with these modifications.
```

### Step 10: Update PRD with Flow-Validated UI/UX Specifications

Add comprehensive PRD flow implementation details:

```markdown
## UI/UX Specifications - PRD Flow Implementation

### PRD Flow Design Approach

- **Selected Design Pattern**: [Step-by-step/Contextual/Progressive based on testing]
- **Flow Optimization**: [Which PRD flows are prioritized and why]
- **User Type Priority**: [Which PRD user types are prioritized]

### PRD User Flow Implementation

1. **[PRD Flow 1 Name]**:

   - Pages: [List of pages in flow]
   - Key Interactions: [Critical UI interactions]
   - Success Criteria: [How completion is communicated]
   - Error Handling: [How PRD error scenarios are handled]

2. **[PRD Flow 2 Name]**:
   - [Same structure for each PRD flow]

### PRD Requirements Traceability

- [ ] [PRD Requirement 1]: Implemented via [UI elements]
- [ ] [PRD Requirement 2]: Implemented via [UI elements]
- [ ] [PRD User Story 1]: Validated through [design approach]
- [ ] [PRD User Story 2]: Validated through [design approach]

### Flow Performance Validation

- **Primary Flow Efficiency**: [Steps reduced, time saved vs baseline]
- **Error Prevention**: [How design prevents PRD-identified errors]
- **User Type Success**: [Validation that PRD user types can complete flows]
- **Cross-Flow Navigation**: [How users move between PRD workflows]

### Implementation Notes for PRD Flows

- **Critical Path Optimization**: [UI prioritization for most important PRD flows]
- **Progressive Enhancement**: [How complex PRD flows are made accessible]
- **State Management**: [How flow progress and context is maintained]
- **Responsive Considerations**: [How PRD flows work across devices]
```

## Platform-Specific Flow Considerations

### For Web Applications:

- **Multi-tab Flow Support**: How PRD flows work across browser tabs
- **Deep Linking**: URLs for specific points in PRD flows
- **Keyboard Navigation**: Tab order optimized for PRD flow efficiency

### For Mobile Applications:

- **Touch-Optimized Flows**: PRD flows adapted for thumb navigation
- **Flow State Preservation**: Handling app backgrounding during PRD flows
- **Gesture Integration**: Swipe patterns that support PRD flow progression

### For Responsive Applications:

- **Adaptive Flow Layouts**: How PRD flows change across screen sizes
- **Cross-Device Flow Continuity**: Starting flow on mobile, finishing on desktop

## Output Requirements

**Phase 1 - Generate PRD Flow Options**: `planning/ui-prototypes/`

- Create 3 flow-focused design options demonstrating all PRD user flows
- Include comprehensive flow performance comparison based on PRD requirements
- Provide PRD-specific selection criteria
- Document how each option serves different PRD user types and business goals

**Phase 2 - After PRD-Based Selection**: Complete prototype optimized for selected approach

- Expand chosen design into complete PRD flow implementations
- Update PRD with validated UI/UX specifications
- Create all necessary pages for PRD-documented user journeys

**Use git to track**: All prototype files and PRD updates for version control

## Instructions for Creation

### Phase 1: Generate PRD Flow-Based Options

1. **Extract all user flows from PRD** systematically
2. **Map PRD requirements to UI needs** (data inputs, business rules, user types)
3. **Create 3 approaches for handling PRD flows** with clear differentiation
4. **Generate working demonstrations** of each PRD flow in each option
5. **Test flow efficiency** and document performance for PRD-specific scenarios

### Phase 2: PRD Flow Optimization (After reviewing options)

1. **Validate flow performance** by testing all PRD user journeys
2. **Select optimal approach** based on PRD user types and business priorities
3. **Refine with PRD-specific modifications** to address any gaps
4. **Generate complete flow-optimized prototype**
5. **Update PRD comprehensively** with implementation-ready specifications

**Start by systematically extracting all user flows from the provided PRD, then generate the 3 flow-focused design options for testing and selection.**
