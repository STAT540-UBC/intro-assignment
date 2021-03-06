Practice assignment
================

Welcome to STAT540!

The point of this assignment is to get you warmed up with git, GitHub,
markdown, and R so you’re more prepared for the future assignments. The
first few seminars will cover all you need to know for completing this
practice assignment.

Note that this practice assignment, just like your 30pt assignment, will
need to be done in Rmarkdown (.Rmd) because it requires R code. You can
start with the .Rmd version of this file, and fill it in where
necessary. Note that Question 1 asks you to add an additional file.

If you have never used R, some resources can be found via [this
page](https://support.rstudio.com/hc/en-us/articles/201141096-Getting-Started-with-R).
There are [hundreds of
tutorials](https://www.google.ca/search?q=R+tutorial) around the web.

And if you just want to hack away and try to manage just with the
built-in help (type `?` before a command, like `?read.table` and you can
even get help for things like `[` or `+` if you surround it with quotes
`?"["`), a pro tip is if you get a cryptic error message, just paste it
into a web search.

## QUESTION 1: Create a README in your repo (1pt)

Once you have accepted this assignment through the Canvas invite link
and have a repository set up (in the format of
`STAT540-UBC-2022/intro-assignment-yourgithubID`), you can start
personalizing it by creating a README.md file. This would help people
who visit your repository understand who you are and what your
repository is about.

Please be sure that your markdown is properly formatted. See this
[markdown
reference](https://guides.github.com/features/mastering-markdown/) from
GitHub if you need help getting started.

Add some information to this README.md file to introduce yourself to the
teaching team. Some things you may wish to include:

-   Your name, your program
-   Links to other profiles (Twitter, LinkedIn, personal website, other
    relevant links, etc)
-   What do you hope to achieve in this course
-   What this repository is for (example: “This repository contains the
    intro assignment for STAT540”)
-   Anything else that you want. You can add emoji, too!

## QUESTION 2: Data inspection with R (2pt)

When answering the following questions, please always “sandwich” your R
code with some text. Ensure fluency by avoiding inserting R code or
outputs without any explanation. For example, if the question ask you
what x + y given x=1 and y=2, you can answer it like this:

------------------------------------------------------------------------

Now we want to find the sum of x and y.

``` r
x <- 1  # Note how I assign them to variables instead of just priting 1+2
y <- 2 
z <- x + y
z # By doing this, I can print out the output of z. Alternately, you can also do (z <- x+y). 
```

    ## [1] 3

Conclusion: we found that the z is 3. \<—- (and here I’m using inline R
code)

If you are looking at the .Rmd of this file (the Rmarkdown that creates
this markdown you’re looking at), and click on “Raw”, you’ll see that I
have used inline R code to refer to the variable “z” instead of directly
typing “3”. This is because if we ever need to change the values of x
and y, we could possibly forget to update “3” as well. You can imagine
that if you have to change the initial inputs of a long statistical
reports, all your numbers in the rest of the report will change. You
don’t want to have to look through every sentence to make sure that your
report is still up-to-date.

By using variables and inline R code, I can change the value of x and/or
y, and rest assure that when I re-knit my Rmarkdown, my conclusion
statement will be updated.

There are some [data
sets](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/00Index.html)
in base R for you to play around with. We will explore the Titanic
dataset. You can view it by typing `Titanic`. Just like with functions,
you can use the question mark `?Titanic` to see more information about
the dataset.

Answer the following questions by subsetting, printing out the result or
by graphing.

### 2.1 Passenger breakdown

Convert the array into a data frame by using `data.frame()` function.

-   How many children and adults were on Titanic?
-   Were there more female adult or male adult passengers?

Find the answers these questions by adding code to the code block below.

``` r
# YOUR CODE HERE
```

Replace this text with an explanation of your code output to answer the
questions.

### 2.2 Survival

Using the same data frame, examine the survival rates.

-   Did the children have better survival rate than the adults?
-   Which class of passengers have a better survival rate? (Crew, first
    class, second class, third class)

Find the answers these questions by adding code to the code block below.

``` r
# YOUR CODE HERE
```

Replace this text with an explanation of your code output to answer the
questions.

## 3. Data visualization (1.5pt)

Here you’ll practice reading data from a text file and do some graphing.
The file
[“guinea_pig_tooth_growth.txt”](https://raw.githubusercontent.com/STAT540-UBC/intro-assignment/main/guinea_pigs_tooth_growth.txt)
is actually the same data as the dataset `ToothGrowth`. You can use
`?ToothGrowth` to see what it’s about. However, use `read.table` to read
this file into a data frame for this question.

-   Create a figure for this dataset (choose whatever graph you’d like!)
-   Explain how your graph is informative: what does it tell you about
    the result of the experiment? Also explain why you choose to present
    the data in this way.

Add code to the code block below to complete these tasks.

``` r
# YOUR CODE HERE
```

Replace this text with an explanation of your code output to answer the
question.

## 4. Mechanics (0.5pt)

This check is for the “quality” of this assignment. Check out the
[assignment
tips](https://stat540-ubc.github.io/submission_guide.html#general-tips-for-working-on-the-assignments)
if you’re not sure what that means. Basically, it’s important to write
up organized reports that are clear and easy to follow, so that your
collaborators and the future you can understand what you are doing. The
elements that make up a good report include (not limited to):

-   Properly labeled graphs
-   Well-formatted markdown (use of headings, subheadings, and numbering
    that makes sense)
-   No inexplicable R outputs (example: printing out an entire dataframe
    unnecessarily when one can simply use `str()`)
-   Codes are commented when needed
-   No broken code.

We will also evaluate this part by looking at :

-   Rmarkdown is properly knitted: markdown is created and easy to read
    on GitHub, figure folder is there, etc.
-   all the files associated with this assignment are present in a
    subfolder (this happens automatically by default).

Be sure to commit and push your completed assignment before the
deadline. Anything submitted or modified after the deadline will not be
marked.
