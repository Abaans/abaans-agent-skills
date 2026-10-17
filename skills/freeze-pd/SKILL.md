---
name: freeze-pd
description: "Freeze a Product Document as a dated PDF from its latest saved Word version, review outstanding feedback, and attach the verified snapshot to a specified Jira issue when requested. A freeze records a revision; it does not grant approval."
---

# Freeze a Product Document

Create a dated PDF snapshot of a Product Document (PD) from its canonical saved Word item. Freezing does not imply stakeholder approval, completed testing or a deployed product.

## Resolve the requested result

Identify the exact live Word document, revision and output destination. When a Jira attachment is requested, verify the issue key and document relationship. A local-export-only request stops at the verified PDF. Preparing or demonstrating this skill does not authorize a live freeze.

The workflow needs access to the live Word item and Word's PDF export. Attaching to Jira also needs an authorized upload route and a way to reopen or retrieve the attachment. Report unavailable capabilities rather than reconstructing the document in another renderer or claiming an upload occurred.

## Review before freezing

Review open document comments and relevant current issue feedback. Compare each request with the body. Make only bounded corrections supported by explicit owner decisions or accepted feedback. Leave unresolved product, commercial or approval choices open; do not invent an answer to make the freeze appear complete.

Resolve a comment only when its requirement is addressed and comment resolution is within scope. Retain the discussion history. Check dates, limits, terms, requirement wording and embedded UI for contradictions that affect the requested revision. Report any material blocker before producing a supposedly final snapshot.

## Preserve the live source

Edit inside the existing Word item. Preserve its identity, shared URL, meaningful title, revision-history rows, embeds and relevant comments/tracked changes. Do not replace the cloud binary or recreate the item. If adding a revision row, use the actual date and supported version; do not carry a prior approval forward.

Reopen the same cloud item to verify any corrections saved. If feedback must be resolved first but persistence cannot be verified, the freeze remains incomplete.

## Export and verify

Use Word's PDF export. Normally exclude comment balloons and markup; honor a requested review copy. If tracked changes remain, establish which revision the export should represent without silently accepting or rejecting them.

Use a distinct dated/versioned filename and preserve earlier snapshots. Inspect the actual exported PDF for correct revision, complete sections, readable tables, preserved images, corrected text and clipped/missing content. A page-count change can be legitimate; investigate unexplained differences rather than requiring identical pagination.

If requested, attach that exact PDF to the verified Jira issue. Reopen or retrieve the attachment and verify filename, revision and content. Compare hashes when the original bytes can be retrieved unchanged. A completed file-picker interaction does not prove upload success. Do not change issue status unless requested.

## Report the achieved state

Return the local PDF or verified attachment link, revision/date, material corrections and remaining limits. Distinguish **exported locally**, **attached and verified**, and **blocked**.

Draft stakeholder wording only when requested. Sending or posting a message needs the user's communication scope and the host's rules; attaching a PDF is not blanket messaging authority. Never report another person's approval without evidence.

See [example request and review cases](references/examples.md).
