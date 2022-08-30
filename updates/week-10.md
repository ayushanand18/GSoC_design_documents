# Week 10
## 15 August to 21 August 2022
+ Weekly meet on 16 August.
    + **Agenda**:
        + update the docs
        + focus on new notebooks
        + does OBIS allow searching with metadata

### Tasks accomplished
+ Fixed some issues in the pagination process
    + Issue [#45](https://github.com/iobis/pyobis/issues/45) might have been a direct cause of the missing `after` parameter while doing the pagination process. Fixed that issue with PR [#64](https://github.com/iobis/pyobis/pull/64).
+ Updated `docs` badge on README and elsewhere, removed redundant examples from the README because it was already present in `docs` as well as `usage_guide.ipynb` notebook.
+ Fixed a formatting error in the docs due to missing new lines in the docstrings for taxa.py. see [#65](https://github.com/iobis/pyobis/pull/65)

### Tasks working on
+ working on dataset contribution notebook
+ writing tests for duplicate occurrence records
+ recreating a map
+ working on species co-occurrence analysis