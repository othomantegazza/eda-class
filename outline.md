
# 0-Intro

Data is the present.

It is not the future, not something that we must prepare for. Data is the present. Most sectors today produce and deal with masssive datasets and databases. And the same is for research: at this moment data are cheap to come by, eterogeneous and everywhere.


# 01 - Let's make an histogram

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

- Rectangular data, and rectangular data in R
  - most obvious and "commmon" form of data,
  - While you explore your data, eventually you will transform you data into rectangular.
  - dataframes (and tibbles come from lists column wise - thus each column is a vector.
    Each column has the same class, makes sense from a data point of view: would you build 
    a dataset rowise?)
  - But how would you import some data from outside R into R? You need functions.
  
- In R you do everything with functions:
  - Some variables already store functions.
  - You can inspect the body of the function, often it is just a collection of R codes... 
    it calls other functions.
  - a function takes some argument and returns an output.
  - documentations: manual pages, vignette, websites, articles/blog posts, books
  - you can provide a variable as an argument and save the output in another variable.
  - You have primitive / low level functions and various levels of high levels function,
    often redundant [readLines, read.csv, read_csv].
  - Packages are a collection of functions (and metadata and documentation)



  - how to assign an object to a variable,
  - Every object has a type,
  - We will use mostly tibbles, which are rectangular data,
- To do anything, you need functions:
  - what is a function? Take input, makes steps, give outputs.
  - you can write a function, or see what a function does.
  - We find functions in packages,
- Packages are a collection of functions and documentation.
  - You can install packages from CRAN,
  - Load the packages to use the functions.
  
### Rectangular Data:

- Rows and columns,
- in R they work columnwise,
- concept  of tidydata.

## 02 - Let's make a scatterplot

### Manipulate Data

- how do you modify data in R,
- Many ways to do one thing - open source,

### DPLYR

- Tell your computer how to achive what you want vs declarative language. (SQL)
- Common dplyr verbs (function),
- the pipe

## GGPLOT2

- what does it mean to do a plot
- Map data to aesthetic property of geometric objects,
- layered elements
- theory of graphical data visualization.