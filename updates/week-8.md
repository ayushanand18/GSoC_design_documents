# Week 8
## 1 August to 7 August 2022
+ Weekly meet on 2 August.
    + **Agenda**:
        + couldn't complete due to network error and some urgent work

### Tasks accomplished
+ Completed `migration_pattern.ipynb`
    + A geo-temporal analysis of species migrations
        - analysed geo-spatial data for *Mola mola* over time
        - created a generic class and methods to grab data, make an interactive plotly plot and even create a GIF to visualize spatial changes over time for any species.
+ Completed /docs/ update
    + details mentioned in [week-7 objectives](./week-7.md)
+ Updated Jupyter Notebook - `depth_time_series.ipynb`
    + added an analysis of averaged depth for an order of species to make up for scarce data.
    + added another analysis to visualize the average deviation from mean depth in species in an `order`
+ created setup.cfg, setup.py and pyproject.toml for the package
    + updated project details and added more fields like `project urls`
+ Fixed some errors in the docs workflow
    + The `deploy_docs` workflow run was throwing some errors due to a broken link to the API docs (which didn't happen during local tests, I don't know why.) Also, there was an error being thrown while navigating into the `_build/html` directory after the building process, because the folder was name `_build/` and workflow was trying to call `build/`.

### Tasks working on
+ updating depth notebook and working on suggestions
+ working on `MeasurementOrFacts Analysis.ipynb` notebook
+ Updated depth analysis notebook and working on suggestions
+ Created `setup.cfg`, `pyproject.toml` and updated `setup.py`
