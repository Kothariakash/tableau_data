
**Data Analysis Exercises**

1. **Tax Authority Distribution for Changed and Removed:**

Analyze the distribution of Tax Authority (Auth) for records labeled as "Changed" and "Removed". This will help understand which tax authorities are most frequently associated with changes and removals.

Findings:

- The highest number of changes are associated with records where Auth is nan, followed by FED.
- States like NJ, WA, and CA also have a significant number of changes.
- Other states and authorities have relatively lower occurrences.

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.001.png)

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.002.png)

The analysis indicates that FED and nan are the most common Tax Authority values for both "Changed" and "Removed" labels. However, there are notable differences in the distribution of other authorities between the two labels. This information can be valuable for further investigations into the reasons behind these changes and removals.

1. **Wage Type Distribution for Changed and Removed**

Examine the distribution of ‘Wage Type’ (WT) for records labeled as "Changed" and "Removed". This analysis will identify which wage types are most modified or removed.

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.003.png)

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.004.png)

1. **Analysis on tax authority as Nan**

   This report analyzes the dataset to identify the distribution and characteristics of records with `NaN` values in the `Auth` (Tax Authority) field. Additionally, it examines the distribution of `Wage Type` (WT) and `Payroll Results` for these records, as well as the presence of multiple `Auth` types per employee.


1. **Records with NaN in ‘Auth’ and its WT distribution:**

- Number of records with ‘NaN’ in ‘Auth’: 559,131
- Certain wage types, such as ‘TRAN’, ‘/845’, ‘/700’, ‘/550’, and ‘/194’, are more frequently associated with records that have ‘NaN’ in the `Auth` field
- Distribution of ‘Payroll Results’ for Records with NaN in ‘Auth’ and The majority of records with NaN in ‘Auth’ are categorized under "Normal Period Results"

  - Normal Period Results: 528,696 occurrences

  - Retro Period Adjustments: 15,674 occurrences

  - Prior Period Adjustments: 14,761 occurrences

  1. Employee Records analysis:
     1. Employees with NaN in ‘Auth’: 9,833 unique employees
     1. Employees with FED in ‘Auth’: 9,705 unique employees
     1. Maximum number of different ‘Auth’ types per employee: 7


![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.005.png)


1. **Tax Authorities adhere to a Federal-State-County hierarchy.**

   It has been observed that Tax Authorities can be primarily categorized into three types: Federal Taxes, NULL/NaN (this category may be used for WTs that do not require tax authorities or for bookkeeping purposes), and State-specific taxes. Under the State-specific tax category, there are County-specific tax authorities and additional state-specific tax authorities utilized for bookkeeping purposes.

   ![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.006.png)

   Kindly refer to [this excel sheet](https://amedeloitte.sharepoint.com/:x:/r/sites/HCaaSAssetandProductDevelopment/_layouts/15/Doc.aspx?sourcedoc=%7B4CC4C3A5-E980-4669-A27B-E62308DC8AA6%7D&file=Tax_Auth_hierarchy.xlsx&action=default&mobileredirect=true&wdsle=0)  for the Mapping of State wise Tax Authorities and their sub- authorities(counties ).





1. **WTs belonging to Different Tax Authorities.**

   During our analysis we found that: 

- There are 189 WTs for Authorities related to State and County (For 9<sup>th</sup> Pay period 181 WTs)
- 31 WT for FED Tax authority (For 9<sup>th</sup> Pay period 37 WTs)
- 280 WTs for NULL(Nan) Tax Authority (For 9<sup>th</sup> Pay period 297 WTs)
- There is no WTs Which are in common between NULL(Nan) Tax Authority and Authorities related to FED, State and County
- There are 10 common WTs between Authorities related to State and County and FED Tax authority

  Note: Kindly use [this excel sheet](https://amedeloitte.sharepoint.com/:x:/r/sites/HCaaSAssetandProductDevelopment/_layouts/15/Doc.aspx?sourcedoc=%7B73D981B0-0F36-4353-9415-FFCC180BF493%7D&file=Tax_Auth_WT.xlsx&action=default&mobileredirect=true&wdsle=0) for detailed cataloging of WT’s based on the Tax       Authorities

1. **Specific Employee and Pay Code Findings**
   1. **Changed/Removed Labels in 3rd Pay Period**:

      Out of 31 employees, 30 were found in prioritized pay codes from David's list.

   1. **Changed/Removed Labels in 9th Pay Period**:

      Out of 23 employees, 21 were found in prioritized pay codes from David's list.

   1. **Remaining Pay Codes**:

      The remaining pay codes not caught were 'LCI', 'LLB', and 2090.

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.007.png)

**Interpretation:**

- A high percentage of employees with changed or removed labels were found in prioritized pay codes, indicating a strong correlation between these employees and the prioritized pay codes from David's list.
- A few pay codes ('LCI', 'LLB', and 2090) were not included in this prioritization, which may require further investigation to understand why they were excluded.
- Tax Authority for all the records in these prioritized pay codes is “NaN”.

1. **Wage Type Grouping** 

   [Tax_related_WTs_grouping.xlsx](https://amedeloitte-my.sharepoint.com/:x:/g/personal/sumityadav34_deloitte_com/Ee-BLpvjPdhAslZkXTVH2joB72mkTC7Y2PBewtOZgk9yxw?e=QToQeG)

![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.008.png)


![](Aspose.Words.aa611bac-56db-47c9-911f-fd33091a9bdf.009.png)





