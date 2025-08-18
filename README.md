# Synthetic Project Analysis

This repository contains a synthetic dataset of project metrics and a Jupyter Notebook that performs exploratory data analysis and predictive modeling on the dataset. The goal is to simulate the type of analysis a business analyst, program manager, or data analyst might perform when assessing project performance and predicting outcomes.

## Dataset

The dataset (`synthetic_projects.csv`) contains 500 rows, each representing a unique project. The columns include:

- **project_id**: Unique identifier for each project.
- **start_date**: Project start date.
- **end_date**: Project end date.
- **planned_budget**: The budget planned for the project (in USD).
- **actual_budget**: The actual budget spent (in USD).
- **team_size**: Number of people on the project team.
- **priority**: Project priority (`High`, `Medium`, `Low`).
- **risk_level**: Risk level (`Low`, `Medium`, `High`).
- **manager_experience_years**: Years of experience of the project manager.
- **complexity**: Project complexity (`Low`, `Medium`, `High`).
- **success**: Binary indicator of project success (1 = success, 0 = not success). Generated using a logistic function of risk, complexity, manager experience, and budget overrun.
- **roi**: Return on investment, calculated as `(planned_budget - actual_budget) / planned_budget`.

## Notebook

The Jupyter Notebook (`analysis.ipynb`) includes:

1. **Data Loading and Overview**: Load the dataset, inspect its structure, and compute summary statistics.
2. **Exploratory Data Analysis (EDA)**: Visualize distributions of budgets, team sizes, and durations; examine relationships between features and success; and compute correlation matrices.
3. **Predictive Modeling**: Build and evaluate a logistic regression and random forest classifier to predict project success based on available features. Split the data into training and test sets, train the models, and evaluate their performance using accuracy and confusion matrices.
4. **Insights**: Summarize findings from the EDA and modeling.

## Usage

1. Clone or download this repository.
2. Install the required dependencies from `requirements.txt` using:

```bash
pip install -r requirements.txt
```

3. Open the Jupyter Notebook located in the root of this repository:

```bash
jupyter notebook analysis.ipynb
```

4. Run the cells to reproduce the analysis. You can also modify the notebook to explore additional questions or models.

## Dependencies

All dependencies are listed in `requirements.txt`. They include `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `notebook`.

## License

This project is provided for educational purposes and does not reflect real project data. Feel free to fork or adapt it for your own learning or portfolio.
