# Football Position Predictions Project

## Barcelona School of Economics - Team Gracia

### Team Members
- Oliver Gatland
- Arianna Michelangelo
- Pere Pericot
- Edward Monbiot

## Project Overview
As a newly appointed data scientist team at a top tier football club our role is to leverage data analytics to enhance the team's talent development strategy. Leveraging data from FIFA 2022, this project aims to establish a robust classification model that can accurately recommend the optimal playing position for each youth player. 
By analyzing players' physical attributes and their correlation with on-field performance, this project delivers actionable insights to coaching staff. This facilitates optimal player positioning and skill development, harnessing data-driven strategies to enhance team performance.

## Core Competencies
- **Data Preprocessing and Quality Assurance**: Implementation of rigorous data cleansing and preprocessing.
- **Exploratory Data Analysis (EDA)**: Employing statistical and visualization techniques for insights.
- **Feature Engineering**: Innovating in feature creation and selection (KNN)
- **Model Development and Evaluation**: Utilizing and evaluating models: logistic regression, RandomForest, LightGBM, and ensembles.
- **Cross-Validation Techniques**: Applying StratifiedKFold and LeaveOneOut to check for robustness of models.
- **Problem-Solving**: Addressed a real-world sports analytics challenge with actionable data insights.

## Technologies and Tools
- **Languages**: Python
- **Libraries**: Pandas, Seaborn, Matplotlib, Scikit-Learn, LightGBM
- **Data Analysis**: Statistical analysis and data visualization
- **Machine Learning**: Implementation of diverse machine learning algorithms

## Model Evaluation Steps
- Ran a logistic regression model, a random forest model and then a Light GBM classifier
- Identified most influential features within random forest model
- The cross validation results showed that all the models performed similarily. Random forest has a slightly lower score for both cross-validation approaches, but the differences are marginal. We then performed hyperparameter tuning for the random forest and light GBM models to see if the accuracy improved in any of the models.
- Then attempted an ensemeble approach (base estimator: random forest, final estimator: logistic regression) but this produced a lower F1 score.

## Conclusion
- After hyperparameter tuning, the random forest model exhibited the highest F1 score. Thus this model was used in the final prediction.
- Best Hyperparameters: {'max_depth': None, 'min_samples_split': 2, 'n_estimators': 1000} F1 with best hyperparameters: 0.39031033882242083

## Installation and Usage
Detailed instructions for setting up and running the project are provided, ensuring straightforward replication and comprehension.

