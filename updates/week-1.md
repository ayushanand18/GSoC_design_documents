# Week 1
## 13 to 19 Jun 2022
+ Weekly meet on 14 June.
    + **Agenda**:
        + Introductions and motivations
        + Deciding tasks that need to be done.
        + Getting Ready for GSoC, and setting up tasks and project boards, main communication channel.

### Tasks accomplished
+ Finishing migration of all modules and function to the new API.
    + Completed modifying occurrences module, as occ.grid() and occ.tile() were left from PR#8 and PR#11.
+ Finsished updating mof response in occurrences.search() function.
    + passing `mof=True` and `hasextensions='MeasurementOrFact'` in the search() now yields a list of pandas DataFrame objects making it easier for users to make use of this data.

### Tasks working on
+ Creating example usage for each module