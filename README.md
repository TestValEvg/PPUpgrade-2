# PPUpgrade-2

Test automation suite for Navigator and Crypto features using Playwright.

## Structure

- **PPUpgradeTests/Tests/** - Test spec files
  - navigator.filters.spec.ts - Navigator filter validation tests
  - navigator.general-suppressed-rule.spec.ts - Navigator general suppression rule tests  
  - crypto.*.spec.ts - Crypto feature tests

- **PPUpgradeTests/Pages/** - Page Object Models
- **PPUpgradeTests/Utilits/** - Selectors and utilities
- **features/** - BDD feature files

## Setup

1. Install dependencies:
   ```
   npm install
   ```

2. Install Playwright browsers:
   ```
   npx playwright install chromium
   ```

3. Configure environment:
   - Copy .env.example to .env
   - Update credentials in .env file

## Run Tests

Run all tests:
```
npx playwright test
```

Run specific test file:
```
npx playwright test PPUpgradeTests/Tests/navigator.filters.spec.ts
```

Run in Chrome only:
```
npx playwright test --project=chromium
```
