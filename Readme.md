# Employee Turnover Prediction
The HR department at Salifort Motors wants to take some initiatives to improve employee satisfaction levels at the company. They have the following question: what’s likely to make the employee leave the company?

Our objective in this project is to analyze the data collected by the HR department and to build a model that predicts whether or not an employee will leave the company.

If our model can predict employees likely to quit, it might be possible to identify factors that contribute to their leaving. Because it is time-consuming and expensive to find, interview, and hire new employees, increasing employee retention will be beneficial to the company.

* The data set is provided in [HR_capstone_dataset.csv](HR_capstone_dataset.csv).<br>
* Decision Tree model is built in [Build_Classification_Model.ipynb](Build_Classification_Model.ipynb).<br>
* [Figures](Figures) folder contains various plots.<br>

> * Tasks Performed:
>   * Conducted extensive `EDA`, `cleaned` and `structured` the dataset for analysis.
>   * `Tuned hyperparameters` of all models through `grid search` and `cross-validation`.
>   * Developed an optimal `Logistic Regression`, `Random Forest`and, `Gradient Boost` Model to predict whether employee will leave or stay.
>   * Evaluated the model performance on validation sets, and then selected Gradient Boosting model as the champion, achieving a `Recall score of 90.19%` and other metrics including an accuracy of 96.82%, f1 of 90.55%, and precision of 90.91%.
>   * Identified key features influencing employee retention: `Tenure`, `Number of project`, and `Overworked`.

> * Recommended: To retain employees,
>   * Cap the number of projects that employees can work on.
>   * Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied.
>   * Either reward employees for working longer hours, or don't require them to do so.
>   * If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear.
>   * Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts.
>   * High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort.

> * Next Steps
>   * It may be justified to still have some concern about data leakage. It could be prudent to consider how predictions change when last_evaluation is removed from the data. It's possible that evaluations aren't performed very frequently, in which case it would be useful to be able to predict employee retention without this feature. It's also possible that the evaluation score determines whether an employee leaves or stays, in which case it could be useful to pivot and try to predict performance score. The same could be said for satisfaction score.

> * Skills Demonstrated: EDA, Logistic Regression, Tree Based ML Algorithms, Hyperparameter Tuning, Cross-validation.