# Vue.js Analytics Dashboard Playwright Testing Example

This example shows how to customize the Playwright testing templates for a Vue.js analytics dashboard project.

## Parameterized Development Guidelines Section

```markdown
## UI/UX Testing with Playwright

### 🎭 **Browser-Based User Experience Testing**

While unit tests verify code behavior, Playwright tests validate actual user experience in real browsers. Use Playwright to ensure the UI works as intended across different devices and interaction patterns.

### **When to Use Playwright Testing**
- **Before PR Creation**: Test core user flows on tablet (768px) and desktop viewports
- **After Major UI Changes**: Verify interactions still meet <150ms response requirement
- **Epic/Feature Completion**: Validate acceptance criteria with real user journeys
- **Responsive Validation**: Confirm dashboard adapts from tablet to desktop layouts
- **Performance Validation**: Ensure UI interactions meet the <150ms standard in actual browsers

### **Required Test Scenarios for Analytics Dashboard**
- **Data Visualization**: Load dashboard → interact with charts → drill down → export data
- **Report Generation**: Select metrics → configure parameters → generate → download PDF/Excel
- **Real-time Updates**: Monitor live data → receive alerts → acknowledge → take actions
- **Dashboard Customization**: Add/remove widgets → resize → save layout → share dashboard
- **Data Filtering**: Date range selection → filter by categories → apply multiple filters
- **User Permissions**: Test role-based access → verify data visibility → audit trail

### **Playwright Testing Commands**
```bash
# Start development server
yarn serve

# In another terminal, delegate UI/UX testing to a sub-agent
claude "Create a Task agent to test the core user flows with Playwright at localhost:8080. 
The agent should:
1. Navigate to the app and take screenshots
2. Test the dashboard interaction and data visualization workflows
3. Verify tablet responsiveness at 768px
4. Validate performance of interactions (<150ms)
5. Report findings and any UX issues discovered"
```

### **Vue.js-Specific Testing Considerations**
- **Reactivity System**: Verify Vue's reactive data updates reflect in charts immediately
- **Computed Properties**: Test complex calculations update when dependencies change
- **Vuex/Pinia Store**: Ensure state management handles real-time data correctly
- **Component Communication**: Validate event emission and prop updates
- **Transition Effects**: Test Vue transitions don't impact performance
- **Async Components**: Verify lazy-loaded dashboard widgets load smoothly
```

## Parameterized Onboarding Prompt Section

```markdown
### Step 5: UI/UX Validation with Playwright
**Critical validation step using Task agents for systematic testing before PR creation.**

#### 5.1 Setup and Environment
1. **Start Development Server**: `yarn serve` (localhost:8080)
2. **Verify Test Environment**: Ensure all implemented features are accessible

#### 5.2 Core User Experience Validation
Delegate comprehensive testing to Task agents for systematic coverage:

```bash
# Primary user flow testing
claude "Create a Task agent to comprehensively test Analytics Dashboard at localhost:8080:

CORE WORKFLOWS TO TEST:
1. Dashboard loading with default widgets and data
2. Chart interactions (zoom, pan, hover tooltips, click-through)
3. Report generation workflow (select data → configure → export)
4. Real-time data updates and notifications
5. Dashboard customization and layout persistence

VALIDATION REQUIREMENTS:
- Take screenshots at each major step
- Test with realistic data (1000+ data points, multiple metrics)
- Verify all interactive elements respond within 150ms
- Test chart rendering performance with large datasets
- Document any broken workflows or UX friction points
- Validate data accuracy in visualizations"
```

#### 5.3 Tablet-First Testing (768px Viewport)
**Primary testing target - tablet usage is common for dashboards:**

```bash
# Tablet-first validation agent
claude "Create a Task agent for tablet UX testing on Analytics Dashboard:

TABLET TESTING PROTOCOL:
1. Set viewport to 768px width (iPad Mini standard)
2. Test touch interactions:
   - Chart touch gestures (pinch zoom, swipe)
   - Widget drag-and-drop rearrangement
   - Date picker and filter controls
   - Tooltip positioning on touch

TABLET-SPECIFIC VALIDATIONS:
- Dashboard grid adapts to tablet layout
- Charts remain readable at tablet size
- Touch targets meet 44x44px minimum
- Modals and overlays work on tablet
- Performance remains smooth with touch interactions
- Export functions work on tablet browsers

DELIVERABLES:
- Tablet screenshot documentation
- Touch interaction performance report
- Dashboard usability assessment
- Recommendations for tablet optimization"
```

#### 5.4 Performance and Real-time Data Validation
**Validate against analytics dashboard requirements:**

```bash
# Performance testing agent
claude "Create a Task agent for performance validation on Analytics Dashboard:

PERFORMANCE TESTING SCOPE:
1. Initial Load Performance:
   - Dashboard loads under 3s with all widgets
   - Individual charts render < 500ms
   - Lazy-loaded widgets appear smoothly
   
2. Interaction Response Times:
   - Chart updates on filter change < 150ms
   - Drill-down navigation < 200ms
   - Export generation starts < 1s
   
3. Real-time Data Testing:
   - WebSocket connections remain stable
   - Updates reflect within 1s of data change
   - Memory usage stays constant over time
   - Handle 100+ concurrent data updates

DELIVERABLES:
- Performance metrics for each interaction
- Memory usage analysis over 30 minutes
- WebSocket stability report
- Optimization recommendations"
```
```

## Key Customizations for Vue.js

1. **Performance Requirements**: <150ms for dashboard interactions
2. **Primary Viewport**: 768px (iPad Mini) for tablet-first approach
3. **Development Server**: Vue CLI's `yarn serve` on port 8080
4. **State Management**: Focus on Vuex/Pinia real-time updates
5. **Reactivity**: Test Vue's reactivity with large datasets
6. **Component Architecture**: Validate widget-based dashboard system

## Testing Checklist

- [ ] Vue components update reactively with data changes
- [ ] Computed properties recalculate efficiently
- [ ] Charts render smoothly with 1000+ data points
- [ ] Real-time updates don't cause performance degradation
- [ ] Tablet touch interactions work flawlessly
- [ ] Export functionality generates accurate reports