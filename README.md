# Price Prediction for Airbnb Listings in New York

## Dataset

Dataset is from [OpenDataSoft](https://public.opendatasoft.com/explore/dataset/air-bnb-listings/information/?disjunctive.neighbourhood&disjunctive.column_10&disjunctive.city) which can be downloaded [here](https://data.insideairbnb.com/united-states/ny/new-york-city/2024-04-06/visualisations/listings.csv).

An alternative dataset can also be obtained from [Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data).

## Virtual Environment setup

1. **Install pipenv**:

   ```bash
   pip install pipenv
   ```

2. **Create a project folder and activate a virtual environment**:

   ```bash
   pipenv shell
   ```

3. **Installation of dependencies**:

   - **Option a)**:
     ```bash
     pipenv install
     ```
     (may not be deterministic)
   - **Option b) [RECOMMENDED]**:
     ```bash
     pipenv install --ignore-pipfile
     ```
     This allows you to install production dependencies (deterministic and installs exact versions).

4. **Run Jupyter notebook**:
   ```bash
   jupyter notebook
   ```
