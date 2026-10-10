# SwimSwam status

Updated: 2026-10-10

## Current stage

Requirements discovery. The coach has described the intended workflow, and the existing plans in `swimming-training-plans.md` have been read. Website implementation has not started.

## Confirmed decisions

- The website is for the owner to use as a swimming coach.
- A plan represents a single swimming session that builds on previous sessions.
- The current workflow starts with a previous week's plan, modifies it, and copies exercises or sets from other weeks.
- Existing plans provide the reference for established formats and progression.
- The main difficulty is deciding how to combine exercises into a coherent session.
- Creating a session should happen mostly through dragging and dropping.
- Exercises and drills must be reusable while remaining adaptable and flexible.
- The website should calculate total swimming distance.
- The website should propose shorter and more beginner-friendly versions of a session.
- The finished session must be exportable as a PDF for printing.
- The resulting printed plans should look like the supplied PDF, stored at [`reference/My Simpass (1).pdf`](reference/My%20Simpass%20%281%29.pdf). This is the visual reference for PDF output.

## PDF layout reference

- The supplied PDF is committed unchanged for reference. `swimming-training-plans.md` remains the readable content reference.
- The reference has 18 portrait pages, each measuring 612 by 792 points, or US Letter.
- The layout uses black text on white, left-aligned exercise lines, bold plan headings and distance totals, and a dashed horizontal separator between longer and shorter plans.
- Longer and shorter plans are stacked vertically. Many pages repeat the pair further down the same sheet; page 7 contains one pair.
- Preserve the reference's compact, plain print style when implementing PDF output. Use the actual PDF to judge typography, spacing, wrapping, and placement.

## Observations from the existing document

These are source observations, not additional product decisions.

- The local document groups plans into 18 pages and preserves repeated plans and stated totals.
- Plans pair a longer session with a shorter session, generally starting with a warm-up and ending with a cool-down.
- Reusable material includes individual drills, drill sequences, and complete repeated sets.
- Notation includes repetitions, distances, component distances within a repetition, rest periods, technique instructions, and optional distance ranges.
- Later pages frequently use freestyle drill blocks that alternate drills with normal swimming, followed by a themed set or stroke sequence.
- Shorter plans sometimes reduce repetitions and distances, but also omit or replace exercises. A beginner-friendly version cannot always be produced by scaling distance alone.
- Many pages repeat the longer/shorter pair; the supplied PDF now establishes the desired print-layout reference.
- Page order is available, but session dates and chronological order have not been confirmed.

## Open questions

- How much help should the website provide in composing a coherent session beyond reusing and adapting existing material? Automatic suggestions or full-session generation have not been decided.
- Should the longer and shorter versions be edited together, and should changes to one suggest changes to the other?
- Should dragging and dropping support individual drills, entire sets, and components inside a set?
- Which swimmer abilities, session goals, pool lengths, equipment, and target distances should guide suggestions?
- How should previous sessions be dated and ordered so progression can be tracked?
- Where should plans be saved, and is access across devices needed?
- Website language and visual style have not been decided.

## Next step

Clarify the editor's behavior using concrete examples from the existing plans, then build an initial version around the agreed workflow and supplied PDF layout reference.
