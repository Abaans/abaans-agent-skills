# Example request and review cases

Use a fictional Product Document and a disposable issue when exercising external actions.

## Local snapshot

“Freeze the specified Product Overview, revision 0.4, as a dated PDF. Keep it local.”

Review relevant open feedback, verify the saved Word revision, export with Word, inspect the PDF and return its path. A suitable filename is `Product Overview - v0.4 - YYYY-MM-DD.pdf`, replacing the date with the actual freeze date. No Jira upload or message is implied.

## Verified attachment

“Freeze this saved revision and attach the verified PDF to the issue I specified. Do not change its status.”

Verify the exact issue, upload the inspected PDF, reopen or retrieve the actual attachment and report its link and revision. If upload succeeds but retrieval/inspection is unavailable, report attachment verification pending.

## Reviewer checks

- An unresolved price or eligibility decision remains a blocker; do not invent a value.
- Historical approved rows remain unchanged and do not approve the new revision.
- Tracked changes are present: establish the requested representation; do not silently accept all edits.
- An older PDF has the same filename: preserve it and choose a distinct versioned filename.
- An exported PDF has a missing diagram: fix or report the defect before claiming the freeze complete.

These cases require manual review or scoped live tests; the repository's structural checks cannot prove cloud persistence or an upload.
