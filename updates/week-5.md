# Week 5
## 11 July to 17 July 2022
+ Weekly meet on 12 July.
    + **Agenda**:
        + do away with the coveralls badge.
        + break the next PR into two, one each for `usage_guide.ipynb` and the other for `occurrences_ocean_sunfish.ipynb` similar to [IOOS Codelab Notebook for r-obis](https://ioos.github.io/ioos_code_lab/content/code_gallery/data_access_notebooks/2018-02-20-obis.html)
        + find more use case for Jupyter Notebooks
        + if multiple packages to install, then run a for loop for each package.

	        ```python
            try:
                    import owslib
                except:
                    !pip install owslib
            ```

### Tasks accomplished
+ Created tutorial usage notebook for modules, and initiating a PR.
    + created sample usage, explained input parameters. Ran an example query and
    explained displayed as well for all modules - occurrences, checklist, dataset,
    nodes and taxa.
+ Done away with the coveralls badge (which had become obsolete)

### Tasks working on
+ creating `occurrence_ocean_sunfish.ipynb`
    + a Jupyter Notebook to research on spatial, temporal distribution of Mola Mola (commonly
    known as the Ocean Sunfish.)
    + can be found [at](https://github.com/iobis/pyobis/blob/master/notebooks/occurrence_ocean_sunfish.ipynb)
+ working on another Jupyter Notebooks for time-series species depth analysis.