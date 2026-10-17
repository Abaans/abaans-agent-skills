# Verification

Release: **0.1.0**. Checked locally on **18 October 2026**, on macOS.

## Automated checks

- Seven packaging tests pass: repository validation, isolated installation of every skill into a path containing spaces, missing-reference rejection, out-of-package-reference rejection, symlink rejection, malformed-metadata rejection, and the exact README installation recipe with existing-installation protection.
- Each installed skill carries its own MIT license, matching name, discovery metadata and bundled references.
- The Codex skill-creator validator accepts each `SKILL.md`.
- The final ZIP is reopened, CRC-checked, compared byte-for-byte with the source tree, extracted to a temporary directory and tested there again. Archive hashes and the owner's review notes are kept outside the published source tree.

The included GitHub Actions workflow runs the packaging suite and validator. Its checkout action is pinned; it needs read-only repository access and no account credentials. The [GitHub Actions tab](https://github.com/Abaans/abaans-agent-skills/actions) records the remote run for each published commit.

## What the checks do not prove

Structural tests check packaging and installation. They do not run an agent against the prose, measure trigger quality, or certify every instruction. The example prompts are manual review cases, not automated behavioral evaluations.

The four workflows were reviewed for stage scope, preservation requirements, fictional examples and capability limits. This candidate has not executed live image generation, font installation, Figma rendering, Word cloud editing/export or Jira attachment workflows. Those need a separately authorized environment and output verification. No third-party font or client asset is bundled.
