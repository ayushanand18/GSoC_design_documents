# Week 2
## 20 to 26 Jun 2022
+ Weekly meet on 21 June.
    + **Agenda**:
        + PR over existing changes
        + dropping obisDownload from pyobis/occurrences
        + Setting up project boards and objectives segragation before deadline.

### Tasks accomplished
+ Writing examples usage for each module.
    + Wrote input parameters description, sample input and expected output for occurrences, and taxa module.
+ Improving MoF records accessibility by unnesting the JSON input into pandas dataframe
    + each occurrence has a unique ID (at least for IPT controlled records) so we perform an inner join
    between unnested and nested data.

### Tasks working on
+ Writing examples for checklist, dataset, nodes modules