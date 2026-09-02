# Content and Rubric Review (latest `main.tex`)

## Rubric benchmark

The linked 2026 Four-New Special Competition article requires a real and specific global issue, a China-positioned/global-view analysis, and a feasible China solution. The report must show **discover problem -> analyse problem -> solve problem**, and contain Title, Abstract, Introduction, Research Design, Results, Discussion & Conclusion, and References. The body (excluding abstract and references) is 2,000--3,000 words; the abstract is 200--300 words. The scoring image weights: topic value 20, research process 20, research outcomes 30, structure 10, expression 20.

## Word count (TeXcount)

Using `texcount -inc -sum main.tex` on the latest source:

- Abstract: **201 words** (within 200--300).
- Body prose: **3,257 words** (latest pre-final pass; already above the 3,000-word ceiling before headings/captions).
- Body headings: 138; captions/source material: 61. A conservative count including these is about **3,456 words**. Tables are included in TeXcount's text count.
- Before the current compression pass, body prose was about 3,521 words. The submission should still remove at least 300--450 words, preferably target 2,750--2,850 prose words to leave a counting-method margin.

**Live update:** after the latest edits, a full copy with abstract and bibliography removed gives about **2,945 words in the five numbered sections** (2,961 including the keyword line), plus 148 heading words and 61 caption/source words. This is likely compliant only under a prose-only counter; trim another ~200 words or remove nonessential front matter/caption prose so a Word-style body count is safely below 3,000.

Section prose counts (useful trimming targets): Introduction 460; Research Design 394; Results 1,072; NE--AI solution 872; Discussion/Conclusion 459. Trim duplicated explanation in Results/Solution first; keep the methods and pilot gates that support the rubric.

## Priority findings and concrete replacements

### P0: factual/source precision

1. **IEA denominator (latest source, Introduction paragraph 2 and Table `global`).** IEA *Electricity 2024* reports approximately 460 TWh in 2022 and a possible >1,000 TWh in 2026 for the combined **data-centre, AI, and cryptocurrency** sector (not data centres or AI alone). The latest wording is mostly corrected, but retain the combined-sector qualifier in both prose and table and add the source note to the row. Suggested wording: “IEA estimates that data centres, AI and cryptocurrency together consumed about 460 TWh in 2022 (nearly 2% of global demand) and could exceed 1,000 TWh in 2026.”

2. **China forecast wording (Introduction, “Why a China-informed perspective matters”).** “the IEA forecasts almost 60% of new capacity becoming operational globally by 2028” is incomplete/ambiguous. Replace with: “the IEA expects China to account for almost 60% of new renewable capacity that becomes operational globally by 2028.” Also distinguish **installed capacity** from generation: “renewable power capacity exceeded half of China’s total installed power-generation capacity” (not “installed generation” if the denominator is capacity).

3. **WEF 44% indicator (Table `global`).** This is an employer-survey expectation about the share of workers’ skills likely to be disrupted, not workers reporting disruption. The latest label is improved; use exactly: “Employers expecting workers’ skills to be disrupted in the next five years — 44% (2023 survey estimate).” Keep “employers” in the interpretation sentence too.

4. **Fudan/Tianda attribution (Introduction, China policy paragraph).** Fudan Consensus and Tianda Action are university-led initiatives discussed/endorsed in Ministry policy material, not necessarily Ministry programmes. Replace “The Ministry of Education’s ‘Fudan Consensus,’ ‘Tianda Action,’ and new-engineering projects promote…” with “The Ministry of Education’s 2017 policy response endorsed the Fudan Consensus and Tianda Action and supported subsequent New Engineering projects promoting…”

5. **Zhangbei technical nomenclature (Results, Zhangbei paragraph).** The cited Hitachi profile says “four-station meshed HVDC voltage-sourced-converter grid,” while the text says “four-terminal.” Use “four-station meshed voltage-source-converter HVDC grid” (or state that it has four terminals only if the source explicitly supports that term). Keep 500 kV/4,500 MW and 14 billion kWh explicitly marked as project-reported; the current caveat about no independent AI metrics is good.

