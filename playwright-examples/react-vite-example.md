# React/Vite Playwright Testing Example

This example shows how to customize the Playwright testing templates for a React/Vite project similar to Puka Reading Tracker.

## Parameterized Development Guidelines Section

```markdown
## UI/UX Testing with Playwright

### 🎭 **Browser-Based User Experience Testing**

While unit tests verify code behavior, Playwright tests validate actual user experience in real browsers. Use Playwright to ensure the UI works as intended across different devices and interaction patterns.

### **When to Use Playwright Testing**
- **Before PR Creation**: Test core user flows on mobile (375px) and desktop viewports
- **After Major UI Changes**: Verify interactions still meet <100ms response requirement
- **Epic/Feature Completion**: Validate acceptance criteria with real user journeys
- **Mobile-First Validation**: Confirm touch targets, one-handed operation, responsive behavior
- **Performance Validation**: Ensure UI interactions meet the <100ms standard in actual browsers

### **Required Test Scenarios for Puka Reading Tracker**
- **Core User Flow**: Add book → update progress → filter by status → search
- **Progress Management**: Test +10%, +25%, Done ✓ buttons for responsiveness
- **Filter Functionality**: Verify All/Want to Read/Reading/Finished tabs work correctly
- **Search Integration**: Confirm search works across different filter states
- **Mobile Viewport**: Test all interactions at 375px width (primary mobile target)
- **Toast Notifications**: Verify success/error messages appear and dismiss properly

### **Playwright Testing Commands**
```bash
# Start development server
npm run dev

# In another terminal, delegate UI/UX testing to a sub-agent
claude "Create a Task agent to test the core user flows with Playwright at localhost:5173. 
The agent should:
1. Navigate to the app and take screenshots
2. Test the add book → progress update → filter workflow
3. Verify mobile responsiveness at 375px
4. Validate performance of interactions (<100ms)
5. Report findings and any UX issues discovered"
```

### **React-Specific Testing Considerations**
- **Component State**: Verify React state updates reflect immediately in UI
- **Hook Behavior**: Test custom hooks work correctly during user interactions
- **Context Updates**: Ensure context changes propagate to all consuming components
- **Suspense Boundaries**: Validate loading states and error boundaries
- **React Router**: Test navigation maintains state and handles deep links
```

## Parameterized Onboarding Prompt Section

```markdown
### Step 5: UI/UX Validation with Playwright
**Critical validation step using Task agents for systematic testing before PR creation.**

#### 5.1 Setup and Environment
1. **Start Development Server**: `npm run dev` (localhost:5173)
2. **Verify Test Environment**: Ensure all implemented features are accessible

#### 5.2 Core User Experience Validation
Delegate comprehensive testing to Task agents for systematic coverage:

```bash
# Primary user flow testing
claude "Create a Task agent to comprehensively test Puka Reading Tracker at localhost:5173:

CORE WORKFLOWS TO TEST:
1. New user onboarding experience (empty state → first book)
2. Add book → set progress → update status workflow
3. Filter switching across all status types (Want to Read, Currently Reading, Finished)
4. Progress updates using inline sliders and quick action buttons
5. Search/filter combinations with live results

VALIDATION REQUIREMENTS:
- Take screenshots at each major step
- Test with realistic data (6+ books across different statuses)
- Verify all interactive elements respond within 100ms
- Document any broken workflows or UX friction points
- Report completion rates for each workflow"
```

#### 5.3 Mobile-First Testing (375px Viewport)
**Primary testing target - mobile experience is critical:**

```bash
# Mobile-first validation agent
claude "Create a Task agent for mobile UX testing on Puka Reading Tracker:

MOBILE TESTING PROTOCOL:
1. Set viewport to 375px width (iPhone SE standard)
2. Test one-handed operation patterns:
   - Thumb reach zones for all interactive elements
   - Filter tabs accessibility with single thumb
   - Progress sliders touch targets (minimum 44x44px)
   - Floating action button positioning and accessibility

MOBILE-SPECIFIC VALIDATIONS:
- Touch interactions feel responsive and natural
- No accidental taps due to element proximity
- Content remains readable without horizontal scrolling
- Filter tabs work effectively in mobile layout
- Progress indicators visible and functional
- All animations smooth at 60fps on mobile

DELIVERABLES:
- Mobile screenshot documentation
- Touch interaction performance report
- Recommendations for mobile UX improvements"
```
```

## Key Customizations for React/Vite

1. **Performance Requirements**: Set to <100ms for snappy interactions
2. **Mobile Viewport**: 375px (iPhone SE) as primary target
3. **Development Server**: Vite's default `npm run dev` on port 5173
4. **State Management**: Focus on React hooks and context
5. **Build Tool**: Vite-specific optimizations and HMR testing

## Testing Checklist

- [ ] React components render correctly
- [ ] State updates trigger immediate UI changes
- [ ] Vite HMR doesn't break functionality
- [ ] Mobile gestures work with React event handlers
- [ ] Performance meets <100ms requirement with React's virtual DOM