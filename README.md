View my portfolio: https://hariteja-chintakunta.github.io/

# Hariteja Chintakunta

**Senior QA Engineer | Pega Specialist | Automation Engineer**

**12 Years Breaking Software Before Customers Do**

Pega • Playwright • TypeScript • Selenium • REST Assured • API Testing • MCP • Migration Testing

Most QA profiles tell you what someone knows. This one shows you what can be run, verified, and challenged.

12 years in Quality Assurance.
9+ years testing mission-critical Pega applications across healthcare, insurance, banking, and fleet management.

Right now, I’m leading quality validation for a large-scale Pega migration: 18 applications, 8 production go-lives, an AWS-to-Pega Cloud transformation, and a team of 8 testers.

Alongside that, I’m building Playwright and REST API automation for my project. I’ve completed proofs of concept with both and am now exploring how MCP (Model Context Protocol) can connect AI tools to these test workflows.

Every framework in my repositories is public. Every claim can be executed. Every failure can be reproduced.

## Test summary

| Field | Result |
|---|---|
| Experience | 12 years in QA, 9+ years testing PEGA applications |
| Domains | Healthcare, insurance, banking, fleet management |
| Current role | Senior Technical Consultant, Perficient India (Jan 2026 – Present) |
| Current project | Healthfirst PEGA migration — 18 apps, AWS → PEGA Cloud, 4 months, 8 go-lives, team of 8 |
| Now building | Playwright + TypeScript, REST Assured + Java, Selenium + TestNG |
| Open to | Pega Tester · Pega Automation Engineer · Gen AI Tester — Hyderabad \| Remote · Immediate joiner |

## Coverage — what I test

- **PEGA & Appian (low-code)** — business rules, case flows, data, integrations, UAT, migration testing
- **Web UI** — Playwright + TypeScript, Selenium + Java
- **APIs** — REST Assured + Java, Postman
- **Migration** — functional parity, data integrity, regression across 18 applications
- **Accessibility & visual** — axe-core scans, screenshot baselines

## Evidence — the repos

### 1. [playwright-capstone](https://github.com/Hariteja-Chintakunta/playwright-capstone) — TypeScript + Playwright

E-commerce automation on AutomationExercise. 10 spec files, 9 page classes, custom fixtures, cross-browser (Chromium, Firefox, WebKit), axe-core accessibility scans, visual regression with baselines, network mocking, typed `.env` config. Covers login, registration, search, cart, checkout, invoice download, contact form.

Run it:

```bash
npm ci
npx playwright test
```

### 2. [Selenium-Capstone](https://github.com/Hariteja-Chintakunta/Selenium-Capstone) — Java + Selenium + TestNG

SauceDemo framework. 46 tests, 8 modules, 9 page classes, Page Object Model, explicit waits only, retry once, parallel 3 threads, Extent + Allure reports, 62 assertions.

Run it:

```bash
mvn clean test
```

Expect `Tests run: 46, Failures: 1`. The 1 failure is deliberate — see below.

### 3. [restassured-capstone](https://github.com/Hariteja-Chintakunta/restassured-capstone) — Java + REST Assured + TestNG

API starter suite: 3 tests — list posts, post details, search. Small on purpose; it is the base the bigger suite grows from.

Run it:

```bash
mvn test
```

## Defects found — the part most profiles hide

**The alwaysRun bug.** First run of the Selenium framework: 37 tests failed in 3 seconds with `NullPointerException`. Cause: TestNG silently skips inherited `@BeforeMethod` setup when `testng.xml` uses group filtering, so `setUp()` never ran. Fix: `alwaysRun = true` on the setup methods. Lesson: a framework bug looks exactly like 37 broken tests.

**The deliberate failure.** `LoginTest.validLoginRedirectsToDashboard` expects the title "Dashboard". The real title is "Products". I kept it failing on purpose — to show the screenshot, the report, and how a failure is explained instead of hidden.

## How I work

- One test, one job. Every test sets up its own data and cleans up after itself.
- No `Thread.sleep`, no fixed waits. Auto-waiting and web-first assertions, or the test is wrong.
- A failure must explain itself: screenshot, trace, and a report — or it is not a finished test.
- If the page changes, one file changes. That is the whole point of the Page Object Model.

## Contact

- LinkedIn: https://www.linkedin.com/in/chintakunta-hariteja/
- Email: haritejac@hotmail.com
- Location: Hyderabad | Remote

---
*12 years finding bugs in other people's software. Now I write the tests that find them automatically.*
