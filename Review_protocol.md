# A Systematic Review of Provenance for Machine Learning Experiments: A New Taxonomy and Comparative Analysis

## Objective

To identify, classify, and compare approaches that model structured provenance or lineage for machine-learning experiments, including data preparation, training, evaluation, and related experimental artifacts. The review also records deployment and inference capabilities when supported by the included publications.

## Rationale

Existing reviews on data provenance are generally broader than ML experimentation, while ML lifecycle and MLOps reviews often address experiment tracking and metadata rather than structured provenance relationships. This review focuses on the provenance mechanisms used in iterative ML experiments and compares them using a common taxonomy.

## Research questions

- **RQ1 (WHAT):** What parts of the ML experimental pipeline are covered by provenance solutions?
- **RQ2 (HOW):** How is provenance acquired, including automation, capture mechanism, intrusiveness, and temporal mode?
- **RQ3 (Representation & Access):** How is provenance represented, stored, queried, and visualized?
- **RQ4 (WHY):** What experimental purposes are supported by provenance?
- **RQ5 (PRACTICAL):** What integration, overhead, storage, and scalability constraints are reported?

## Methods

### Review design

The review follows Kitchenham's systematic literature review methodology, with the study-selection process reported using PRISMA 2020.

### Eligibility criteria

**Inclusion criteria**

- Publications proposing, implementing, or empirically evaluating structured provenance or lineage for ML experimentation.
- Explicit modeling of derivation or dependency relationships among experimental artifacts, activities, or runs.
- Domain-agnostic approaches when applicable to ML or data-science environments (such as scripts, notebooks, numerical libraries, or workflows) and meeting the structured-relationship criterion.
- Peer-reviewed journal, conference, or established workshop publications.

**Exclusion criteria**

- General provenance without a qualifying ML/data-science experimental context.
- ML experiment tracking, monitoring, versioning, or metadata management without explicit structured experimental provenance relationships.
- Non-primary or non-peer-reviewed work, including surveys, position papers, documentation, and posters.
- Non-English publications.

### Information sources and search strategy

ACM Digital Library, IEEE Xplore, ScienceDirect, and SpringerLink were used in the primary search. The database-specific Boolean expressions, search date, and raw exports are documented in `Search_documentation.md` and the four corresponding ZIP archives. Scopus was additionally used as a supplementary coverage check, not part of the primary 611-record count.

### Study selection

The primary search yielded 611 records; four duplicates were removed, leaving 607 unique records. Title/metadata screening excluded 567 records and identified 40 reports for full-text assessment. Of these, 37 were eligible: one report was excluded for lacking eligible structured provenance and two were excluded as non-primary vision/position work. Publication-family tracing identified six further associated reports; the final corpus comprised 43 primary reports.

### Unit of analysis

Publications that extend, demonstrate, or apply the same technical system lineage are consolidated into one family for system-level comparison, while individual publications remain evidence sources. The 43 reports were consolidated into 29 system families. Later-version features are not retroactively assigned to earlier versions.

### Data extraction

Information was extracted using a structured form organized around the five research questions. The form covers provenance scope, capture, representations and access, experimental purposes, and practical evidence; see `DEF_v1_final.odt`.

### Data synthesis

The 29 system families are compared through a faceted, multi-label taxonomy with five axes: WHAT, HOW, Representation & Access, WHY, and PRACTICAL. The narrative synthesis identifies patterns, trade-offs, and research gaps. Practical performance figures are retained in their original measurement contexts rather than converted into global ranks.

## Public materials

This compact package provides the protocol, search documentation, raw bibliographic exports, and extraction form. Detailed per-record screening outcomes and completed per-report extraction sheets are not part of this public version. The selected reports, family assignments, and comparison tables are reported in the associated manuscript.
