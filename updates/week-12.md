# Week 12
## 29 August to 4 Sept 2022
+ Weekly meet on 30 August.
    + **Agenda**:
        + fun fact: the project in the organisation that had the most number of commits
        + maybe the last meeting before deadline? it feels a bit weird and sad to ask but shall we meet next week?
            + thats great we can meet next week.
        + GitHub permissions for renaming the branch. -> **ask Pieter**
        + feature update discussion
            + will update all docs after this update
            + will update all notebooks after this update
            + will update changelog as well -> **will do so**
        + OBIS Manual here, can document your issues here:
            + https://github.com/iobis/manual/pull/57
        + MBON Pole to Pole notebook -> **can recreate this notebook**
        + Filipe will help create a PyPI release and then a conda-forge release with the recipe.
        
        + should we implement issue #54 (Undocumented countryid parameter for occurrences/grid endpoint)
        and #55 (showing suggestions for possible results for a search query) ? The latter one has been
        resolved partly by the response class feature update. One more part is having suggestions from dataset
        names. -> **#54 need to connect with Pieter, wait for more discussion.**

        + final submission how do I? I read guidelines from Google and they recommend anything from a blog post,
        a GitHub gist, a website etc and get that approved from the mentors. We were continously updating the 
        design documents repo and I have published it as a GitHub pages blog. How does this sound? 
        -> **need to write a blog post, and maybe divide into two parts - how the project was etc, and what learning did you have from it?**

        + we might need to look at the issues page and figure out what to resolve?
            + maybe #52 into utils library -> **further discussion, let's keep this open**
            + what to do with #36 -> **further discussion is needed, let's keep this open**
            + what to do with #61. If we keep JSON response the process will be faster since we fetch JSON data and append it to the already fetched data. Now we start converting to pandas dataframe in between it will consume both space and time. My personal opinion what do you feel? -> **convert occurrences.search to pandas dataframe object only because developers love to see the raw API response but researchers want the tables directy**
            + for #72 might be useful for us. this was something adapted directly from pygbif but wasn't implemented. Insights:
                + this list is not updated one (as far as I know) because there exists at least one error code which is not documented here. See this query https://api.obis.org/occurrence?scientificname=ayush
                Response is ```{"total":0,"results":[],"error":"NAME_NOT_FOUND"}```
                + we can update it (but I don't know where to look at for the updated list and personally I don't know much about the error codes that OBIS uses) and document it in docs as a seperate function so that it can help people identify the error themselves. The codes are more or less self-explanatory as well. -> **we can remove it**
            + #75 is resolved I suppose, I have updated the docstrings accordingly. **done**
            + no need to have that .to_pandas function. **discussion concluded**
            + #69 and #70 are also done I believe. **PR is approved but yet to merge**
            + we need to work on #17, #29, and #75 specifically. **yes finally PyPI is here. Hurray!**
        
        + write a blog post on your experience, the state you inherited and the state you'll be leaving.
            + inspo https://lohithmunakala.medium.com/seafloor-sampling-and-data-demo-center-jupyter-book-migration-gsoc21-ioos-a9930abc4c42
            + write the stumbling blocks, where did you feel stuck in your journey and how did you overcome?
        + once we rename master -> main, can update the fork as in [here](https://github.com/ioos/ioos_code_lab/pull/20#issuecomment-918516941)

### Tasks accomplished
+ making changes to the `feature update` and iterating over feedback
    + renamed class name for each module
    + created superclass `OBISQueryResult` and added some inherited functions which inherently common 
    in all other modules.
+ update `/docs/` after the feature update
    + improved the documentation and examples

### Tasks working on
+ adding `dna` field to `occurrences.search()`
+ update the docstrings in module files.
+ change occ.search behaviour and bring in consistency by returning pandas dataframe only
