# Routing and accounts

## Source map

- In the owner workspace named `new driver app`, use the `Drivekind` folder extracted from the source export. Start with its README and `EXPORT_NOTES.md`.
- Routing is in `lib/drivekind/engine.ts` and `app/api/routes/route.ts`. Check `lib/auth.ts`, `app/api/auth/`, `db/schema.ts`, and `drizzle/` for existing account scaffolding.
- Use the project's test, typecheck and build commands. Existing source and release reports do not establish the hosted account flow.

## Route behavior

- For practice loops, budget for the entire trip back to the start. Drive Somewhere has a one-way budget. Strict highway and exclusion rules must remain enforced when no candidate fits.
- Preference scores and difficulty labels are heuristics. Demo session totals stay separate from real practice totals.
- Demo Mode runs without a provider key. The optional real-map adapter has more limited capabilities. Confirm a supported feature before showing it and keep secrets server-side. The demo route and real-map planning flows are for use while parked.
