# Playwright-Typescript-Framework

A robust end-to-end testing framework using [Playwright](https://playwright.dev/) and [TypeScript](https://www.typescriptlang.org/).

## Features

- Cross-browser testing (Chromium, Firefox, WebKit)
- TypeScript support for type safety and autocompletion
- Automatic test reports (HTML, Allure, etc.)
- Parallel test execution
- Easy configuration and custom commands

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16+ recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation

```bash
npm install
# or
yarn install
```

### Running Tests

```bash
npx playwright test
```

### Generating Reports

- **Playwright HTML Report:**  
  ```bash
  npx playwright show-report
  ```
- **Allure Report:**  
  (If configured, generate with:)
  ```bash
  npx allure generate allure-results --clean -o allure-report
  npx allure open allure-report
  ```

### Folder Structure

```
.
├── tests/                # Test specs
├── playwright.config.ts  # Playwright configuration
├── test-results/         # Test result artifacts (gitignored)
├── playwright-report/    # HTML reports (gitignored)
├── node_modules/         # Dependencies (gitignored)
├── README.md             # Project documentation
└── ...
```

## Useful Commands

- Run specific test file:  
  `npx playwright test tests/example.spec.ts`
- Run tests in headed mode:  
  `npx playwright test --headed`
- Debug tests:  
  `npx playwright test --debug`

## Resources

- [Playwright Docs](https://playwright.dev/docs/intro)
- [TypeScript Docs](https://www.typescriptlang.org/docs/)

---

Feel free to contribute