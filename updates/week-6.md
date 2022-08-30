# Week 6
## 18 July to 24 July 2022
+ Weekly meet on 19 July.
    + **Agenda**:
        + Resolve all bugs as discussed in the [call](../notes/07-19.md).

### Tasks accomplished
+ Resolving bugs and initiating PRs for the same.
    + occurrence pagination (use default size 5000)
        - wrote a new function to enable fetching occurrence records iteratively, w/ and w/o user-specified limits
    + MoF accessibility (duplicate columns)
        - resolved duplicate column issue when fetching MoF records. Some columns like `scientificName` and `eventID` were being repeated when performing `inner_join` on normalized and non-normalized DataFrame.
    + MoF Null Records
        - Added a null-check function when accessing MoF records. Previously, accessing MoF records for species without any occurrence records resulted in an error.
    + added progress bar to occurrences.search function, so that when the records fetching process is informative.
    
+ Completing 1st Jupyter Notebook Analysis - `occurrence_ocean_sunfish.ipynb`.
    + completed writing notebook with experiments on ocean sunfish occurrence records.

+ Adding more information to the README and making it more beginner friendly
    + Since `pyobis` is an open-source project, there is a strong need to expand the README to include information related to, but not limited to:
    + Data Quality Issues reporting: If any user finds some issues with the data grabbed from `pyobis` it will be a natural instinct for him/her to open issues here. Therefore, README must contain relevant information regarding the right place to open issues.
    + Data Related Queries: If any user has some queries related to the data being returned by `pyobis` say pertaining to the fields returned with occurrence records then it might be wise to include links to the OBIS main page, contact page or some forum.
    + Update short examples contained in the README
    + Add link to `usage_guide.ipynb` and to `/notebooks/` folder for sample use case-analysis
    + Other changes: Changing the links that have gone obsolete, adding Further Reading material, adding link to CONTRIBUTING.md guide.

### Tasks working on
+ writing a progress bar to occurrence records fetch process.
+ Debugging flake8 linting
+ creating `depth_time_series.ipynb` - a time-series analysis for average depth for some species
    + an elaborate line plot with 3 or 5-year average also depicted.