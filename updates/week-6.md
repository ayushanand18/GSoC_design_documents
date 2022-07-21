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

+ Completing 1st Jupyter Notebook - `occurrence_ocean_sunfish.ipynb`.
    + completed writing notebook with experiments on sunfish occurrence records.

### Tasks working on
+ writing a progress bar to occurrence records fetch process.
+ Debugging flake8 linting
+ creating `depth_time_series.ipynb` - a time-series analysis for average depth for some species
    + an elaborate line plot with 3 or 5-year average also depicted.