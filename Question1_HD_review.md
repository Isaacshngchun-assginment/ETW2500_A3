# Question 1 review against the HD rubric

This is an evidence-based review of the Question 1 contribution, not a predicted mark. The rubric applies to the whole assignment; Questions 2 and 3 and the final combined submission also need to meet it.

| Rubric criterion | Evidence in this contribution | Remaining requirement |
|---|---|---|
| Reproducibility and documentation (10) | An R Project file disables workspace restoration; relative `here()` paths read unchanged CSVs in `dataset`; the README explains setup, fresh-session rendering, expected results and file structure; R code is visible. Software versions are recorded in `document/session-info.txt`. | Preserve this structure when combining the group's work and rerun the final document from a fresh session. |
| Code accuracy, efficiency and clarity (10) | Tidyverse selects the intended variables, checks unique IDs and missingness, calculates one maximum per household, and counts the zero cases. Both distances use `dist()`. The comparison table is generated from the actual results. | Use tidymodels where appropriate in the later work. It is not needed for Question 1, which involves no fitted predictive model or PCA recipe. |
| Appropriate analysis (20) | Euclidean distances answer the specified comparison. The calculation includes exactly eight named brands and excludes the pooled `BrOthers` category. IDs are excluded from distances; both example proportions already use the same scale. | Justify the separate variable selection and methods for Questions 2 and 3. |
| Presentation (20) | Seven numbered answers follow the question order, with a short objective, readable tables, a labelled comparison table, visible code, and both HTML and PDF formats. | Review the combined report's headings, cross-references, page layout and table consistency. |
| Interpretation and theoretical reasoning (30) | The report distinguishes loyalty from brand identity, explains why ungrouped `max()` is wrong here, interprets all 22 zero values using `NoBrands` and `BrOthers`, and explains both the correction and the limitations of the new measure. Item 7 remains within the requested two sentences. | Maintain this reasoning standard in the segmentation and dimension-reduction sections. |
| Language and format (10) | Clear explanations, consistent variable names, project-relative paths, required document/dataset folders, and all analysis code visible in both formats. | Supply the leader's full name, every member's name and student ID, and the required leader-based folder and Quarto filenames. Merge all questions into one final document. |

## Interpretation points to preserve

- X and Y have equal purchase-share loyalty despite buying different brands.
- The original distances make X-Y the most distant pair; this reflects brand identity.
- `MaxBrShare` makes X-Y distance zero, while both distances to Z are 0.5.
- All 22 zero values refer to single-brand buyers whose brand is pooled into `BrOthers`. Zero is not evidence of disloyalty.
- The maximum does not reveal purchase order or the distribution of remaining shares. It is one indicator of loyalty, not a complete description.

## Final submission status

Question 1 can be reviewed independently, with Ahmad Sfui Aziz Shah recorded as its current author. The overall assignment is not submission-ready until Questions 2 and 3, final leader attribution, all student IDs, remaining member details and the prescribed final naming are completed. No mark or HD outcome can be guaranteed by this checklist.
