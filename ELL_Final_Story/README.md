# English Language Learners are transforming city schools — and pushing their limits
### As immigrant families arrived in record numbers, some public schools saw their ELL populations explode, exposing deep gaps in educational equity and stretching already thin support systems.
#### By Juan Lasso | New York, May 20, 2025
---
In the wake of a historic surge in immigration to New York City, public schools experienced a dramatic increase in English Language Learner (ELL) enrollment—jumping from 135,000 to over 148,000 students between the 2022 and 2023 school years. While the influx reflects the growing linguistic diversity of the city, it also reveals deep disparities in how schools are able—or unable—to serve these students. The burden has disproportionately fallen on low-income and overwhelmingly minority schools, with limited bilingual resources, raising questions about the quality of ELL education. 
[Download the final story (HTML)](https://github.com/Juan-Lasso/ELL_Final_Story/raw/main/ELL_data_folder/advdata_final_story_ell.html)

# Methodology 
To understand where the number of English Language Learner students is growing fastest in New York City, I analyzed enrollment data released by the city’s Department of Education.

The information comes from the DOE’s Demographic Snapshot, a dataset that includes demographic and enrollment figures for every public school in the city. I focused on a subset of the data that tracks ELL enrollment at the school level across recent academic years.

The file — downloaded in April 2025 — includes data up through the 2023–24 school year. The analysis compared enrollment from 2022–23 to 2023–24 to identify which schools saw the biggest increase in the number of ELL students, regardless of school size using percent change.

To perform the analysis, the data was cleaned and reformatted using Python and the Pandas library. I filtered the file to retain only the relevant fields: school name, year, total enrollment, and the number and percentage of ELL students. A new column was added to extract the starting year of each school year (e.g., 2022 for 2022–23) to simplify comparisons.

After isolating the two most recent years, I calculated the year-over-year change in the number of ELL students at each school. Schools were ranked based on the highest percent change in ELL students, and the 10 schools with the largest jumps were selected.

One outlier, Olympus Academy, was excluded from the final results. While the school technically saw a 700% increase in ELL enrollment — from one student in 2022–23 to eight in 2023–24 — the change was not statistically significant compared to the much larger increases at other schools. To maintain the integrity of the findings, only schools with meaningful absolute gains were considered.

The analysis does not account for percentage growth or longer-term trends. Schools with missing data for either of the two years were excluded, as were schools with no change or a decrease in ELL enrollment. The dataset includes both traditional public and charter schools, but no distinction was made between them.
Factors such as changes in classification, policy shifts, or new program rollouts may also influence ELL counts beyond student movement alone. While the data offers insight into recent shifts, it may not capture the full picture of why certain schools saw rapid growth.


# Data Source

The original dataset used in this analysis can be found here:  
[Download Demographic Snapshot Data (Excel)](https://github.com/Juan-Lasso/ELL_Final_Story/raw/main/ELL_data_folder/raw-data/Demographic_Snapshot_ENL.xlsx)

The cleaned, modified data set in this analysis can be found here:
[Download ENL Percent Change Data (Excel)](https://github.com/Juan-Lasso/ELL_Final_Story/raw/main/ENL_percent_change.xlsx)

