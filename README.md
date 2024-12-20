Last revision: 12/10/2024

### **Estimating Enrollment of Black, Latina, AIAN, NHPI Women in Computing Programs**

The model estimates the number of women and Black, Latina, AIAN, NHPI women enrolled in Bachelor's level computing programs for the current and following academic years.

Public Statements for use: 

For the academic year 2025 (Fall 2024 \- Spring 2025): Approximately 173,595 undergraduate women are studying computing across the country – 141,045 (or 81%) are enrolled at non top 25 ranked schools.  92% of BLN women are enrolled at non top 25 ranked schools.

#### **Findings**

1. **Where to Recruit From**  
   Companies who focus their recruiting/hiring on the “top 25” universities are missing out on 87% of total computing degree earners and **92%** of Black, Latina, AIAN, NHPI Women (as of 2023).  
   Based on IPEDS data, the top-25 universities graduate relatively few Black, Latina, AIAN, NHPI women: in 2023, these universities awarded:   
   \-   15,649 total computing Bachelor’s degrees  
   \-   4,988 to women  
   \-   481 to women identifying with one of the above underrepresented ethnicities  
2. **Predicted Growth in Degree Completions**  
   The total awarded computing degrees shows a positive growth YoY, but the growth rate has been slowing down prior to 2023\. As of 2023, the growth rate from the previous year is only 4%.  
3. **Share of Women in Computing**  
   The share of Women and Black, Latina, AIAN, and NHPI Women show a steady increase both in absolute numbers and as a percentage of total degrees conferred (excluding top 25 universities).  
   The share of women computing degrees has increased from 17.9% in 2015 to 22.1% in 2023 while the share of Black, Latina, AIAN, and NHPI women’s computing degrees has increased from 4.5% in 2015 to 5.4% in 2023\.  
4. **Enrollment Estimate**  
   For the 2025 (current) academic year, the model estimates 141,045 of women and 37,243 of Black, Latina, AIAN, and NHPI women in computing degrees at non- top 25 universities.   
   For the 2026 academic year: 148,289 of women and 39,751 of Black, Latina, AIAN, and NHPI women pursuing computing Bachelor’s degrees.

#### **Limitations**

* **Degree Completion Trends as Proxy for Enrollment**   
  Enrollment data at the program level was unavailable. Hence, completions were used as a proxy for trends.  
* **Retention Rates**  
  Assumed unchanged retention rates across all cohorts, which may not fully capture institutional or programmatic differences.  
* **Growth Rate Selection**  
  The model used absolute degree growth instead of growth rate trends due to the absolute degree growth showing a more consistent linear growth compared to the growth rate data points that do not follow a linear trend.

#### **Methodology and Data Summary**

1. **Data Collection and Preparation**:  
   * Sourced from **IPEDS:** the degree completions data for each year (2015–2023) was joined with institutional characteristics for the same year.  
   * Filtered for **Bachelor's programs** under **CIP code 11 (Computing)** and **excluding** **top 25 computing programs**.  
   * For each year, aggregated the following metrics:   
     total computing degrees conferred, computing degrees awarded to women, computing degrees awarded to Black, Latina, AIAN, and NHPI women.

| Year | Total degrees | growth rate | % of students graduating from non- top 25 schools | Women degrees | % of total | Black, Latina, AIAN, NHPI Women degrees | % of total | % of women |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| 2015 | 56,653 | \-- | 91.3% | 10,144 | 17.9% | 2,575 | 4.5% | 25.4% |
| 2016 | 60,721 | 7.2% | 90.1% | 11,302 | 18.6% | 2,705 | 4.5% | 23.9% |
| 2017 | 66,881 | 10.1% | 89.5% | 12,619 | 18.9% | 3,034 | 4.5% | 24.0% |
| 2018 | 74,286 | 11.1% | 89.0% | 14,687 | 19.8% | 3,310 | 4.5% | 22.5% |
| 2019 | 81,878 | 10.2% | 88.5% | 16,456 | 20.1% | 3,766 | 4.6% | 22.9% |
| 2020 | 89,051 | 8.8% | 87.7% | 18,405 | 20.7% | 4,024 | 4.5% | 21.9% |
| 2021 | 95,922 | 7.7% | 87.6% | 20,264 | 21.1% | 4,771 | 5.0% | 23.5% |
| 2022 | 98,923 | 3.1% | 87.2% | 21,629 | 21.9% | 5,113 | 5.2% | 23.6% |
| 2023 | 103,007 | 4.1% | 86.8% | 22,749 | 22.1% | 5,572 | 5.4% | 24.5% |

     

