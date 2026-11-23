# Titanic EDA — Written Summary

## Objective
Explore the Titanic passenger dataset using Pandas to identify patterns in passenger survival.

## Questions
1. Did female passengers have a higher survival rate than male passengers?
2. Did passenger class relate to survival rate?
3. Did survival rate differ across passenger age bands?

## Data preparation
The dataset contains 891 passenger records. The notebook inspects the DataFrame with `head()`, `info()`, and `describe()`. Missing values are counted with `isna().sum()`. Missing ages are filled with the median age within the same passenger class and sex group. Missing embarkation ports are filled with the mode. The deck/cabin column is dropped because most entries are missing. Exact duplicate rows are counted; rows are not deleted blindly.

## Main findings
- Female passengers survived at approximately **74.2%**, compared with approximately **18.9%** for male passengers.
- Survival by passenger class was approximately **63.0%** for first class, **47.3%** for second class and **24.2%** for third class.
- The child age band had the highest survival rate (approximately **58.0%**) while the senior age band had the lowest (approximately **22.7%**) under the age-band definitions in the notebook.
- Overall survival was approximately **38.4%**.

The notebook calculates and prints all group rates from the cleaned data and displays the supporting tables and charts.

## Conclusion
Survival rates differed across sex, passenger class and age bands. Female passengers and passengers in first class had higher observed survival rates. These are descriptive associations, not proof that any one factor caused survival.

## Limitations
Age-band values partly depend on the age-imputation method. The senior group is small, so its percentage is less stable. This historical dataset should not be generalized beyond its scope without further evidence.
