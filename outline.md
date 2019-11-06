
# 0-Intro

Data is the present.

It is not the future, not something that we must prepare for. Data is the present. Most sectors today produce and deal with masssive datasets and databases. And the same is for research: at this moment data are cheap to come by, eterogeneous and everywhere.


# 01 - Let's make an histogram


Read the data into an R object and store it into a variable.

## Load the data in an R object and store it in a variable

Sorry, this part might be a bit boring, but R is the tool for data science.

And to do any data science of it, you must first familiarize with the tool.

I'll try to give you a very minimal introduction to R, oriented to data exploration and data science. But you'll need to learn a bit of R programming anyway.

### Objects

- Everything in R is an object:
  - r understands what you tell it,
  - everything is an object, and it has a class,
  - vectors collect objects of the same class,
  - We will skip matrices, everything else is a list.
  - list can be nested.
  
### Variables

- Unquoted text is interpreted as a variable
  - you can store in them any object you like
  - Once you call the variable it returns the object you associated to it,
  - Some variables are already occupied!

Check the variables with already data associated to them (in Rstudio), reflections on the Rectangular data format.
Introduce concept of tidy data.

### Rectangular Data

- Rectangular data, and rectangular data in R
  - most obvious and "commmon" form of data,
  - While you explore your data, eventually you will transform you data into rectangular.
  - dataframes (and tibbles come from lists column wise - thus each column is a vector.
    Each column has the same class, makes sense from a data point of view: would you build 
    a dataset rowise?)
  - But how would you import some data from outside R into R? You need functions.
  
### Functions

- In R you do everything with functions:
  - Some variables already store functions.
  - You can inspect the body of the function, often it is just a collection of R codes... 
    it calls other functions.
  - a function takes some argument and returns an output.
  - documentations: manual pages, vignette, websites, articles/blog posts, books
  - you can provide a variable as an argument and save the output in another variable.
  

### Functions in packages

- Why do we need to install packages
  - You have primitive / low level functions and various levels of high levels function,
    often redundant [readLines, read.csv, read_csv].
  - Packages are a collection of functions (and metadata and documentation),
  - Primitive and internal functions are the building blocks of R and generally are written in C,
  - You can do everything with those building blocks, but we want our life easier, so we can use some blocks that are already assembled,
  - Those assembled block are the functions in packages,
  - Example, you need to import a CSV file in R --> readLines is primitive.
  - But you can call read.csv that read the lines as if they were a CSV,
  - or read_csv, newer version.
  
### You can write your own function

Better explained with scheme.

## Put it together 

Read the data into an R object and store it into a variable.

Resource :https://evamaerey.github.io/ggplot_flipbook/ggplot_flipbook_xaringan.html


# 02 - Analyze data with the tidyverse

- Do you know what high level programming is?

- Tidyverse is a collection of high level packages and functions for data science!
  There are others, pick the one best suited for you. https://www.tidyverse.org/packages/
  
- I will not introduce them one by one because we must use to analyze data we must use them together. 

- I will not go in detail on bioinformatics and bioconductor (the other huge ecosystem of packages in R) because this is more generic and fundamental. Once you get the basic data exploration right, it is easier  to switch to bioconductor

## Dataset

NY Squirrel census: https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-10-29

Because:

- It is large enough to provide a challenge.
- It is tidy and detailed,
- It stores quantitative and categorical variables,
- it stores spatial variables,
- it stores time variables.


## Basic exercises of data manipulation

Afterwards:

## With plots you can see things more clearly

Graphical representation of data is a powerful tool to explore them.

GGplot2 is one of the most powerful data visualization libraries available.

It's not your only choice for data vis in r, but we will focus on it only, because it's the most widely used.

Layered Grammar of Graphics.

Compare ggplot2 and D3

# Data cleaning

This datatset has great examples of data cleaning

https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-11-05

# Practical session

Explore your own dataset.

1. Select a dataset, I will provide three of them. But feel free to choose one of your own if you prefer.

  - In case, take care that it is a tamed dataset,
    https://rstudio-pubs-static.s3.amazonaws.com/396363_adaf67178eab4bd793bd9dd17dda70b3.html
    https://r4ds.had.co.nz/tidy-data.html

2. Familiarize yourself with the topic. Know at least just a bit of what the dataset is about.

3. Do you have a description of all the columns in the dataset?
  - If you don't have this information, can you gather it?
  - Do those description match what you observe in R? If not, what does not match?
    - Is it an issue of how the data are loaded? Can you fix it?
    
4. Are the data tidy?
  - Are there NA? How are NA encoded?
  - Do the column have practical names, do they need renaming?
  - Do the data are structured according to the tidy principles, do they need spreadong/gathering?
    
    - Each variable must have its own column.
    - Each observation must have its own row.
    - Each value must have its own cell.
  
  
5. How are the variable distributed? If they are categorical which level do they have.

6. Do you have hypothesis on what is the main information hidden in the dataset? Do you know how to find it?



