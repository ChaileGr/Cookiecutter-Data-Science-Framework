# cookiecutter_data_framework

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

evaluation of predictive poolicing models and running data processing pipeline

Name: Chaile Grandy 

Course: INST414 Section: 0201

Topic: Racial Biases in Predictive Policing Models

Research Questions:

For this sprint, a model is being created to answer the following questions:

What is the estimated accuracy rate of racial bias in algorithmic models?
How large is the gap between different racial arrests?
Is there a correlation with race and economic-status along with the number of arrests.

Key Findings:
Accuracy Results: 80% overall accuracy results in predicing the outcome for race and annual income.
Visual Trends: Data shows relatively high correlation with race,income, and conviction especially relating to Black and Hispanic populations.
Model Performance: Linear Regression Model was the only model to really work consistently and show accurate results.


Method Overview:
Merge two-to-three datasets that include factors of race, socio-economic status, and arrests.
Once the datasets have been merged or added, I will then clean up the dataset as there are over 400,000 rows combined and dates ranging from 2008-2015.
Once the data is cleaned up, the statistical tests (XGBooster, RF Model, Linear Regression Model) will be ran to identify the correlation between race/economic bias along with arrest rates and calculate the estimated rate of racial bias in the dataset.
Data Visualizations:

Once the statistical tests are complete, Jupyter Lab will then be used to visualize the actual data and will be used as a comparison to ensure the dataset and tests are both accurate.
Results:

There is clear bias within the dataset for jupyterlab as shown visually, however in vscode the data shows something different based on the numeric data. The data in vscode shows a fairly even distribution of the data and that is due to simply removing categorical values of race and keywords like "SUSPECT". With the numerical data, the only included factors were numbers mostly based on income per race. So, as an intervention–removing keywords of race (Black, White, Hispanic) and focusing more on the numerical data may help reduce the bias results received from predictive policing models.

Reproduced Results (Cookiecutter Data Framework):

The ccds structure was created in my terminal and then used to reorganize the data used in creating this model. Running and evaluating the model(s) gave challenges to my project, as I struggled to do this task for the original Sprint 2 assignment. However, I should still be able to run the data processing pipline with ease.

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         cc_df and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── cc_df   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes cc_df a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

