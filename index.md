# GSoC 2022 with IOOS

Believe me, GSoC is an amazing experience every developer must have. 
It not only helps you get into Open Source as a beginer but its twelve
weeks are so mesmerizing that you will never stop contributing to Open
Source ever in your life.

## Table of Contents
+ [Before we start](#before-we-start)
+ [My Project](#my-project)
    + [Introduction](#introduction)
    + [Overview of the project](#overview-of-the-project)
+ [About me](#about-me)
+ [My tryst with Google Summer of Code 2022](#my-tryst-with-gsoc-2022)

## Before we start
Before we start talking about the project and the intricacies involved, there are people who deserve
the first mentions!

Thanks a ton to my mentors - **Tylar Murray** (@7yl4r), **Mathew Biddle** (@MathewBiddle), and **Filipe Fernandes** (@ocefpaf). They are so helpful that my whole journey through GSoC was as amazing as it
could ever be. 

And special thanks to **Google** for conducting such an amazing program every year! 
Thank you so much everybody, to all python developers, GitHub developers and everybody else on Earth
who created every tool I am using everyday!

## My project
> Making ocean biodiversity data easily accessible with python (pyobis revamp)

### Introduction
[pyobis](https://github.com/iobis/pyobis) is an interesting python package that helps users
fetch data from OBIS API which holds a great amount of ocean open-data, with ease. This project
is intended to update the existing pyobis python package to use the new OBIS API v3 and ensure 
the package is used for product generation in the future.

The pyobis package is really powerful and can fetch huge records of marine species,
particularly in the indo-pacific ocean region, and regions near the US, UK, and Australian
coastline. It is interesting to note that OBIS also holds data for species even dating back to
around 1078 AD, which makes pyobis even more essential to be maintained.

### Overview of the project
Due to major changes in OBIS API over these years, `pyobis` package stopped functioning. My goal in this project
was to get it back to a working stage and then carry on from there to implement new features and resolve issues.
I also brought out interesting visualization and analysis using this package in my Jupyter Notebooks, and
now they are a part of the official dev package to help researchers gets started with using it.

During each step, I was motivated to do three things,
+ look at the package from the user's point of view and make it the most friendly as it could be
+ work on what hasn't been done before. Do something new everytime.
+ code, test, document, and repeat. It's an Open Source project and so my view must be as readable to 
    the community as much as it can be

During the course of my project I found many bugs, and issues, fixed them and got engaged in very 
informative and interesting communications with the community.

## About me
Oh! The most interesting thing about me is that I am very boring. Still if you'd like to know
more about me [LinkedIn](https://linkedin.com/in/theayushanand) and [GitHub](https://github.com/ayushanand18)

## My tryst with GSoC 2022
Here is my tryst as Google Summer of Code 2022 participant with IOOS (Integrated Ocean Observing System).
+ [You can see the weekly agendas, accomplishments and updates on this page](updates)
+ [Here is the list of PRs opened by me](https://github.com/iobis/pyobis/pulls?q=is%3Apr+is%3Aclosed+author%3Aayushanand18). Interestingly, I opened 30 pull requests and still counting.
+ [The issues I opened](https://github.com/iobis/pyobis/issues?q=is%3Aopen+is%3Aclosed+author%3Aayushanand18+). To be precise, I opened 9 issues throughout the length of the project and worked on at least 27 of them directly.
+ [My experience and key takeaways](./updates/README.md#key-takeways)
