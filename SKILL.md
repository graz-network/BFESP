---
name: bfesp-orchestrator
description: orchestrate the extension of rapport-fep-graz and the wider bfesp source archive into a bilingual academic article workflow with pdf review, archive analysis, expert coaching lenses, yearly talent romandie summaries, originality and extension planning, journal-style selection, mandatory citation policy, and final latex plus pdf deliverables. use when chatgpt must coordinate a thesis or report pdf, bfesp project documents, talent romandie history, or produce staged academic outputs in english and french with independent researcher syntheses.
---

# BFESP orchestrator

Use this skill to run a staged research workflow around `Rapport-FEP-Graz` and the broader BFESP project archive.

The objective is to transform the original coaching report into a stronger academic contribution of about 20 pages while preserving the original training-science core.

This skill is designed for projects that combine:
- one anchor PDF such as `Rapport-FEP-Graz-digital.pdf`
- a broader BFESP document archive
- a Talent Romandie historical corpus spanning multiple years
- a need for bilingual academic outputs in English and French
- a final delivery in LaTeX and PDF

## Core orchestration model

Run the project through seven analytical lenses and two independent writer lenses.

### Expert lenses
- cycling coaching expert
- sports coaching expert
- performance sport psychology expert
- freestyle sport expert
- olympic cross-country mountain biking (XCO) expert
- researcher agent english
- researcher agent french

The first five lenses analyze the material and produce structured expert findings.
The two researcher agents then synthesize the expert materials independently.
They work from the same source base, but each writes its own final article in its own language.
Do not collapse the English and French researcher outputs into a single mixed-language draft.

## Mandatory composition rule

When `pdf-review-workflow` is available, use it on the anchor PDF first.
Treat its outputs as a required input to the rest of this workflow.
At minimum extract and carry forward:
- summary
- academic review
- main arguments
- weaknesses
- next steps

The `next steps` from `pdf-review-workflow` must not remain generic.
Translate them into a concrete extension plan using the BFESP archive and the historical Talent Romandie materials.

## Mandatory style and citation rule

Before any full article drafting begins, select the target article style using `references/journal-style-selector.md`.
Then apply the mandatory citation policy in `references/citation-policy.md`.

Do not draft the full paper until both of these are fixed:
- target journal or article style profile
- citation style policy

If the user does not specify a target journal, default to the generic sport-science profile and APA 7 style implemented through author-date citations.

## Supported inputs

Use these inputs whenever available:
- uploaded `Rapport-FEP-Graz` PDF
- uploaded BFESP project files
- uploaded or connector-accessible Talent Romandie files
- BFESP notes, drafts, bibliographies, source tables, spreadsheets, and related PDFs
- Google Drive files when the user points to them or when the archive lives there

If the archive is too large to bundle in the skill, treat it as runtime input and analyze it through available connectors.

## Default project objective

Unless the user specifies a narrower task, use this default objective:
- analyze `Rapport-FEP-Graz` in full
- summarize and evaluate the report as a whole
- map the original contribution, method, training logic, and practical recommendations
- analyze BFESP documents for supporting evidence, continuation paths, and contradictions
- summarize Talent Romandie materials by year
- identify historical evolution across Talent Romandie documents
- convert the archive into a defensible academic extension
- produce two independent article versions, one in English and one in French
- deliver the final article package as LaTeX and PDF

## Workflow decision tree

1. Determine the user task stage.
   - archive inventory request -> follow `intake and source map`
   - report understanding request -> follow `anchor pdf review`
   - project corpus analysis request -> follow `bfesp archive pass`
   - yearly history request -> follow `talent romandie chronology pass`
   - expert interpretation request -> follow `expert lenses pass`
   - style or journal targeting request -> follow `journal style selector pass`
   - extension or originality request -> follow `research extension pass`
   - writing request -> follow `dual researcher writing pass`
   - latex or pdf request -> follow `article package pass`
   - final quality control request -> follow `preflight checklist pass`

2. If the user does not specify a stage, run the default sequence:
   - intake and source map
   - anchor pdf review
   - bfesp archive pass
   - talent romandie chronology pass
   - expert lenses pass
   - research extension pass
   - journal style selector pass
   - article blueprint pass
   - bibliography workflow pass
   - dual researcher writing pass
   - preflight checklist pass
   - article package pass

## Intake and source map

Start every new project with an inventory.

Produce:
- anchor document list
- BFESP source list
- Talent Romandie source list
- source type map by year
- missing pieces or unclear files
- research question candidates
- extension hypotheses

Always identify the anchor report explicitly:
- title
- author
- date
- original scope
- original practical setting
- original athlete or case focus if present

## Anchor pdf review

Apply `pdf-review-workflow` to the full `Rapport-FEP-Graz` PDF.

