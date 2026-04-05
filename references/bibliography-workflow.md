# Bibliography workflow

Use this workflow whenever the user asks for the full article package or a citable final paper.

## Objective

Build a transparent bibliography that separates:
- works explicitly cited in the anchor report
- archive documents used as primary sources
- new secondary literature introduced by the article

## Source classes

Maintain three classes in the bibliography plan.

### A. Anchor report references
These are references already present in `Rapport-FEP-Graz`.
Use them to reconstruct the intellectual base of the original report.

### B. Archive primary sources
These are BFESP and Talent Romandie documents used as source material rather than scholarly literature.
Treat them as primary-source or organizational-source entries.

### C. New scholarly framing sources
These are additional academic works introduced to make the article defensible as journal-style writing.
Use them sparingly and purposefully.
Prefer sources that help frame:
- youth athlete development
- coaching systems
- skill acquisition and technical development
- self-regulation and fatigue monitoring
- sport psychology in performance settings

## Workflow steps

1. Extract the bibliography already present in the anchor report.
2. Build a list of archive documents actually used in the article.
3. Separate archive documents from scholarly references.
4. Add only the minimum new academic framing references needed for:
   - conceptual framing
   - method justification
   - discussion positioning
5. Remove decorative references that do not affect the argument.
6. Convert all retained items into a `.bib` file.
7. Check that every in-text citation has a matching `.bib` entry.
8. Check that every `.bib` entry is cited or intentionally retained as a primary source appendix item.

## Citation discipline

- Do not invent missing bibliographic fields
- If fields are missing, keep the entry partial and mark the uncertainty in a note if needed
- Distinguish clearly between academic publications and organizational documents
- Prefer stable titles and dates over guessed metadata

## Recommended BibTeX entry types

Use these defaults when suitable:
- `@book` for books
- `@article` for journal articles
- `@inproceedings` for conference papers
- `@phdthesis` or `@mastersthesis` for theses
- `@techreport` for institutional reports
- `@misc` for archive documents, presentations, or web items when no better type fits

## Minimum bibliography outputs

Produce all of the following when generating the full package:

1. **bibliography audit**
   - anchor report references recovered
   - archive documents cited
   - new secondary sources added
   - unresolved metadata gaps

2. **bibliography.bib**
   - cleaned BibTeX file for the final LaTeX package

3. **reference-use note**
   - one short note explaining how the bibliography balances original report sources, archive materials, and later framing sources

## Suggested balancing rule

Default target mix for the final article:
- preserve the anchor report's core references where still relevant
- add archive citations where the argument depends on organizational history
- add only a focused set of new scholarly references to support framing and discussion

The final paper should not look like a literature review detached from the archive.
The archive remains central.
