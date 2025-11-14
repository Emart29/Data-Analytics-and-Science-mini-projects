# ⚽ Hypothesis Test on Goals Scored in Men's and Women's FIFA World Cup Matches

## 📊 Project Overview
This project conducts a statistical hypothesis test to compare the mean number of goals scored in women's and men's international soccer matches, specifically focusing on FIFA World Cup games since January 1, 2002. The analysis assumes match independence and uses a non-parametric test due to the non-normal distribution of goals scored.

The null hypothesis is that the mean goals scored in women's matches equals that in men's matches. The test is performed at a 10% significance level to determine whether to reject or fail to reject this hypothesis.

## 🎯 Objectives
- Filter FIFA World Cup matches from 2002 onward for both men's and women's datasets.
- Compute the total goals scored per match.
- Assess data normality and select an appropriate hypothesis test (Mann-Whitney U test, two-sided).
- Calculate the p-value and decide on the null hypothesis (reject if p-value ≤ 0.10).
- Summarize results in a dictionary containing the p-value and test outcome.

## 📂 Dataset Description
The datasets are sourced from CSV files containing historical soccer match results:
- **men_results.csv**: Men's international match data, including date, teams, scores, and tournament.
- **women_results.csv**: Women's international match data, with similar attributes.

Key columns used: `date`, `home_team`, `away_team`, `home_score`, `away_score`, `tournament`.

## 🧮 Key Analysis Steps
- Loaded datasets using Pandas and converted dates to datetime format.
- Filtered data for FIFA World Cup matches after 2002-01-01.
- Calculated `goals_scored` as the sum of home and away scores for each match.
- Combined filtered datasets and pivoted for hypothesis testing.
- Performed a two-sided Mann-Whitney U test using SciPy to compare goals in women's vs. men's matches.
- Extracted p-value (0.0102) and compared to significance level (0.10), resulting in rejection of the null hypothesis.

## 🛠 Tools & Libraries Used
- Python
- Pandas (data manipulation and filtering)
- SciPy (for Mann-Whitney U test)
- Jupyter Notebook (analysis environment)

## 📁 Project Files
- **notebook.ipynb**: The main Jupyter notebook containing the full analysis code.
- **men_results.csv**: Dataset for men's soccer results.
- **women_results.csv**: Dataset for women's soccer results.

## 💡 Insights
- The p-value (0.0102) is less than 0.10, leading to rejection of the null hypothesis. This suggests a statistically significant difference in the average goals scored between women's and men's FIFA World Cup matches.
- Women's matches may exhibit higher goal counts based on the data, but further analysis (e.g., one-sided tests) could explore directionality.
- These insights can inform sports analytics, betting strategies, or tournament planning by highlighting differences in scoring dynamics.

## 🧾 Example Output
The results are stored in a dictionary:
```python
result_dict = {
    "p_val": 0.010213219650887282,
    "result": "reject"
}
```