2. **Trend Analysis and Prediction**:  
   * A **4-year lookback window** (2020–2023) was used to calculate annual growth rates via the **LINEST() function** (applied to columns: total degrees, women degrees, and Black, Latina, AIAN, NHPI women degrees)  
   * Based on the best-fit linear trend, future completions were predicted incrementally through 2030\.

| Year | Total degrees | Women degrees | Black, Latina, AIAN, NHPI Women degrees |
| ----- | ----- | ----- | ----- |
| 2024 | 107,494 | 24,189 | 6,071 |
| 2025 | 111,981 | 25,628 | 6,569 |
| 2026 | 116,468 | 27,068 | 7,068 |
| 2027 | 120,955 | 28,508 | 7,566 |
| 2028 | 125,442 | 29,948 | 8,065 |
| 2029 | 129,928 | 31,387 | 8,564 |
| 2030 | 134,415 | 32,827 | 9,062 |

   * The previous step (2) will account for growth rate in degree completions when deriving enrollment estimates in the following step (3).

       
3. **Enrollment Estimation**:  
   * Used cohort retention rates provided by a previous consultant:  
     * Freshman: 100%, Sophomore: 82%, Junior: 74%, Senior: 66%, Graduation: 64%.  
   * Predicted enrollment for 2024–2026 based on projected degree completions, accounting for retention rate dynamics.   
   * For instance, to calculate enrollment data for academic year of 2024:  
     * Freshmen enrollment \= completions for 2027 \* 100% / 64%  
     * Sophomore enrollment \= completions for 2026 \* 82% / 64%  
     * Junior enrollment \= completions for 2025 \* 74% / 64%  
     * Senior enrollment \= completions for 2024 \* 66% / 64%  
     * Total 2024 enrollment estimate \= Freshmen enrollment \+ Sophomore enrollment \+ Junior enrollment \+ Senior enrollment

**Enrollment Estimate (excl. Top 25 Universities)**

| Year | Women Total | Black, Latina, AIAN, NHPI Women |
| ----- | ----- | ----- |
| 2024 | 133,802 | 34,734 |
| 2025 | 141,045 | 37,243 |
| 2026 | 148,289 | 39,751 |

#### 

#### 

#### **Future Considerations**

1. **Lookback period**  
   Adjust the lookback period for the model from 4 years to another number of years that reflects the degree completions trend better. If the computing degree completion trend increases rapidly, the lookback period should be less than 4 years. If it appears to be more stagnant as time goes by, the lookback period can be extended to more than 4 years.

2. **Integrating IPEDS enrollment data**  
   While the enrollment data files do not provide a breakdown by CIP code (cannot filter by computing), this data can be considered in this model to account for Bachelor’s program enrollment growth trends.   
   This can provide insights into academic trends in more real-time compared to graduation data alone. The current model takes the computing program graduation data for the last 4 years to inform the computing degree completion growth rate, after which enrollment numbers are estimated. This method does not provide enough flexibility if there is a sudden boom or decline in enrollment into Bachelors programs. In such a case, the model will reflect that trend only after 6 years: 4 years for students to graduate \+ 2 years for IPEDS to release graduation data (in academic year 2025, we only have data on 2023 available).   
   Integrating enrollment data can help finetune the growth rate in this model.

3. **Research and provide better estimates for the academic funnel**  
   Per the methodology, the cohort retention rates were kept the same from the 2022 version of this report:   
   Freshman: 100%, Sophomore: 82%, Junior: 74%, Senior: 66%, Graduation: 64%.   
   This might change in the long term.

4. **List of Top 25 universities (by Computing program)**  
   The top-25 list is updated periodically, so the model will need to be adjusted.

5. **Expanding the scope of this project**  
   For future work, it would be interesting to look at the breakdown by HBCU / PWI.
