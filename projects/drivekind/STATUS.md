# Status — Drivekind — Driving Practice

**Updated** 2026-11-05

## Done

- Inspected the extracted Drivekind source export, including routing, authentication endpoints, storage and database migration files.
- Source documents a fictional map and routing engine, avoidance controls, alternative routes, local progress and a real-map beta adapter. A previous update reported build/type checks on the scroll landing page.
- Imported and verified the source on `main` in the private `driving-app` repository, renamed from `new-repo-1`. The import includes the app, route engine, authentication endpoints, schema, migrations and tests.

## Next

1. Clone the GitHub source and record a clean test, typecheck and build baseline.
2. Audit existing login/logout and storage before implementing the requested separation of authentication and practice history. Verify identity, persistence and logout in the browser.
3. Test demo loop time budgets, strict avoidances and preference explanations. Verify real-mode configuration separately if authorized.

## Blockers

- Account separation, hosted authentication, browser/device coverage and the real-map beta runtime are unverified.
