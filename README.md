# Education

> Is school performance associated with location and socioeconomic factors?

---

## Project Overview

- **Objective:** The main goal of this project is to determine how much of the variation in schools’ average ACT scores can be explained by location, school type, and socioeconomic factors.
- **Domain:** Education
- **Key Techniques:** Multiple Linear Regression

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** https://www.edgap.org/, https://nces.ed.gov/ccd/
- **Description:** EdGap (Excel): 7,986 schools × 7 columns, for the 2016-2017 school year. NCES school information (CSV): 102,183 schools × 65 columns, seven were kept.

---

## Analysis

JupyterLab was used to preform the analysis. It was preformed in the notebook Education_Project.ipynb and should be run in order. The file explores and cleans the data into the file education_clean.csv and uses multiple linear regression to discover how loaction, school type, and other socioeconomic factors are associated with school's average ACT scores.

---

## Results

The final model explained about 68% of the variation in high schools’ average ACT scores (R² = 0.682, adjusted R² = 0.680, RMSE = 1.42, MAE = 1.02; n = 7,227 schools in 20 states).

Free and reduced-price lunch had by far the largest association with average ACT (-1.821), followed by the percent of adults with a college degree (0.4045). Unemployment rate, percent of children in married-couple families, and median income had much smaller associations. Each state had a significant association. School type and charter status added no detectable value, although the data contained very few schools that were not regular, non-charter schools. 

Full results can be found in results.pdf in the reports folder.
---

## Authors

- Joey Matte - [@mattejoey](https://github.com/mattejoey)

---

## License

This project is licensed under the MIT License.

---

## Acknowledgements

- Tools/libraries used: numpy, pandas, matplotlib, seaborn, scikit-learn, statsmodels, jupyter, notebook, ipython
- Courses referenced: Seattle University MSDS DATA 5100 Foundations of Data Science
- Inspiration: Dr. Xiaoxi Zhang