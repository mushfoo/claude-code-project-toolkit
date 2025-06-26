# Next.js E-commerce Playwright Testing Example

This example shows how to customize the Playwright testing templates for a Next.js e-commerce project.

## Parameterized Development Guidelines Section

```markdown
## UI/UX Testing with Playwright

### 🎭 **Browser-Based User Experience Testing**

While unit tests verify code behavior, Playwright tests validate actual user experience in real browsers. Use Playwright to ensure the UI works as intended across different devices and interaction patterns.

### **When to Use Playwright Testing**
- **Before PR Creation**: Test core user flows on mobile (390px) and desktop viewports
- **After Major UI Changes**: Verify interactions still meet <200ms response requirement
- **Epic/Feature Completion**: Validate acceptance criteria with real user journeys
- **Mobile-First Validation**: Confirm touch targets, one-handed operation, responsive behavior
- **Performance Validation**: Ensure UI interactions meet the <200ms standard in actual browsers

### **Required Test Scenarios for ShopFlow E-commerce**
- **Shopping Flow**: Browse products → add to cart → checkout → payment confirmation
- **User Account**: Register → login → view orders → manage addresses → track shipments
- **Product Search**: Search → filter by category/price → sort → view details → read reviews
- **Cart Management**: Add items → update quantities → apply coupons → calculate shipping
- **Mobile Commerce**: Test swipe gestures, touch-optimized checkout, mobile payment methods
- **Performance**: Ensure product images lazy load, cart updates are instant, search is responsive

### **Playwright Testing Commands**
```bash
# Start development server
npm run dev

# In another terminal, delegate UI/UX testing to a sub-agent
claude "Create a Task agent to test the core user flows with Playwright at localhost:3000. 
The agent should:
1. Navigate to the app and take screenshots
2. Test the complete shopping flow from browse to checkout
3. Verify mobile responsiveness at 390px
4. Validate performance of interactions (<200ms)
5. Report findings and any UX issues discovered"
```

### **Next.js-Specific Testing Considerations**
- **SSR/SSG Validation**: Ensure server-rendered pages load with correct data
- **API Routes**: Test Next.js API endpoints integrate properly with UI
- **Dynamic Imports**: Verify code splitting doesn't break user flows
- **Image Optimization**: Validate Next.js Image component loads efficiently
- **Middleware**: Test authentication redirects and route protection
- **ISR Pages**: Ensure incremental static regeneration works correctly
```

## Parameterized Onboarding Prompt Section

```markdown
### Step 5: UI/UX Validation with Playwright
**Critical validation step using Task agents for systematic testing before PR creation.**

#### 5.1 Setup and Environment
1. **Start Development Server**: `npm run dev` (localhost:3000)
2. **Verify Test Environment**: Ensure all implemented features are accessible

#### 5.2 Core User Experience Validation
Delegate comprehensive testing to Task agents for systematic coverage:

```bash
# Primary user flow testing
claude "Create a Task agent to comprehensively test ShopFlow E-commerce at localhost:3000:

CORE WORKFLOWS TO TEST:
1. Guest checkout experience (browse → add to cart → checkout without account)
2. User registration and first purchase workflow
3. Product search with filters (category, price range, ratings)
4. Cart management (add, remove, update quantities, apply discounts)
5. Order tracking and history viewing

VALIDATION REQUIREMENTS:
- Take screenshots at each major step
- Test with realistic data (50+ products, multiple categories)
- Verify all interactive elements respond within 200ms
- Test payment form validation and error handling
- Document any broken workflows or UX friction points
- Report completion rates for each workflow"
```

#### 5.3 Mobile-First Testing (390px Viewport)
**Primary testing target - mobile commerce is critical:**

```bash
# Mobile-first validation agent
claude "Create a Task agent for mobile UX testing on ShopFlow E-commerce:

MOBILE TESTING PROTOCOL:
1. Set viewport to 390px width (iPhone 14 standard)
2. Test one-handed operation patterns:
   - Product browsing with thumb swipes
   - Add to cart button accessibility
   - Checkout form completion with mobile keyboard
   - Mobile payment method selection (Apple Pay, Google Pay)

MOBILE-SPECIFIC VALIDATIONS:
- Product images load efficiently on mobile
- Cart drawer/modal works on small screens
- Checkout form adapts to mobile keyboard
- Touch targets for size/color selection are adequate
- Mobile-specific features (camera for card scan) work
- All animations smooth at 60fps on mobile

DELIVERABLES:
- Mobile screenshot documentation
- Touch interaction performance report
- Mobile conversion funnel analysis
- Recommendations for mobile UX improvements"
```

#### 5.4 Performance and Responsiveness Validation
**Validate against e-commerce performance requirements:**

```bash
# Performance testing agent
claude "Create a Task agent for performance validation on ShopFlow E-commerce:

PERFORMANCE TESTING SCOPE:
1. Page Load Times:
   - Product listing pages under 2s
   - Product detail pages under 1.5s
   - Checkout pages under 1s
   
2. Interaction Response Times:
   - Add to cart animations < 200ms
   - Filter/sort updates < 300ms
   - Search suggestions < 150ms
   
3. Data Volume Testing:
   - Test with 100+ products in cart
   - Browse 1000+ product catalog
   - Handle multiple concurrent users

DELIVERABLES:
- Core Web Vitals report
- Time to Interactive metrics
- Recommendations for performance optimization"
```
```

## Key Customizations for Next.js

1. **Performance Requirements**: <200ms for e-commerce interactions
2. **Mobile Viewport**: 390px (iPhone 14) as primary target
3. **Development Server**: Next.js default on port 3000
4. **SSR Testing**: Validate server-side rendering behavior
5. **API Routes**: Test full-stack functionality
6. **Image Optimization**: Leverage Next.js Image component

## Testing Checklist

- [ ] SSR pages load with correct initial data
- [ ] Client-side navigation maintains state
- [ ] API routes handle errors gracefully
- [ ] Images lazy load using Next.js optimization
- [ ] Mobile checkout flow completes successfully
- [ ] Performance meets e-commerce standards