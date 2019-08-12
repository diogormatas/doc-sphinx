# Key Data Project Types and Considerations
The basis for any successful data project is a clear understanding of what you're tasked to build and then understanding the major items that you need to consider in order to design a solid solution. We categorize data projects into three types that from our experience will typify many data projects. This categorization then allows us to explore the primary items we need to consider before starting on implementation. Not every project will fall neatly into one of these categories, and some projects might straddle these categories, but we feel that these project types will provide a useful framework for understanding your data use cases.


## Major Data Project Types
Let's begin by describing the three project types that we use to categorize data projects:

* **Data pipelines and data staging:** We can think of these as Extract, Transform, and Load (ETL)-type projects; in other words, these are projects that involve the collection, staging, storage, modelling, and so on of datasets. These are essentially projects that provide the basis for performing subsequent analysis and processing of data.

* **Data processing and analysis:** These are projects that end in providing some kind of actionable value. This might be the creation of reports, creation and execution of machine learning models, and so forth.

* **Applications:** A data framework that's meant to support live operational needs of application; for example, the data back-end for web and mobile applications or dashboards.


# Directory structure

This is the directory structure that every Data Science and Engineering project must obey accordingly to it's project type.

## Data pipelines and data staging

```
├── data
│   ├── external: Data from third party sources
│   ├── intermediate: Intermediate data that has been transformed.
│   ├── processed: The final, canonical data sets for modeling.
│   └── raw: The original, immutable data dump.
│
├── docs: A default Sphinx project; see sphinx-doc.org for details.
│
├── references: Data dictionaries, manuals, and all other explanatory materials.
│
├── reports: Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures: Generated graphics and figures to be used in reporting.
│
├── src: Source code for use in this project.
│   ├── data: Scripts to download or generate data.
│   ├── features: Scripts to turn raw data into features for modeling.
│   ├── visualization: Scripts to create exploratory and results oriented visualizations.
│   └── __init__.py: Makes src a Python module.
│
├── tests: Unit and integration tests. This must replicate the same structure of src.
│
├── CHANGELOG.md: Log about deployments versions and changes.
├── Makefile: Makefile with commands like 'make data' or 'make train'.
├── README.md: The top-level README for developers using this project.
├── requirements.txt: The requirements file for reproducing the analysis environment, e.g. generated with 'pip freeze > requirements.txt'.
└── setup.py: Make this project pip installable with 'pip install -e'.
```

The template repository to **data pipelines and data staging** projects is [here](https://gitlab.com/noesisportugal/dse/templates/data-pipelines-and-data-staging).
