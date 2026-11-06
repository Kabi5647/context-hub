# Workflow and verification

## Demonstration sequence

1. Open a synthetic encounter, draft or enter notes, and have the clinician review the source.
2. The clinician selects Prepare discharge. Generate instructions, then run the independent verifier on both documents.
3. Surface omissions, changed instructions, unsupported additions and ambiguous text with evidence where available.
4. Review or correct discrepancies. Edits rerun verification and invalidate stale approval. After final clinician approval, show patient-facing instructions and print preview.

## Scope and maintenance

- The local prototype uses deterministic generation and bounded extraction. Unrecognized text and ambiguous changes require human review. A passing comparison covers only the checks the verifier can perform.
- For speech testing, use only fictional conversations with consent. Browser-service recognition may send audio to the browser provider. On-device-only mode must avoid silent cloud fallback.
- Keep the local prototype evidence separate from any hosted build. Use the source repository linked in the [project brief](../BRIEF.md#code-repository). Request working-document access from the owner. Use the dated category logs for workflow, clinical safety/testing, security, data, deployment and competition updates.
