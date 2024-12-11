
# Experiment runs

## tsa-flirtini-241126-r241112

analysis note: make sure to check well by well that the temp melt curves "make sense" (i.e. the curve should be a single peak, and the temperature should be the melting temperature of the DNA).
redo analysis of the data.

Analysis operations
- convert the raw data file (tidy table) into a 384w plate layout dataframe with Tm D being the target value.  this is then pasted into the analysis tab
- split this dataframe into two dfs, left and right
- for both dfs:
  - label columns 1-4 "APO" and columns 5-8 "DNA"
  - label rows by sample (rows B-P) and DMSO (row A)
  - make a new df called summary_df
    - calculated columns:
      - AVG of 4 APO replicates: "APO Tm"
      - SD of 4 APO replicates: "APO SD"
      - DMSO subtraction of APO samples: "APO dTm" (hold DMSO APO Tm value constant and subtract from all sample APO Tm)
      - AVG of 4 DNA replicates: "DNA Tm"
      - SD of 4 DNA replicates: "DNA SD"
      - DMSO subtraction of DNA smaples: "DNA dTm" (hold DMSO DNA Tm value constant and subtract from all sample APO Tm)

**Results**
![](readme_img/2024-12-09-16-43-46.png)

**Notes**
- No echo transfer report errors
-
**Protocol**
![](readme_img/2024-11-26-15-37-40.png)


---
# Notes
[compound request link](https://scorpiontx.sharepoint.com/:x:/r/sites/SPWorkingDocuments/_layouts/15/Doc.aspx?sou[…]0Assay%20Tracker.xlsx&action=default&mobileredirect=true)


## r241112

- ST-0136747-01
- ST-0136755-01
- ST-0176880-01
- ST-0176773-01
- ST-0136751-01

