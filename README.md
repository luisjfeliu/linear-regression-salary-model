# Linear Regression: Salary Prediction Model

This project analyzes employee salary data to explore relationships between salary and predictors such as education level, years of experience, gender, and job title. It uses descriptive statistics, visualizations, and linear regression models to identify statistically significant salary drivers and interpret their practical impact.

## Project Structure

- **`salary_prediction_project.ipynb`**: Main Jupyter Notebook with data cleaning, exploratory analysis, regression modeling, feature reduction, and interpretation.
- **`salary_data.csv`**: Source dataset with employee demographics, job titles, experience, education, and salary.
- **`salary_prediction_project.html`**: Exported HTML version of the notebook.
- **`presentation/Model Salary Data with Linear Regression Presentation Slides.pdf`**: Final presentation deck in PDF format.

## Key Analyses

1. **Data Description and Cleaning**
   - Loads the salary dataset and reviews the first rows.
   - Checks dataset size and missing values.
   - Drops rows with missing fields before modeling.
   - Summarizes the salary range, mean, median, and overall distribution.

2. **Exploratory Data Analysis**
   - Counts employees by education level.
   - Visualizes education-level counts with a bar chart.
   - Visualizes salary distribution with a histogram.
   - Compares average salary by gender, education level, and years of experience.

3. **Regression Modeling**
   - Uses ordinary least squares regression with `statsmodels`.
   - Creates indicator variables for gender, education level, and job title keywords.
   - Fits an initial salary model using gender, years of experience, education, and job-title flags.
   - Identifies variables that are not statistically significant and fits a reduced model.

4. **Model Interpretation**
   - Interprets the expected salary change for each additional year of experience.
   - Estimates the salary difference associated with a senior title.
   - Estimates the salary difference associated with a PhD.
   - Calculates a predicted salary and residual for an example employee.

5. **Model Fit and Diagnostics**
   - Evaluates model fit using regression output, including `R-squared`.
   - Uses a residuals-versus-fitted plot to assess whether the linear model is appropriate.
   - Discusses model performance and remaining prediction error.

## Libraries Used

- **Pandas**: Data loading, cleaning, grouping, and dummy-variable creation.
- **NumPy**: Numeric operations.
- **Matplotlib**: Bar charts, histograms, and residual plots.
- **Statsmodels**: Ordinary least squares regression and regression summaries.

## Getting Started

1. Install dependencies:
   - `pip install pandas numpy matplotlib statsmodels jupyter`
2. Open the notebook:
   - `jupyter notebook salary_prediction_project.ipynb`
3. Run all cells to reproduce the descriptive statistics, regression models, and visualizations.

## Presentation

Presentation files are in `presentation/`:

- `presentation/Model Salary Data with Linear Regression Presentation Slides.pdf`

## License

This project is licensed under the MIT License. See `LICENSE` for details.
