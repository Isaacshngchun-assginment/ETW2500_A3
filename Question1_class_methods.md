# Question 1: links to the supplied class methods

The working answer is `document/PersonA.qmd`. Open `ETW2500_A3.Rproj` before rendering. It covers Question 1 only. The PDF filename and the user's request identify this as A3, although the PDF's first-page heading says Assignment 2.

| Method used                                       | Supplied class material |
|---                                                |---|
| Quarto, visible R code, `read_csv()` and `here()`                  | `week 1 and 2/document/tut 2 inclass.qmd` |
| `select()`, `filter()`, `mutate()`, `group_by()` and `summarise()` | `Note/Data wrangling basic notes and R scripts/wrangling R script.R` |
| `max()`, `n_distinct()` and counting with `sum()` | `Note/Data wrangling basic notes and R scripts/Data Wrangling.pdf`, page 20 |
| Grouped `mutate()`, `across()` and `count()` | `Note/Data Wrangling Intermediate Notes and R scripts/data wrangling - intermediate.R` |
| `ungroup()` | `tutPCA.qmd`, the plot of the three largest loadings |
| Euclidean distance using `dist()` | `week 4/tutorial/document/Tutorial 4.qmd` |
| `summary()` and checking missing values with `is.na()` | `week 5/tut_cluster2 student/tut_cluster2 student/document/tut_cluster2.qmd` |
| `tibble()` for the distance comparison table | `Note/Data Wrangling Intermediate Notes and R scripts/data wrangling - intermediate.R` |
| `gt()` and `fmt_number()` for readable tables | `Note/Descriptive Analysis 2 - notes and R script/descriptive p2.R` |

The grouped maximum combines methods in these materials. It works row by row here because the answer first verifies that `MemberID` is unique. It avoids introducing `rowwise()`, `c_across()`, `pmax()` or `apply()`, which were not found in the supplied materials reviewed.

Question 1 does not need a fitted clustering model, PCA, regression, a train/test split or standardisation. Both example brand shares already use the same 0–1 scale, and the requested distances are calculated directly from those shares.

The project now uses the required `document` and `dataset` folders. For the group's final submission, merge this answer into the group's single Quarto file, add the leader's name, members' names and student IDs, and apply the required filenames. The current files are a working Question 1 contribution, not the complete group submission. See `README.md` for reproduction and submission instructions.
