# Planner

## Planner flow

1. Let users enter known lengths, ask for measurement help or skip. Preserve an unknown value and request a measurement if a recommendation depends on it.
2. Support a small initial set of maintenance routines or style transitions, each with length ranges, required tools and illustrated steps for the top/front, sides and back.
3. Compare current lengths to target ranges, explain what to trim or grow, and let the user pause and resume a session.
4. Record the actual cut and feedback, then use measurement history for a growth range when enough data exists.

## Implementation notes

- Use structured templates and section-level rules. Computer vision was discussed as a future experiment. Hair segmentation alone does not provide reliable lengths.
- Keep photos and journal records in the product's intended data boundary. Ask the owner for access to the original source and preview package through the project workspace.
