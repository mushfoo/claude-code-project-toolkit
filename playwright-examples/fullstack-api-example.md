# Full-Stack API + Frontend Playwright Testing Example

This example shows how to customize the Playwright testing templates for a full-stack project with a backend API and frontend application.

## Parameterized Development Guidelines Section

```markdown
## UI/UX Testing with Playwright

### 🎭 **Browser-Based User Experience Testing**

While unit tests verify code behavior, Playwright tests validate actual user experience in real browsers. Use Playwright to ensure the UI works as intended across different devices and interaction patterns.

### **When to Use Playwright Testing**
- **Before PR Creation**: Test core user flows on mobile (375px) and desktop viewports
- **After Major UI Changes**: Verify interactions still meet <100ms response requirement
- **API Integration Changes**: Validate frontend handles API responses correctly
- **Mobile-First Validation**: Confirm touch targets, one-handed operation, responsive behavior
- **Performance Validation**: Ensure UI interactions meet the <100ms standard in actual browsers

### **Required Test Scenarios for Task Management System**
- **Authentication Flow**: Login → MFA verification → dashboard access → logout
- **Task CRUD Operations**: Create task → edit details → assign users → complete → delete
- **API Error Handling**: Network failures → validation errors → rate limiting → timeouts
- **Offline Functionality**: Work offline → queue changes → sync when online
- **Collaboration Features**: Real-time updates → notifications → comments → mentions
- **Data Synchronization**: Verify frontend state matches backend after all operations

### **Playwright Testing Commands**
```bash
# Start backend API server
npm run server:dev

# Start frontend development server
npm run client:dev

# In another terminal, delegate UI/UX testing to a sub-agent
claude "Create a Task agent to test the core user flows with Playwright at localhost:3000. 
The agent should:
1. Navigate to the app and test full authentication flow
2. Test CRUD operations with API validation
3. Verify mobile responsiveness at 375px
4. Test API error scenarios and recovery
5. Validate offline functionality
6. Report findings and any UX issues discovered"
```

### **Full-Stack-Specific Testing Considerations**
- **API Response Handling**: Verify frontend gracefully handles all API states
- **Authentication State**: Test token refresh, session timeout, role changes
- **Data Consistency**: Ensure frontend cache stays in sync with backend
- **WebSocket Connections**: Validate real-time features remain stable
- **CORS and Security**: Test cross-origin requests work correctly
- **API Versioning**: Ensure frontend handles API version mismatches
```

## Parameterized Onboarding Prompt Section

```markdown
### Step 5: UI/UX Validation with Playwright
**Critical validation step using Task agents for systematic testing before PR creation.**

#### 5.1 Setup and Environment
1. **Start Backend Server**: `npm run server:dev` (localhost:4000)
2. **Start Frontend Server**: `npm run client:dev` (localhost:3000)
3. **Verify Test Environment**: Ensure API and frontend are connected

#### 5.2 Core User Experience Validation
Delegate comprehensive testing to Task agents for systematic coverage:

```bash
# Primary user flow testing
claude "Create a Task agent to comprehensively test Task Management System at localhost:3000:

CORE WORKFLOWS TO TEST:
1. Complete authentication flow (login → MFA → access)
2. Task lifecycle (create → assign → update → complete)
3. Collaboration features (comments, mentions, notifications)
4. API error recovery (network failures, validation errors)
5. Offline mode (work offline → sync when reconnected)

VALIDATION REQUIREMENTS:
- Take screenshots at each major step
- Test with realistic data (50+ tasks, 10+ users)
- Verify all interactive elements respond within 100ms
- Test API error scenarios systematically
- Validate data consistency between frontend and backend
- Document any broken workflows or sync issues"
```

#### 5.3 Mobile-First Testing (375px Viewport)
**Primary testing target - mobile experience is critical:**

```bash
# Mobile-first validation agent
claude "Create a Task agent for mobile UX testing on Task Management System:

MOBILE TESTING PROTOCOL:
1. Set viewport to 375px width (iPhone SE standard)
2. Test one-handed operation patterns:
   - Task creation with mobile keyboard
   - Swipe gestures for task actions
   - Touch targets for all interactive elements
   - Mobile-optimized forms and inputs

MOBILE-SPECIFIC VALIDATIONS:
- Authentication works with mobile password managers
- Task cards are readable and actionable
- Offline mode indicators are visible
- Sync status is clear on mobile
- Touch gestures feel natural
- Forms adapt to mobile keyboard

DELIVERABLES:
- Mobile screenshot documentation
- Touch interaction performance report
- Offline functionality assessment
- Mobile-specific bug report"
```

#### 5.4 API Integration and Performance Validation
**Validate frontend-backend integration:**

```bash
# API integration testing agent
claude "Create a Task agent for API integration validation:

API TESTING SCOPE:
1. Authentication Flow:
   - Login response handling < 500ms
   - Token refresh works seamlessly
   - Logout clears all frontend state
   
2. CRUD Operations:
   - Create task API call < 200ms
   - Update operations are optimistic
   - Delete confirmations prevent data loss
   
3. Error Scenarios:
   - Network timeout handling (30s)
   - 400/500 error recovery flows
   - Rate limit (429) user feedback
   - Validation error display
   
4. Real-time Features:
   - WebSocket connection stability
   - Message delivery < 1s
   - Reconnection after disconnect
   - State sync after reconnection

DELIVERABLES:
- API response time analysis
- Error handling documentation
- WebSocket stability report
- Frontend-backend sync validation"
```
```

## Key Customizations for Full-Stack Projects

1. **Dual Server Setup**: Backend API (port 4000) + Frontend (port 3000)
2. **API Integration Focus**: Test all frontend-backend interactions
3. **Error Scenario Coverage**: Network, validation, auth errors
4. **Offline Functionality**: Progressive enhancement testing
5. **State Management**: Frontend cache vs backend truth
6. **Security Testing**: Authentication, authorization, CORS

## Testing Checklist

- [ ] Frontend handles all API response types gracefully
- [ ] Authentication flow works end-to-end
- [ ] Offline mode queues changes correctly
- [ ] Real-time updates work via WebSocket
- [ ] Mobile experience matches desktop functionality
- [ ] Performance meets requirements with API latency
- [ ] Error messages help users recover