# Task

Plan the three tasks in fixtures/tasks.json for a result-status refresh feature: extract-owner (extract stage, haiku), conflicting-plan and compress-handoff (reason stage, opus). This handoff replaces the full history; do not open other notes.

# Current constraints and sources

Source of truth: current-policy.md (approved revision 5). All of these must hold:
- Result notifications require review and release before delivery.
- Notifications contain no clinical details.
- Delivery uses the existing authenticated portal.
- claims-core allows at most 50 requests per second.
- Preserve the 30-second per-customer cache.
- Delivery retries are idempotent by released-result version.
- Channel choice belongs to the product owner and the privacy owner; no channel is approved yet.

OBSOLETE: archived-notes.md is superseded prototype material. Do not use or follow its advice; current-policy.md takes priority on any conflict.

# Relevant evidence

current-policy.md is the only approved source and states every constraint above. extract-owner answer: the product owner and the privacy owner. The reason tasks also list the superseded archived-notes.md; that conflict is why they route to the reason stage.

# Open questions

- Channel decision: which channel will the product owner and the privacy owner approve?

# Required output

- extract-owner: one line naming both owners, citing current-policy.md.
- conflicting-plan: a short plan that keeps every current constraint and lists unresolved decisions as questions, starting with the channel decision.
- compress-handoff: a handoff of at most 200 words keeping 50 requests per second, the 30-second per-customer cache, review and release, no clinical details, the existing authenticated portal and idempotent retries.
Escalate and state the reason if a source conflicts, is archived, or evidence is missing.