Extract at minimum:
- title and context
- one-paragraph summary
- full-section map
- research objective or coaching objective
- methodology or reasoning style
- main findings
- practical recommendations
- weaknesses or limitations
- next steps

Also create a focused extraction of the report's internal architecture:
- discipline analysis
- athlete analysis
- annual planning logic
- training intervention logic
- competition analysis logic
- technical innovation or freestyle contribution
- psychological implications already present or absent

## BFESP archive pass

Analyze BFESP documents as the second evidence layer.

For each relevant BFESP file, classify it as one or more of:
- conceptual continuation
- methodological support
- empirical support
- historical context
- contradiction or tension
- later reinterpretation
- implementation material

Produce:
- BFESP corpus table
- key themes recurring across files
- evidence that strengthens the original report
- evidence that dates or weakens parts of the original report
- evidence that opens a stronger academic contribution

Do not treat every file equally. Prioritize documents that materially change the interpretation of the anchor report.

## Talent Romandie chronology pass

Summarize Talent Romandie materials year by year.

For each year represented in the source archive, produce:
- document list for that year
- short yearly summary
- athlete development themes
- coaching structure themes
- performance themes
- technique themes
- psychological or motivational themes
- evidence of institutional evolution
- relevance for extending `Rapport-FEP-Graz`

Then produce a longitudinal synthesis across years:
- what remained stable
- what evolved
- what intensified
- what became outdated
- what new coaching or sport-psychology questions emerged

If the source base is incomplete, state clearly which years are evidenced and which are not.

## Expert lenses pass

Load `references/expert-lenses.md` and generate the required expert memoranda.

## Journal style selector pass

Load `references/journal-style-selector.md`.
Select one style profile before article drafting.
At minimum fix:
- target readership
- article type
- sectioning profile
- tone profile
- citation and reference expectations
- figure/table appetite
- default title and abstract conventions

If no user preference is provided, choose the generic sport-science profile.
Record the choice explicitly in the article blueprint.

## Research extension pass

Convert the review outputs, archive findings, and expert memoranda into an article extension plan.

The extension plan must answer:
- what is academically original in the extended article
- what is historically valuable but not original
- what remains practical coaching know-how
- what can be generalized
- what should remain a bounded case
- which claims are strongly evidenced
- which claims are provisional
- where the archive materially extends the 2016 report

Always distinguish between:
- claims supported directly by the anchor report
- claims supported by later BFESP or Talent Romandie materials
- interpretive claims proposed by the new article

## Article blueprint pass

Use `references/article-outline.md` and `references/output-spec.md`.

Produce:
- working title options
- chosen style profile
- final section outline
- section word budgets
- figures/tables plan if relevant
- contribution statement
- originality statement
- risk list for overclaiming

## Bibliography workflow pass

Use `references/bibliography-workflow.md` and `references/citation-policy.md`.

Produce:
- bibliography audit
- citation style decision note
- list of anchor-report references recovered
- list of archive sources cited as primary material
- list of new scholarly framing sources
- cleaned `bibliography.bib`

## Dual researcher writing pass

After the blueprint and bibliography steps are complete, generate two independent article drafts.

### English researcher agent
Produce:
- full English article draft
- English abstract
- English title options
- English author note if requested

### French researcher agent
Produce:
- full French article draft
- French abstract
- French title options
- French author note if requested

Rules:
- both articles must follow the same evidence base and article blueprint
- they may differ in phrasing and argument emphasis
- they must not be treated as literal translations of one another
- the French outputs may be written in French; all orchestration notes remain in English

## Preflight checklist pass

Before final LaTeX packaging, load `references/preflight-checklist.md`.

Run the final preflight and explicitly report:
- coherence status
- originality status
- evidentiary balance status
- unresolved weaknesses
- citation compliance status
- section budget compliance status
- archive coverage limits

If any item fails, revise before packaging unless the user explicitly asks for a draft with known issues.

## Article package pass

Package the final outputs according to `references/output-spec.md`.
Use the LaTeX template in `assets/article_template.tex` and the bibliography starter in `assets/bibliography_template.bib` when useful.

Deliverables should normally include:
- English `.tex`
- French `.tex`
- bibliography `.bib`
- generated PDFs when tool support is available
- brief packaging note listing any unresolved compile or citation issues

## Resource map

Read these files when needed:
- `references/expert-lenses.md` for the expert roles and evaluation criteria
- `references/article-outline.md` for the strict article outline and word budgets
- `references/output-spec.md` for the package contract
- `references/bibliography-workflow.md` for bibliography recovery and `.bib` generation
- `references/journal-style-selector.md` for target journal or article style selection
- `references/citation-policy.md` for the mandatory citation policy
- `references/preflight-checklist.md` for final article quality control
- `assets/article_template.tex` for the final LaTeX scaffold
- `assets/bibliography_template.bib` for starter bibliography structure