### P1: method validity and evidence traceability

6. **“Mixed-method” overclaim (Research Design, Overall logic).** The study has descriptive secondary statistics plus qualitative coding/case comparison, but no inferential quantitative method. Replace “mixed-method comparative case design” with “structured desk review and qualitative comparative case analysis based on secondary evidence.” This avoids a method mismatch under “research process.”

7. **Screening counts need an auditable denominator.** The 126 -> 89 -> 54 -> 38 -> 31 flow is useful, but the manuscript does not give per-database hits, search date, exact result-export date, or a list/appendix of records. Add one compact sentence: “Searches and exports were run on [date]; database-level counts and inclusion decisions are in the screening log (supplementary file).” If no supplementary file exists, call the counts an author-created process record and avoid implying a systematic-review protocol.

8. **Single-reviewer recheck.** The latest text correctly says it is not inter-rater reliability. Keep that limitation and specify what was rechecked (e.g., 20% random sample, all numerical claims, or all included records). Suggested wording: “A second pass rechecked all included records and numerical extractions; because there was one reviewer, this is a consistency check rather than inter-rater reliability.” Do not claim “triangulation” unless independent sources were actually compared.

9. **Sensitivity/robustness paragraph is not reproducible.** “Re-coding… still produced…” gives no counts or coding rule. Either report the exact retained counts by sensitivity run, or soften to: “A qualitative sensitivity check found the same four themes after separately removing policy and peer-reviewed sources; this is indicative, not a statistical robustness test.”

10. **Case selection scope.** Two purposively selected Chinese cases cannot establish global transferability or causal effects. Add “illustrative, mechanism-focused cases” and explicitly state that no non-Chinese case was analysed. The current limitation paragraph should say transfer claims are hypotheses for the pilot, not findings.

### P1: outcome strength and implementation

11. **Rubric’s highest-weight item (research outcomes, 30%).** The four-layer framework is clear and innovative, but resource/cost responsibility remains implicit. Add a short “delivery responsibility and cost gate” sentence/table cell: utility owns operational safety and baseline KPIs; university owns curriculum/benchmark; regulator/community committee owns consent and pause decisions; procurement reports lifecycle cost. State that scale is blocked if total lifecycle cost, water stress, or outage risk exceeds a pre-registered margin. Avoid unsupported budget numbers unless labelled planning assumptions.

12. **Targets need operational definitions.** Define mean absolute error (MAE), SAIDI, SAIFI, PUE, WUE, and LCA at first use. Replace “no increase in SAIDI/SAIFI” with “SAIDI and SAIFI non-inferior to baseline within a pre-specified margin,” and define the denominator for “100% auditable high-impact actions” and “20% lower carbon per inference.” Add prediction-interval coverage/calibration as a technical KPI; MAE alone does not test probabilistic reliability.

13. **Target rationale.** The 15% MAE, 10% curtailment, and 20% carbon-per-inference thresholds are labelled ex ante, which is responsible, but their selection is unexplained. Add one clause: “Thresholds are deliberately illustrative planning hypotheses, to be set after baseline variance and power analysis,” or cite a benchmark. Do not present them as expected effects.

14. **Equity mechanism.** “Equity-oriented financing and knowledge-sharing” is not yet a mechanism. Name the beneficiary and metric: paid apprenticeships/technician seats, offline tool availability, outage/price distribution by subgroup, and a community veto/pause channel. This directly answers the rubric’s social value and feasibility criteria.

15. **AI governance claims.** “The approach fits NIST, IEC, ISO/IEC, UNESCO, and OECD principles” overstates alignment. Replace with “The approach is designed to be consistent with relevant NIST, IEC, ISO/IEC, UNESCO, and OECD principles.” Add a source or qualify the uncited claim that federated learning “can improve models.”

## Language and academic expression

