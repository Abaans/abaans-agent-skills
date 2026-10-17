---
name: live-word-text-update
description: "Update text in an existing shared OneDrive or SharePoint Word document while preserving its file identity, revision history and embedded content. Use for scoped edits from a revised draft, including documents with active collaborators."
---

# Live Word text update

Edit the existing shared Word item in place. Preserve its canonical URL, title, sharing and protected content. A local preview is not evidence that the cloud document saved.

## Inputs and tools

Resolve the revised source, exact live destination and intended changes. Similar filenames are not sufficient identity evidence. A request to prepare a draft or demonstrate this skill does not authorize a live edit.

Prefer a dedicated tool that can edit bounded ranges in the existing Word item while preserving surrounding objects and collaboration state. Uploading a replacement binary, delete/recreate or Save As over the live path does not meet this contract. Google Docs editing is not a substitute for Word editing.

The documented UI route uses Microsoft Word on macOS plus the canonical OneDrive/SharePoint browser item. Use fresh accessibility/UI state and current tool documentation; never replay screen coordinates. A different tool/platform must satisfy the same preservation checks. If range editing is unavailable, provide a change map and report the blocker.

## Prepare the change map

1. Open source and destination. Verify the live cloud identity, meaningful title and saved/sync state. Record only the baseline needed for verification: revision-history rows, affected sections, embeds and their anchors, relevant headers/footers, comments and tracked changes.
2. Map source text to destination headings, paragraphs and table cells. Preserve a meaningful live title when the draft has a generic one. Reconcile explicitly requested version/date changes; do not restore stale metadata by default.
3. Preserve existing revision-history rows and their approval fields. Append supported new entries only once. A historical approval does not approve this revision.
4. Keep images, diagrams, embedded objects and captions in place unless the user specifically asked to change them. Use a permitted recovery snapshot when needed; keep private content out of reusable examples and logs.

## Edit bounded ranges

Verify the active document and selection before each edit. Update only the intended paragraph, section or cell, with formatting appropriate to its destination. Edit text around an embed as separate ranges rather than selecting across the object. Do not flatten tables or use blind whole-document Select All and paste.

Immediately before changing a range, recheck it for concurrent edits. Reconcile changes only within the authorized scope. If a collaborator's new text creates an unresolved conflict, leave that range intact and ask for the decision. Continue independent ranges only when safe.

Inspect each edit. On an unexpected paste, undo only the agent's identifiable edit when safe, then reassess. Do not retry a whole-document replacement from a stale snapshot.

## Verify persistence

Compare the final document against the change map and baseline: intended text, title, all historical rows, inventoried embeds, tables, headers/footers and relevant comment/tracked-change state. Inspect affected pages for clipping or displaced objects.

Wait for saved/synced status, then reopen or refresh the same canonical cloud item. Confirm the edited text persisted, protected content remains and the item identity/link is unchanged. If remote verification is unavailable, report **edited; cloud persistence unverified**.

Report the changed sections, preservation checks and persistence result. Do not claim that every collaborator's open copy refreshed. Keep any project evidence limited to what the user authorized.

See [change-map example and review cases](references/examples.md). End-to-end cloud editing requires an authorized live environment; package checks alone do not prove it.
