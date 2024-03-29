## The Afternoon

> Published on Medium.com [here](https://medium.com/@theayushanand/my-experience-of-gsoc-2022-with-ioos-part-2-1496061f9880)


> If you have come untill here with me then I must thank you. Thank you for bearing with me and reading this blog from a very boring man! Or if you have come straight here without reading [the morning](./what-gsoc-taught-me-the-morning.md), then you must give it a read.

The clock is now ticking afternoon. It's time for us to time travel back to May 20th. 

I am into the coding period and the project board is in front of my eyes. I open VS Code and fetch changes from GitHub first. **This has been my daily routine throughout this summer. Nothing interesting? Yup, I just said it at first - I am very boring person. Nothing interesting, not all.**

But I had been working consistently on my project almost everyday. For the first third of the period I wasn't able to contribute much since I was busy with academics at my college. I had back-to-back 27 exams in around 60 days. Yes, college life is hard - but we are even harder!

This project is very closely aligned with my passion for conserving marine animals. Marine science interests me a lot more than any other subject (but not more than physics because I am a hardcore physics guy). Every single day I was led with passion and curiosity to do new experiments. As a part of my project I did:

+ **Fix the whole package at first**. To be honest the state at which I inherited the project was terrible. The code was totally broken, and the API updated to v3 while the package remained on v1. So, fixing all the broken links and adhering to the new API requirements was a major task which I undertook in the beginning of the period. My previous experience with the project during the pre-application period helped a lot, and I had already got two patches of fixes merged before the accepted applications were announced. 

+ **Bring in some cool features to the package**. Features are what makes a package cool to use. I implemented some cool features like bringing a progress bar while fetching occurrence records - it's quite a simple one yet does the very thing it was designe for; improve the way MeasurementOrFacts are rendered - the API returns them as a list of dictionaries but the package unnests it into a pandas dataframe and it does it like a pro; a response class for every module - now with a response class the user can not only fetch the data with the set parameters but also get the corresponding OBIS API URL and OBIS Mapper URL (for some functions) making their task really easy and giving a greater command over the requests they make.

+ **Some cool analysis and visualization with ocean data**. Biodiversity Data analysis was the coolest part of the project, to be honest. We just used the package we had improved and grabbed some interesting data for the analysis. I could produce 5 analysis notebooks with spatiotemporal analysis on themes ranging from ocean sunfishes to Measurement or Facts records, a time series analysis of species depth and an interesting migration pattern analysis. I also worked on a notebook exemplifying dataset contribution from a geo-temporal region of interest. In short, it was really interesting and amazing. [Go have a look at those cool plots and the data story.](https://github.com/iobis/pyobis/tree/master/notebooks)

+ **Bug fixes on the go**. You clearly know that bugs land up in development journey as mysteriously as ships dissapear from the Bermuda Triangle. However tedious they may be, but bug hunting and fixing is always an interesting task. I had got a dozen of bugs during this journey let alone the ones which came up during local development. If you want to have a deep thought on the issues, [you can have it here](https://github.com/iobis/pyobis/issues?q=is%3Aopen+is%3Aclosed+author%3Aayushanand18+). To be precise, I opened 9 issues throughout the length of the project and worked on at least 27 of them directly.

+ **Expanding the documentation and other info**. Package rebuilding was a heavy task but an even heavier task is to document the work done. During the project I worked on expanding the information we deliver on the project README by adding about the package, how to report issues, where to report for data quality issues, etc; plus we also added a CONTRIBUTING.md to the project repository so as to serve as a guiding principle for all fresh contributors. The guidelines included where and how to start contributing, filing bug reports, creating PRs, the code of coduct and others with some excerpts adapted from Facebook's guidelines. 

+ **Some intriguing experiments and those doubts**. I have a habit, the habit of experimenting with things. I don't if this is good or terrible, but it keeps me interesting into things. I experimented a lot with the package I was rebuilding, the OBIS API, and the OBIS Mapper. And each time I used to monitor the network logs and look at what was actually being done in the background. To my surprise, I found so many endpoints and things that was not documented but was very very useful for us. So, I brought up issues for them and also suggested some crazy ideas. Part of which were accepted and the rest tabled on for further discussion. Open Source is all about communication, it's the pillar behind an amazing OSS.

+ **The release**. Apart from those massive changes, we could also manage a release on both GitHub and PyPI. That was a great moment for us. Bringing the package to a shape, piece by piece, arranging and cleaning up all blocks and finally releasing the package so close to the heart is mesmerizing. 

If you want to know about all the changes we had done, watch out for [the list of PRs opened by me](https://github.com/iobis/pyobis/pulls?q=is%3Apr+is%3Aclosed+author%3Aayushanand18). Interestingly, I opened 29 pull requests and still counting. You can also [checkout the release notes here](https://github.com/iobis/pyobis/releases/tag/1.2.6).


On top of this, I learnt some amazing development stuff, including:
+ **Pre-commits**. I didn't know anything about pre-commits before this project. They are just as cool as anything. We had linting, code coverage tests, PEP 8 complaince tests, everything on the pre-commit - and it was really amazing. I learnt it for the first time!
+ **Project Board on GitHub**. I had never used project boards on GitHub before and it was a great experience. Issue tracking, milestones, progress tracking everything closely related to the GitHub workflow and super easy to sync with.
+ **git rebase**. To be very honest, this was the best thing that I had learnt to use with ease during this project. Git PR workflow has its basis on this one single powerful tool. But if not used correctly it can ruin your project. Thanks to my mentor, (@7yl4r) I learnt the intricacies of `git rebase` and it became a powerful weapon in my hand.

> Over and above all, those weekly calls every Tuesday were great and filled me with enthusiasm. During those calls, we used to brainstorm on some technical aspects of the project as well as what to do next. We used to discuss interesting ideas, and in each call I used to learn something really new and incredible. In the call we had in the 11th week, we got all my mentors join in and it was so amazing meeting with such great minds that it will be forever etched in my memory. I'm just flooded with emotions at this time. Words have failed me. 

Even if we might have got short of words but we do have the clock with us pointing now towards the evening. I hope you are enjoying the journey so far with me, and if you are not I'm really sorry. I didn't intent to bore you but I do request you [to read the continual part "the evening".](./the-evening.md)
