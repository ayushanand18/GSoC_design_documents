# Week 11
## 22 August to 28 August 2022
+ Weekly meet on 23 August.
    + **Agenda**:
        + update the changelog
        + update the dataset contributions notebook
        + create a response class
        + make a github release, conda-forge release till the time we do a PyPI release

### Tasks accomplished
+ `[feature-update]` created response class for each module
    + A response class in each module has
        + an `__init__` function (to initialize but no specialized function to do
        + all existing functions as methods to the class
        + `get_search_url` returns OBIS API URL for the query
        + some functions have `get_mapper_url` methods to get OBIS Mapper URL, we identify functions to show a mapper url using a `self.mapper` flag (if true for a method then it has a corresponding Mapper URL).
        + docstrings have also been updated
    + Additional Changes
        + Tests have also been updated. Wrote tests for new methods and an extensive testing to check whether returned url do really exist have been introduced. I believe this will make this package more robust.
        + Updating docs for all modules as per new feature updates.
+ finished writing `contributions_quantification.ipynb` notebook.
    + completed analysis on how much dataset owners have contributed to the OBIS ecosystem by publishing by
        + temporal distribution analysis
        + spatial distribution analysis
        + taxonomic distribution analysis
        + MoF analysis
+ updated the changelog and upgradded version for the package
    + also changed the `Development Status` to `4 - Beta` for PyPI

### Tasks working on
+ working on PRCRMP biodiversity notebook
    + recreating the map graphic
+ adding `dna` field to `occurrences.search()`
+ creating a response class
+ 