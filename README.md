# ETW2500 Assignment 3: Question 1

This project contains the Question 1 contribution on brand loyalty. It is not the complete three-question group submission.

## Files

- `ETW2500_A3.Rproj`: open this file in RStudio to establish the project root. Saved workspaces are not restored or saved.
- `document/PersonA.qmd`: editable answer, with all seven items and visible R code.
- `document/PersonA.html`: main rendered report; resources are embedded for sharing.
- `document/PersonA.pdf`: rendered PDF attachment.
- `dataset/brand_example.csv`: the supplied three-household example.
- `dataset/bathsoap.csv`: the supplied 600-household dataset, unchanged.
- `document/session-info.txt`: R and package versions used for the verified render.
- `Question1_class_methods.md`: links between the code and the supplied teaching materials.
- `Question1_HD_review.md`: rubric review and outstanding group-submission requirements.

The original CSVs and class materials at the project root are retained for reference. The report reads only the copies in `dataset`.

## Reproduce the report

1. Install R, RStudio and Quarto if needed. The verified R and Quarto versions are recorded in `document/session-info.txt`.
2. Open `ETW2500_A3.Rproj` in RStudio. Restart R so that the document is checked without objects from an earlier session.
3. Once per computer, install missing packages in the R console:

   ```r
   install.packages(c("tidyverse", "here", "gt", "knitr", "rmarkdown"))
   ```

4. Open `document/PersonA.qmd` and choose **Render** for HTML. Choose **Render PDF** from the render menu for the attachment. PDF rendering needs a working TeX installation; if none is installed, run `quarto install tinytex` in the RStudio Terminal once.
5. Alternatively, run these commands from the project root in the RStudio Terminal:

   ```text
   quarto render document/PersonA.qmd --to html
   quarto render document/PersonA.qmd --to pdf
   ```

The output files are written beside the Quarto source in `document`. Paths use `here()` and do not depend on a particular user's desktop location. Keep the R Project file, `document` folder and `dataset` folder together when moving the project. No manual import, `setwd()`, saved workspace or internet dataset is required. The analysis contains no random operations, so no random seed is needed.

## Checks to expect

- 600 observations and 600 unique `MemberID` values.
- No missing values in the eight named brand-share columns.
- `MaxBrShare` ranges from 0 to 1, with no missing or out-of-range values.
- 22 zero-share households; all have `NoBrands = 1` and `BrOthers = 1`.
- Original example distances: X-Y = 1.414214; X-Z = Y-Z = 0.707107.
- Revised example distances: X-Y = 0; X-Z = Y-Z = 0.5.

`group_by(MemberID)` is a valid row-specific calculation for this dataset because each ID occurs once. If the dataset is replaced or edited, check ID uniqueness again before relying on that calculation. The written interpretations describe the supplied data; review them if the inputs change. The distance comparison table is calculated automatically.

## Complete the group submission

Merge Questions 1–3 into one Quarto file. Add the group leader's full name as the YAML author and all members' names and student IDs in the YAML or opening text. Use the first ten letters of the leader's name, without spaces, for the project folder and Quarto filename as required by the brief; update the source filename in these instructions and re-render after renaming. Keep one final Quarto file, one HTML and one PDF in `document`, with the CSVs in `dataset`. Zip the final project folder for submission.

The current Question 1 author is Ahmad Sfui Aziz Shah, as provided. Do not present this contribution as the complete assignment. The final leader attribution, all student IDs, remaining group-member details and final naming convention still need to be completed for the group submission.
