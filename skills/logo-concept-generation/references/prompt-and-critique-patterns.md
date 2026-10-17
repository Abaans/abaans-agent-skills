# Prompt and Critique Patterns

Use these patterns after establishing the brand brief. Replace every placeholder with concrete visual instructions.

## Logo anatomy vocabulary

Use one primary term and define its mechanics:

- **Wordmark:** the brand name rendered as the primary mark.
- **Custom wordmark:** purpose-drawn lettering rather than an unchanged typeface.
- **Connected custom lettering:** neighboring glyphs join through named terminals, stems, crossbars, or shared strokes.
- **Lettermark:** a short abbreviation built from letters.
- **Monogram:** two or more initials combined into one compact symbol.
- **Emblem:** lettering contained within a badge, seal, or enclosing form.
- **Combination mark:** a symbol and wordmark designed to work together or separately.

Treat “typographic logo” as ambiguous until mapped to one of these structures.

## Search ladder

Build queries in this order and stop when new results stop adding useful attributes:

1. `<tone> <logo anatomy> brand identity`
2. `<brand category> <tone> logo design`
3. `<adjacent aspirational category> logo identity`
4. `<structural mechanism> custom lettering logo`
5. `<logo anatomy> black and white small-size application`

Example structural terms: connected wordmark, ligature logo, shared-stroke monogram, interlocking initials, continuous-line lettering, high-contrast custom serif, geometric letter construction.

For each selected reference, record:

| Field | Question |
|---|---|
| Source | Where is the reference, and who made it if known? |
| Learn | Which specific visual principle is useful? |
| Reject | Which feature would be clichéd, illegible, or off-brief? |
| Transfer | How can the principle become original geometry for this brand? |

Do not use “make it like this logo” as a transfer rule.

## Direction card template

```text
Direction: <short name>
Thesis: <one sentence>
Anatomy: <wordmark, connected lettering, monogram, etc.>
Mechanism: <specific shared strokes, ligatures, cuts, or proportions>
Learn from references: <attributes, not identities>
Exclude: <cliches, effects, or conflicting forms>
Risk: <legibility, similarity, complexity, or reproduction risk>
```

## Generation prompt template

```text
Create one original logo concept for the exact brand name "<EXACT NAME>".
Spell it exactly as written, with <capitalization and line-break instructions>.

Logo anatomy: <explicit structure>.
Letter construction: <named glyph relationships and connection mechanics>.
Visual character: <mood translated into contrast, proportions, spacing, terminals, and rhythm>.
Composition: <horizontal/stacked/compact, alignment, whitespace, symbol relationship>.
Rendering: flat vector-like graphic, crisp edges, no texture.
Color: solid black mark on a pure white background.

Avoid: <wrong anatomy>, generic stock-font treatment, unrelated icons, gradients,
shadows, bevels, mockups, illegible joins, extra letters, misspellings, and decorative
elements that do not serve the construction.

Show only the logo concept, centered with generous clear space.
```

For connected lettering, name the intended transitions. Example: “Extend the first letter's exit stroke into the next letter's vertical stem; keep counters open; do not turn the word into cursive script.”

Commit to one construction per prompt. Remove branching phrases such as “single- or double-storey,” “serif or sans,” and “connected or overlapping.” Verify that every term applies to the named glyph; do not invent anatomy merely to make a prompt sound specific.

## Refinement prompt template

```text
Refine the supplied logo concept; preserve its identity rather than restarting.

KEEP
- <successful anatomy, silhouette, spacing, or stroke behavior>

CHANGE
- <precise local geometry change>
- <one additional variable cluster if necessary>

AVOID
- <observed failure mode>
- <new elements, restyling, or text errors>

Maintain the exact spelling "<EXACT NAME>". Return a flat black logo on white with
no mockup, texture, shadow, or presentation scene.
```

Replace vague corrections such as “more premium” with visible deltas such as “reduce the stroke contrast slightly, lengthen the entry terminal, and increase the gap around the central ligature.”

## Critique rubric

Score each dimension from 1 to 5, then explain the lowest two scores first:

| Dimension | Test |
|---|---|
| Text fidelity | Is every letter present, ordered, and readable? |
| Brief fidelity | Does the concept use the requested anatomy and mechanics? |
| Legibility | Does it read quickly at full and small size? |
| Distinctiveness | Does the silhouette remain recognizable without effects? |
| Construction | Are joins, counters, spacing, and stroke transitions intentional? |
| Relevance | Does it fit the positioning without category clichés? |
| Originality | Is it visibly independent of the reference set? |
| Reproducibility | Can it survive monochrome, reverse color, and vector redraw? |

Use these outcomes:

- **Advance:** the construction is clear; prepare a vector redraw brief.
- **Refine:** the core idea works; issue one delta-based edit.
- **Retire:** the anatomy or originality is wrong; return to a different direction card.

## Vector handoff checklist

Before calling a concept production-ready, require:

- Manual vector reconstruction rather than automatic raster tracing alone
- Optical kerning and curve cleanup
- Consistent joins, counters, terminals, and overshoots
- Horizontal, stacked, icon, and reversed-color variants as needed
- Small-size, embroidery, engraving, and single-color tests where relevant
- Source-file packaging and a basic clear-space rule
- Appropriate name and trademark screening
