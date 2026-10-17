# Live Word text update

![Live Word text update: shared Word document updates in OneDrive or SharePoint](assets/live-word-text-update.jpg)

Edit text in a shared Microsoft Word document while preserving its file identity, revision history and embedded content.

## Use it in Codex

```text
Use $live-word-text-update to apply this revised eligibility paragraph to the specified shared Word document. Preserve its title, revision history and adjacent diagram.
```

A report of the edited ranges and preservation checks, plus the verified cloud-save result or an explicit persistence gap.

## Requirements

- Access to the exact Word source and shared destination.
- Bounded editing tools and the ability to reopen the canonical cloud item.

## Install

Copy this complete `live-word-text-update` folder into your Codex skills directory. Keep its references and license together. The [repository installation guide](https://github.com/Abaans/abaans-agent-skills#install-in-codex) includes a copy command that refuses to replace an existing installation.

Read the [skill instructions](SKILL.md) and [examples](references/examples.md) before running the workflow.

## Verification

Packaging and isolated-copy tests pass. Live-account execution needs its own scoped test; package checks do not certify Word, Figma, Jira or image-generation results.

[MIT license](LICENSE). By [Abaan](https://github.com/Abaans).
