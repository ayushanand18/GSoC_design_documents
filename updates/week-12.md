# Week 11
## 29 August to 4 Sept 2022
+ Weekly meet on 30 August.
    + **Agenda**:
        + `Ayush`
        + maybe the last meeting before deadline?
        + feature update discussion
            + will update all docs after this update
            + will update all notebooks after this update
            + will update changelog as well
        + should we implement issue #54 (Undocumented countryid parameter for occurrences/grid endpoint) 
        and #55 (showing suggestions for possible results for a search query) ? The latter one has been
        resolved partly by the response class feature update. One more part is having suggestions from dataset
        names.
        + final submission how do I? I read guidelines from Google and they recommend anything from a blog post,
        a GitHub gist, a website etc and get that approved from the mentors. We were continously updating the 
        design documents repo and I have published it as a GitHub pages blog. How does this sound?
        + we might need to look at the issues page and figure out what to resolve?
            + maybe #52 into utils library 
            + what to do with #36
            + what to do with #61. If we keep JSON response the process will be faster since we fetch JSON data and append it to the already fetched data. Now we start converting to pandas dataframe in between it will consume both space and time. My personal opinion what do you feel?
            + for #72 might be useful for us. this was something adapted directly from pygbif and still not implemented. To be noted:
                + this list is not updated one (as far as I know) because there exists at least one error code which is not documented here. See this query https://api.obis.org/occurrence?scientificname=ayush
                Response is ```{"total":0,"results":[],"error":"NAME_NOT_FOUND"}```
                + we can update it (but I don't know where to look at for the updated list and personally I don't know much about the error codes that OBIS uses) and document it in docs as a seperate function so that it can help people identify the error themselves. The codes are more or less self-explanatory as well.
            + #75 is resolved I suppose, I have updated the docstrings accordingly.
            + #69 and #70 are also done I believe.
            + we need to work on #17, #29, and #75 specifically.

### Tasks accomplished
+ making changes to the `feature update` and iterating over feedback
    + renamed class name for each module
    + created superclass `OBISQueryResult` and added some inherited functions which inherently common 
    in all other modules.
    
### Tasks working on
+ adding `dna` field to `occurrences.search()` 