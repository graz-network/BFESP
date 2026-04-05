# BFESP Orchestrator

`bfesp-orchestrator` is a research orchestration skill for turning the 2016 **Rapport-FEP-Graz** professional sport performance coaching report and the broader **BFESP / Talent Romandie** archive into a stronger bilingual academic article package.

It is designed for projects that combine:

- one anchor PDF such as `Rapport-FEP-Graz.pdf`
- a broader BFESP archive
- Talent Romandie materials spanning multiple years
- a need for **independent English and French article drafts**
- final delivery in **LaTeX** and **PDF**

## What the skill does

The skill runs a staged workflow that moves from archive understanding to publishable article packaging.

### Default objective

Unless the user narrows the task, the skill will:

- analyze `Rapport-FEP-Graz` in full
- summarize and evaluate the original report
- map the report's training logic, contribution, and limitations
- analyze BFESP materials for continuations, contradictions, and supporting evidence
- summarize Talent Romandie documents by year
- build a longitudinal interpretation across the archive
- convert the material into a defensible academic extension
- produce two article drafts:
  - one in English
  - one in French
- package outputs in LaTeX and PDF

## Core workflow

The orchestrator follows this default sequence:

1. intake and source map
2. anchor PDF review
3. BFESP archive pass
4. Talent Romandie chronology pass
5. expert lenses pass
6. research extension pass
7. journal style selector pass
8. article blueprint pass
9. bibliography workflow pass
10. dual researcher writing pass
11. preflight checklist pass
12. article package pass

## Analytical model

The skill uses **seven analytical lenses** plus **two writer lenses**.

### Expert lenses

- cycling coaching expert
- sports coaching expert
- performance sport psychology expert
- freestyle sport expert
- olympic cross-country mountain biking (XCO) expert
- researcher agent english
- researcher agent french

The first five lenses generate expert findings.
The two researcher lenses then write **independent** final articles from the same evidence base.

## Required dependency

This skill assumes the presence of `pdf-review-workflow`.

The anchor PDF must first be processed through that workflow, with at least these outputs carried forward:

- summary
- academic review
- main arguments
- weaknesses
- next steps

The “next steps” must then be converted into a **concrete archive-based extension plan**.

## Style and citation rules

Before full drafting begins, the skill must fix:

1. a **journal / article style profile**
2. a **citation policy**

### Default style

If the user does not specify a target journal, the default is:

- **generic sport-science**
- **APA 7 compatible author-date logic**

The style profile is selected from `references/journal-style-selector.md`.
Citation rules are enforced by `references/citation-policy.md`.

## Supported inputs

The skill is designed to work with:

- uploaded `Rapport-FEP-Graz` PDFs
- uploaded BFESP files
- uploaded or connector-accessible Talent Romandie files
- notes, drafts, source tables, spreadsheets, and related PDFs
- Google Drive archives accessed at runtime

## Output package

Standard staged deliverables include:

1. source map
2. anchor PDF review bundle
3. BFESP archive memorandum
4. Talent Romandie yearly summaries
5. longitudinal Talent Romandie synthesis
6. five expert memoranda
7. style decision note
8. extension plan
9. article blueprint
10. bibliography audit
11. English article draft
12. French article draft
13. preflight note
14. LaTeX package
15. PDF package

### Typical final package

```text
project-output/
  english_article.tex
  french_article.tex
  english_article.pdf
  french_article.pdf
  bibliography.bib
  figures/
  tables/
  preflight_note.md
```

## Repository structure

```text
bfesp-orchestrator/
  SKILL.md
  agents/
    openai.yaml
  assets/
    article_template.tex
    bibliography_template.bib
  references/
    article-outline.md
    bibliography-workflow.md
    citation-policy.md
    expert-lenses.md
    journal-style-selector.md
    output-spec.md
    preflight-checklist.md
```

## Key reference files

### `SKILL.md`

Main orchestration logic, required stages, and package expectations.

### `references/expert-lenses.md`

Defines the expert roles and the questions each lens should answer.

### `references/journal-style-selector.md`

Defines supported style profiles and the selection rule.

### `references/citation-policy.md`

Defines mandatory citation discipline and source-class distinctions.

### `references/article-outline.md`

Sets the default article structure and section word budgets.

### `references/bibliography-workflow.md`

Explains how to separate:

- anchor report references
- archive primary sources
- new scholarly framing sources

### `references/preflight-checklist.md`

Final QA before packaging.

### `assets/article_template.tex`

LaTeX scaffold for final article packaging.

### `assets/bibliography_template.bib`

Starter bibliography structure.

## Typical use cases

This skill is a good fit when you want to:

- evaluate `Rapport-FEP-Graz` as a whole
- reconstruct the logic of the 2016 report
- connect later BFESP or Talent Romandie materials to the original report
- identify what is still valuable vs outdated
- build a bilingual academic article from a coaching archive
- produce a LaTeX/PDF-ready submission package

## Example prompt

```text
Using Rapport-FEP-Graz-digital.pdf as the anchor document and the Talent Romandie archive as the extension layer, analyze the full report, identify the strongest coaching and sport-psychology contributions, summarize the historical evolution of Talent Romandie by year, and produce English and French LaTeX article drafts in the generic sport-science style with APA-style author-date citations.
```

## Design principles

- **Anchor first**: the 2016 report is the starting point, not an afterthought.
- **Archive-aware**: later BFESP and Talent Romandie documents are used to extend, not flatten, the original report.
- **Bilingual by design**: English and French outputs are parallel, not literal translations.
- **Evidence-disciplined**: archive materials must not be presented as peer-reviewed literature.
- **Packaging-ready**: the workflow is built to end in LaTeX and PDF.

## Notes

- The skill is strongest when the archive contains at least one anchor report plus several later organizational documents.
- If corpus coverage is partial, the final outputs should state that clearly.
- Historical value, practical coaching innovation, and academic originality should be kept distinct.

## License / project note

Add the repository's actual license and contribution policy here if this skill is published outside a private workflow environment.
