# EDA on Titanic — Project 01

Exploratory Data Analysis of Titanic passenger records using Python and Pandas.

## Project questions

1. Did female passengers have a higher survival rate than male passengers?
2. Did passenger class relate to survival rate?
3. Did survival rate differ across passenger age bands?

## Repository contents

- `Titanic_EDA_Project.ipynb` — explained Jupyter notebook containing data inspection, cleaning, group comparisons, visualizations and written findings.
- `titanic.csv` — dataset used by the notebook. Keep this file in the same directory as the notebook.
- `Titanic_EDA_Summary_Report.pdf` — written project summary with numerical findings and methodology.
- `requirements.txt` — Python dependencies.

## Run the notebook

1. Clone or download this repository.
2. Install Python 3.10 or later.
3. Install the packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `Titanic_EDA_Project.ipynb` and select **Kernel → Restart & Run All**.

The notebook reads `titanic.csv` from its current directory.

## Analysis approach

The notebook uses `head()`, `info()`, `describe()`, missing-value counts and duplicate checks. Missing ages are filled with the median age for the corresponding passenger class and sex group; missing embarkation ports are filled with the mode; the highly incomplete deck/cabin column is dropped. Exact duplicate rows are counted, not blindly removed.

Survival rates are compared by sex, passenger class and age band. Results are descriptive associations and should not be interpreted as proof of causation.

## Expected findings

The accompanying report and notebook calculate the observed group rates from the included data. Re-run the notebook to reproduce the tables, charts and numerical findings.

## Notes

This is an educational exploratory analysis of historical Titanic passenger data. Add your name or student details to the notebook if required by your course before submission.
