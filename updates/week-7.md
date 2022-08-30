# Week 7
## 25 July to 31 July 2022
+ Weekly meet on 26 July.
    + **Agenda**:
        + work on a geo-temporal analysis to figure out trends of species migrations over time on water
        + decide on what issues to take up this week

### Tasks accomplished
+ Refactoring /docs/
    + updating the documentation of all modules in the package
        - renaming the resources module, and removing groups
        - adding new functions from other modules
    + setting up sphinx and fixing bugs while building html.
    + modified taxa/taxa.py to introduce a blank line (it was causing some unexpected output otherwise.)
+ Expanding README
    - included some more information regarding what is the aim of this project, where to go to resolve data quality issues.
+ Writing Jupyter Notebook - `depth_time_series.ipynb` [pull #42](https://github.com/iobis/pyobis/pull/42)
    + Jupyter notebook utilising `pyobis.occurrences` to gain insights on the change in depth with respect to time for different species of whales, tuna, sharks, turtles and some fishes. The analysis includes the change in depth, whether it is shift, compression or expansion. Some species have also witnessed conservation.
+ Fixed unexpected bug in docs workflow see [#48](https://github.com/iobis/pyobis/pull/48)
+ Found and reported issues with data quality in OBIS [see #45](https://github.com/iobis/pyobis/issues/45)

### Tasks working on
+ updating depth notebook
+ working on `migration_patterns.ipynb` jupyter analysis notebook