# DSI Project Style Guide

_Tim Dwyer_

Your projects will become your portfolio. That means that every project that you turn in should be considered part of your resume and a direct reflection of how you are likely to perform as an employee. Take your projects seriously now and you will finish the course with a portfolio that you can feel proud to apply with.

**You do not know where recruiters will focus in your projects. This means that every aspect of your project should be equally exceptional.**

## Have a structural plan for your project.

Having a plan for your project means more than having multiple notebooks. Notebooks should be separated for a reason.

A great reason for starting a new notebook is that you have completed the task at hand and are moving on to another, possibly related, task.

For example, data collection (i.e. web scraping or querying an API) and storage (saving data to a `.json` or `.csv` file, inserting into a database etc.) could be done in one notebook which is followed by another for data processing and some initial exploratory data analysis.

Somewhere there has to be an explanation of what purpose every single file and directory serves. `README.md` files within different directories are a great place for this.

You should tell the reader what you're doing in a notebook. This sounds repetitive, and it is, but a nice framework for this could be something like the following:

1. At the beginning of each notebook, explain what you're going to do in this notebook and how it is the natural next step from the previous notebook.
1. At the end of each notebook, explain what you have just done in this very notebook.
1. After explaining what was done in this notebook, give an idea of where you're going (what you'll be doing in the next notebook).
1. Every time you start a new task or make a new decision for modeling, data processing and cleaning, write at least one sentence explaining why you did this. I do not mean that every line of code requires a sentence of explanation. You will have to use your judgment to measure the "Number of decisions you've made in your code".

## Edit your work.
1. Remember all those explanations scattered throughout your notebooks? Ensure that they are grammatically correct and without spelling errors.
1. You should also edit your code! Are you importing every module you've ever used in every notebook? Stop doing that! Only import modules you use. Are you defining functions/variables that you never use? Stop doing that! By re-reading and editing your code you can find these unnecessary (and incredibly confusing) pieces of code and remove them. There are some tools that will do this for you automatically, but these tools are not very well developed for notebooks.

## Assume that the reader does not know what you're doing or why.
1. These projects are a part of your public portfolio. They will, with any luck, be read by technical recruiters and hiring managers. Assume that the reader is a technically minded person who is, explicitly, not a data scientist.
1. The reason for this framing is not that a data scientist will never read your projects, rather that others may as well. If you write for the more general audience, more people will be able to -- at least somewhat -- understand your work.

## README
1. A README was mentioned above as a way to describe the contents of each of the files and directories in your repository. READMEs will render in Github for any directory they're in (so feel free to include one in **every** directory).
1. **Use markdown in your README.** It takes only a minute to add this formatting and results in a *much* clearer document. Don't know how to markdown? [Check this out](https://help.github.com/articles/basic-writing-and-formatting-syntax/).
1. The landing page for your project (the main directory) should have an executive summary. What should this include?...

## Executive Summary
1. Problem statement
    - **S**pecific
    - **M**easurable
    - **A**chievable
    - **R**elevant
    - **T**ime-bound
2. Description of data
    - REQUIRED: Size (samples & features)
    - REQUIRED: Source (provide a link to the original source if possible, or describe how/where you acquired it)
    - REQUIRED: Target (classification/regression/unsupervised)
    - RECOMMENDED: Data dictionary (describe every feature in your data set, or at least those features that were prominent in your final model)
    - Consider including a plot or two from your EDA
3. Model performance on training/test data
    - Did you fit many models? Feel free to summarize some of your scores here.
    - Consider useing a markdown table to make results easy to review.
    - It should be clear which model you chose for production and why.
4. Primary findings/conclusions/recommendations
    - These should follow from your project
    - You should provide an answer to your problem statement
5. Next steps
    - **Always** focus on the positive (it's not what you did wrong, it's what you look forward to improving).
    - Is your model ready for production? Probably not, but you can comment on how it might get there.
    - Does this project demonstrate skills that you think could be applied to similar problems?

## Please write your code in REUSABLE functions.

Writing code in functions serves many purposes, but for the purpose of these projects I want to focus on two.

1. Writing functions to perform individual tasks will clarify, to you as well as the reader, what each line of code is doing. Just like how we use separate notebooks to allow readers to keep distinct tasks separated in their minds, functions can serve an identically helpful organizational purpose.
1. When you are interviewing, you will absolutely be expected to write functions since that is how code is, in practice, written and used. It is genuinely a very important part of writing code.
