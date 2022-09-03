## The Afternoon

> If you have come untill here with me then I must thank you. Thank you for bearing with me and reading this blog from a very boring man! Or if you have come straight here without reading [the morning](./what-gsoc-taught-me-the-morning.md), then you must give it a read.

The clock is now ticking afternoon. It's time for us to time travel back to May 20th. 

I am into the coding period and the project board is in front of my eyes. I open VS Code and fetch changes from GitHub first. **This has been my daily routine throughout this summer. Nothing interesting? Yup, I just said it at first - I am very boring person. Nothing interesting, not all.**

But I had been working consistently on my project almost everyday. For the first third of the period I wasn't able to contribute much since I was busy with academics at my college. I had back-to-back 27 exams in around 60 days. Yes, college life is hard - but we are even harder!

This project is very closely aligned with my passion for conserving marine animals. Marine science interests me a lot more than any other subject (but not more than physics because I am a hardcore physics guy). Every single day I was led with passion and curiosity to do new experiments. As a part of my project I did:

+ **Fix the whole package at first**. To be honest the state at which I inherited the project was terrible. The code was totally broken, and the API updated to v3 while the package remained on v1. So, fixing all the broken links and adhering to the new API requirements was a major task which I undertook in the beginning of the period. My previous experience with the project during the pre-application period helped a lot, and I had already got two patches of fixes merged before the accepted applications were announced. 

+ **Bring in some cool features to the package**. Features are what makes a package cool to use. I implemented some cool features like bringing a progress bar while fetching occurrence records - it's quite a simple one yet does the very thing it was designe for; improve the way MeasurementOrFacts are rendered - the API returns them as a list of dictionaries but the package unnests it into a pandas dataframe and it does it like a pro; a response class for every module - now with a response class the user can not only fetch the data with the set parameters but also get the corresponding OBIS API URL and OBIS Mapper URL (for some functions) making their task really easy and giving a greater command over the requests they make.

+ **Some cool analysis and visualization with ocean data**. Biodiversity Data analysis was the coolest part of the project, to be honest. We just used the package we had improved and grabbed some interesting data for the analysis. I could produce 5 analysis notebooks with spatiotemporal analysis on themes ranging from ocean sunfishes to Measurement or Facts records, a time series analysis of species depth and an interesting migration pattern analysis. I also worked on a notebook exemplifying dataset contribution from a geo-temporal region of interest. In short, it was really interesting and amazing. [Go have a look at those cool plots and the data story.](https://github.com/iobis/pyobis/tree/master/notebooks)

+ **Bug fixes on the go**. You clearly know that bugs land up in development journey as mysteriously as ships dissapear from the Bermuda Triangle. How tedious they may be but bug hunting and fixing is always an interesting task. I had got a dozen of bugs during this journey let alone the ones which came up during local development. If you want to have a deep thought on the issues, [you can have it here](https://github.com/iobis/pyobis/issues?q=is%3Aopen+is%3Aclosed+author%3Aayushanand18+).

+ **Expanding the documentation and other info**. Package rebuilding was a heavy task but an even heavier task is to document the tasks. 