- Define “New Engineering” once as the formal Four-New direction, then capitalize consistently; avoid alternating “new-engineering,” “New Engineering,” and “emerging-engineering.”
- Define abbreviations on first use: AI, DC, MAE, SAIDI, SAIFI, PUE, WUE, LCA, and (if retained) RMF. The table currently introduces several without expansion.
- “The interfaces are contractual” is opaque. Replace with “The interfaces are specified as acceptance criteria.”
- “A day-ahead model outputs a distribution … and calibrated interval” -> “A day-ahead model outputs a predictive distribution with calibrated intervals.”
- “low confidence or lost connectivity returns control” -> “low confidence or lost connectivity returns the controller to a tested deterministic policy.”
- “Every pilot reports compute energy per training run and inference” -> “Every pilot reports energy per training run and per defined inference workload.”
- “accounted compute impacts” in the conclusion -> “explicitly accounted-for compute impacts.”
- Split the long robustness-check paragraph and the long implications paragraph into 2--3 sentences each. Keep one claim per sentence where evidence or a caveat changes.
- Keep one spelling convention (the manuscript currently uses British `optimisation`, `programme`, `centres`, `labelled`, `anonymised`; apply it consistently in headings, tables, and references).

## Citation/reference audit

- All 26 citation keys currently resolve to a bibliography entry; no missing or uncited key was detected.
- References are not alphabetised (the list starts IEC, then Hong). Reorder alphabetically by author/institution, or explicitly use a consistent citation-order style. APA-like entries should also use one consistent treatment of report titles, URLs, and access dates.
- `sgcc2020` is keyed as SGCC but the entry is Hitachi Energy. Rename the key or use a State Grid primary source to avoid misleading provenance.
- The IEA table source note aggregates several indicators; add row-level citations in prose/table notes where feasible so each number has an unambiguous source.
- Replace `http://` government URLs with `https://` where the same document is available, and use the exact standard part for IEC 62443 rather than a generic landing page if possible.
- Corporate/news sources (Hitachi Energy, China Daily) are acceptable for project-reported facts only; label them as such and do not use them to infer causal performance.

## Format/compliance observations for the main thread

- The seven required modules are present and ordered logically; the problem -> method -> results -> framework -> evaluation -> discussion chain is a strength.
- All five long tables use `xltabular` with repeated heads, `Table n (continued)`, a continuation notice, and `booktabs` top/mid/bottom rules. This satisfies the requested cross-page three-line-table behavior; keep the continuation label in English in the English report.
- `config.sty` sets A4, 1-inch margins (2.54 cm), 1.5 spacing, and Times New Roman under XeLaTeX. Strict reading of the article’s “全文12号” could question `\small` captions/source notes and the title-page note; decide whether to retain smaller table source notes for legibility.
- The title page author is the placeholder “English Research Report.” Replace with actual participant/team/university information before submission.

## Estimated score (latest text, before final fixes)

This is an evidence-based estimate, not an official judging result:

| Dimension | Max | Current estimate | Rationale |
|---|---:|---:|---|
| Topic value | 20 | 17--18 | Strong New Engineering fit, concrete global grid/AI issue, China + global lens; national strategy link and beneficiary can be sharper. |
| Research process | 20 | 14--16 | Clear review flow and coding dimensions; single-reviewer, two-case scope and incomplete audit trail limit reproducibility. |
| Research outcomes | 30 | 23--26 | Coherent four-layer framework and staged gates; cost ownership, KPI definitions, and observed-vs-ex-ante distinction need strengthening. |
| Structure | 10 | 9 | Required modules and logic are clear; some repetition and front matter can be trimmed. |
| Expression | 20 | 16--18 | Generally fluent academic English and broad citations; undefined abbreviations, attribution/denominator wording, reference ordering, and a few opaque sentences remain. |
| **Total** | **100** | **79--87** | Likely 88--92 after word-count compliance, source precision, KPI/resource detail, and reference cleanup. |
