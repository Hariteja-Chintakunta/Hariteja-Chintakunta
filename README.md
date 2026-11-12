View my portfolio: https://hariteja-chintakunta.github.io/

*QA Engineer — PEGA & Appian Testing | Playwright • TypeScript • REST Assured**

> TEST REPORT — Profile under test: Hariteja · Status: Open to Work · Last updated: November 2026
>
> No badges. No contribution graphs. No "currently learning" list.
> The work is below. Run it.

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

## Known limitations — read this before you hire me

- I do **not** claim 3 years of production Playwright. My production experience is 12 years of QA, mostly PEGA and manual testing. My Playwright work is the capstone above — open it and run it.
- I have **not** shipped a production LLM evaluation harness. I test AI-assisted features with golden datasets and pass/flag decisions, and I use GenAI tools inside QA work.
- The REST Assured repo is a **starter** (3 tests). The full suite is in progress.

## How I work

- One test, one job. Every test sets up its own data and cleans up after itself.
- No `Thread.sleep`, no fixed waits. Auto-waiting and web-first assertions, or the test is wrong.
- A failure must explain itself: screenshot, trace, and a report — or it is not a finished test.
- If the page changes, one file changes. That is the whole point of the Page Object Model.

## Now building

- Playwright 20-hour hands-on plan — Hour 1 next (setup + first green run)
- REST Assured suite — Hours 1–2 packs written (JSONPlaceholder, specs, POJOs, schema checks), first laptop run pending
- TypeScript fluency sprint (10 hours)

## Contact

- LinkedIn: https://www.linkedin.com/in/chintakunta-hariteja/
- Email: haritejac@hotmail.com
- Location: Hyderabad | Remote

---
*12 years finding bugs in other people's software. Now I write the tests that find them automatically.*




Yes. The content is already strong, but it still reads slightly like a résumé. If your goal is to stand out against hundreds of LinkedIn profiles and make recruiters, hiring managers, and QA leads stop scrolling, make it more direct, evidence-driven, and unapologetically confident.

Hariteja Chintakunta
Senior QA Engineer | PEGA Specialist | Automation Engineer
12 Years Breaking Software Before Customers Do
PEGA • Playwright • TypeScript • Selenium • REST Assured • API Testing • Migration Testing

Most QA profiles tell you what they know.

This profile shows you what can be run, verified, and challenged.

12 years in Quality Assurance.

9+ years testing mission-critical PEGA applications across healthcare, insurance, banking, and fleet-management platforms.

Currently leading quality validation for a large-scale PEGA migration involving 18 applications, 8 production go-lives, AWS-to-PEGA Cloud transformation, and a team of 8 testers.

Every framework below is public.

Every claim can be executed.

Every failure can be reproduced
