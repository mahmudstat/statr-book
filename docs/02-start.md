# Getting Started with Statistics and R {#start}

## Segment 01

### What is Statistics? 

The term has got three different meanings. 

- **Plural of the term statistic**, which refers to any function of sample values, for example, $\bar x = \frac {\sum_i^n x_i} n$
- **Table of values**


Table: (\#tab:unnamed-chunk-1)A Subset from Iris Data Set

| Sepal.Length| Sepal.Width| Petal.Length| Petal.Width|Species |
|------------:|-----------:|------------:|-----------:|:-------|
|          5.1|         3.5|          1.4|         0.2|setosa  |
|          4.9|         3.0|          1.4|         0.2|setosa  |
|          4.7|         3.2|          1.3|         0.2|setosa  |
|          4.6|         3.1|          1.5|         0.2|setosa  |
|          5.0|         3.6|          1.4|         0.2|setosa  |
|          5.4|         3.9|          1.7|         0.4|setosa  |

- **Technique of dealing with data**
  + Collection
  + Organization
  + Analysis (such as *regression analysis*)
  + Interpretation
  + Presentation
  

### Statistics vs Data Science

Statistics deals mainly with analyzing and interpreting data, while data science deals more with predictive analytics. (<span>more</span>) 

### Statistics vs Mathematics

Consider the following equations

- $Y = X + 0.2 \times X$

Say, $X$ = Basic Salary of an employee in a company, while $Y$ is computed from $X$, with adding to $X$ 20% of $X$. In this scenario, given the values of $X$, we can always tell what the gross salary would be. 

What if we have an equation such as the following:

$Y = X + 0.1 \times R$

Where, $R$ is the revenue the company earns through the employee. In this case, the salary of the employee would vary in each month. 

The salaries from month to month would unpredictably vary, which is where statistics comes in. Statistics deals with randomness, situations where we cannot exactly tell which outcome we might get. We may (or may not) know the possible outcomes (like when tossing a coin, we know the possible outcome, but which will happen)

### Why R? 

R is the most popular programming language for statistical analysis, second most popular for machine learning. 

Reasons at a glance

- Free and Open Source Software (FOSS)
- Big Community
- Made by statisticians for statisticians
- Easy to use codes
- Stunning graphics, esp. with *ggplot2*
- Reproducibility


### Who Use R? 

R is both used in academia and industry. 

- Good analyses for theses are now accomplished using R.
- Industries heavily rely on R for statistical analysis, predictive analytics, and machine learning. 

Some of the renowned companies using R are:

- Google
- Facebook
- Twitter (Tweet sensitivity analysis)


### Who Developed R? 

R was developed by Ross Ihaka and Robert Genetleman (<span>MORE</span>)

### Other Languages and Packages

Some other languages for data analysis are:

- Python
- Julia
- Java
- Scala

**Packages**

- SPSS
- STATA
- Eviews


### Installing R and Rstudio

- [x] [Go to Cran](https://cran.r-project.org) [^1]


### Start Writing R Code (Windows, Linux, and Command Line)

- Using R Console directly: Not a good idea
- Using Rstudio Console: Equivalent to using R console
- Using R Script from Rstudio: to run, press `Ctrl + Enter`

**It is best to use Rstudio.**

### Effectively Using Rstudio

- **Keep things organized**
- **Make a project** Put all codes, data and output inside that project directory. 
- **Use `View` function** to view data tables. 

### R Script

An R script is a convenient tool to organize a work. A project may consist of several or many such scripts. They can be easily shared with others. 

#### Quoting R codes from another R file. 

`source('r_file.R')`

### R Documentation (Help)

To get help, type `?keyword` or `help(keyword)`

For example, `?mean` would show options and examples for the mean function. 

### Handling Error

- If the code is not run, and shows a `+` sign, it means the code is not complete yet complete it or press `esc` to start over. 
- If the erros message shows `could not find function ...`, correct the function name. 
- If you do not understand the error message, copy and paste it to your browser search bar, and see what help the community has to offer. 

### R Packages 

R packages are extensions of base R, providing some very useful tasks. Many R packages made R more popular and useful, such as `ggplot2`, `karet`, and `rmarkdown`. 

To install a packages, run `install.pckages("package_name")`, for example `install.pckages("tidyverse")` installs the package `tidyverse`. When installing, the package name must be enclosed within quotation marks (" "). 

Before being able to make use of a package, one must load the package, by running `library(package_name)`, for example, to load `ggplot2`, run `library(ggplot2)`, this time without quotation marks (" ").


### R Mathematical Operations

- [ ] Make a table: Purpose, code, example, output

### Assigning Values

Variables make it easy to assign values and use them later. 

- To assign values to variables, you can use either `=` or `<-`, but in R, `<-` is preferred. In Rstudio, pressing `alt + -` is a very good shortcut for correctly typing `<-`. 
- Comments start with `hash` (#)

**Example**


```r
x <-  3
y <-  4
x+y
```

```
## [1] 7
```

```r
x*y
```

```
## [1] 12
```

```r
x+10-y
```

```
## [1] 9
```

```r
x^y
```

```
## [1] 81
```

```r
x**y
```

```
## [1] 81
```

```r
log(x)
```

```
## [1] 1.098612
```

```r
round(log(x), 3)
```

```
## [1] 1.099
```

#### Round, Floor, and Ceiling

Suppose, we have a number 3.9856

- `round` rounds the number; 


```r
x <- 3.9856
round(x,3) # (up to 3 digits)
```

```
## [1] 3.986
```
- `celing` switches the number to the next integer; 


```r
ceiling(x)
```

```
## [1] 4
```

`floor` gives the previous integer. 


```r
floor(x)
```

```
## [1] 3
```

- [x] `celing` and `floor` always give integer output. 

### Generating Multiple Numbers


```r
x <- 1:10
x
```

```
##  [1]  1  2  3  4  5  6  7  8  9 10
```

```r
seq(1,20, 2) # Keeping fixed gap between the numbers
```

```
##  [1]  1  3  5  7  9 11 13 15 17 19
```

```r
seq(1,50, length.out = 5) # Generating specific amount of numbers.
```

```
## [1]  1.00 13.25 25.50 37.75 50.00
```


### Data Types

- Logical
- Numeric
  + integer
  + Double
- Character  

### Learn More

- [x] Stat Mania artciles and link to contents
- [x] Books
- [x] Coursera, Edx, and other MOOCs. 

## Segemnt 02

### Vector

A vector is set of similar items. In Linear Algebra, it is defined as a matrix with only one column or one row. It could contain numbers of different types, strings, or logical values. 

A vector makes it easy to simultaneously operate on multiple items.

- [x] We make a vector when we are dealing with only one variable. 
- [x] A vector can contain only one type of values, such ac numeric, logical etc. 

A vector in `R` is usually made using `c`, which stands for *concatenate*. A vector can also be made using `seq` command shown earlier, or by using a `colon` (`:`) sign, if the values are successive integers. 


```r
x <- c(4, 5, 7)
a <- 10:12
y <- c("red", "green", "blue", "black", "orange")
z <- c(TRUE, FALSE, TRUE, TRUE, FALSE)
```

#### Adding Vectors

- If a scalar (a single value) is added to a vector, it would be added to values. 
- If two (or  more) vectors with equal lengths are added together, corresponding values would be added; the same goes for almost any other mathematical operation (such as subtraction or division). 

- If, however, the lengths are unequal, the values of the smaller vector would be repeated from the beginning. 


```r
x + 3 # Adds 3 all values of x.
```

```
## [1]  7  8 10
```

```r
x + a # Corresponding values are added.
```

```
## [1] 14 16 19
```

```r
b <- 6:7
x + b # Values of b are repeated. 
```

```
## Warning in x + b: longer object length is not a multiple of shorter object
## length
```

```
## [1] 10 12 13
```

#### Indexing Vectors

- Using `[]`: 

  
  ```r
  x
  ```
  
  ```
  ## [1] 4 5 7
  ```
  
  ```r
  x[2] # Extracts the second value.
  ```
  
  ```
  ## [1] 5
  ```
  
  ```r
  x[2:3] # Extracts second through third values.
  ```
  
  ```
  ## [1] 5 7
  ```
  
  ```r
  x[c(1,3)] # Extracts the first and third values.
  ```
  
  ```
  ## [1] 4 7
  ```
  
  ```r
  x[-1] # Extracts all except the first value.
  ```
  
  ```
  ## [1] 5 7
  ```
  
  ```r
  x[-c(1,3)] # Extracts all except the first and third values.
  ```
  
  ```
  ## [1] 5
  ```
- Using `Logical`

  
  ```r
  x[c(TRUE, TRUE, FALSE)] # Extracts the first and second values.
  ```
  
  ```
  ## [1] 4 5
  ```
  
  ```r
  y
  ```
  
  ```
  ## [1] "red"    "green"  "blue"   "black"  "orange"
  ```
  
  ```r
  z
  ```
  
  ```
  ## [1]  TRUE FALSE  TRUE  TRUE FALSE
  ```
  
  ```r
  y[z] # Using variables already stored. Does not extract values corresponding to FALSE items. 
  ```
  
  ```
  ## [1] "red"   "blue"  "black"
  ```
  
#### Changing Value(s) of A Vector

#### Sorting 

### Matrix

A matrix a rectangular array of similar items. Although it has more than two rows and columns, it can only contain items of a single type. 

<span>Contents from Jafar Sir</span>

### Data Frame

A Data frame contains many variables; each variable can be different type. Distinct variables are placed in columns and values/observations are in rows. 

**Example**



Table: (\#tab:unnamed-chunk-11)A Subset from mtcars Data Set

|                  |  mpg| cyl|  disp|  hp| drat|    wt|
|:-----------------|----:|---:|-----:|---:|----:|-----:|
|Mazda RX4         | 21.0|   6| 160.0| 110| 3.90| 2.620|
|Mazda RX4 Wag     | 21.0|   6| 160.0| 110| 3.90| 2.875|
|Datsun 710        | 22.8|   4| 108.0|  93| 3.85| 2.320|
|Hornet 4 Drive    | 21.4|   6| 258.0| 110| 3.08| 3.215|
|Hornet Sportabout | 18.7|   8| 360.0| 175| 3.15| 3.440|
|Valiant           | 18.1|   6| 225.0| 105| 2.76| 3.460|
|Duster 360        | 14.3|   8| 360.0| 245| 3.21| 3.570|
|Merc 240D         | 24.4|   4| 146.7|  62| 3.69| 3.190|
|Merc 230          | 22.8|   4| 140.8|  95| 3.92| 3.150|
|Merc 280          | 19.2|   6| 167.6| 123| 3.92| 3.440|

#### Making A New Data Frame

`data.frame` command is used to produce a data frame. 

- [x] Length of each variable must be equal. 


```r
df <- data.frame(x=c(10, 12, 15),
                 y=c("Dhaka", "Cumilla", "Rajshahi"),
                 w=sample(100, 3),
                 v=20:22)
```

#### Indexing A Data Frame

- [x] Methods used for matrices apply. 


Table: (\#tab:df)An Example Data Frame

|  x|y        |  w|  v|
|--:|:--------|--:|--:|
| 10|Dhaka    | 47| 20|
| 12|Cumilla  | 90| 21|
| 15|Rajshahi |  4| 22|


```r
df[2,3] # Extracts value from the third column in the second row. 
```

```
## [1] 90
```

### List

A list can contain scalars, vectors, matrices, data frames, as well as other lists! 

### Functions 

A function is used to 

- avoid repetitive tasks and mistakes therefrom
- find values from a complicated formula

**A function to compute Harmonic Mean (HM)**

**Formula:** Reciprocal of Mean of $\frac{1}{x_i}$

Reciprocal of $\frac{\frac{1}{x_1}+\frac{1}{x_2}+...+\frac{1}{x_n}}{n}$

Thus, $HM = \frac{n}{\sum \frac{1}{x_i}} =\frac 1 {\text{Mean of 1/x}}$


```r
hm <- function(x) {
  1/sum(1/x)
}
```

We have, x = 4, 5, 7

Therefore, 


```r
hm(x)
```

```
## [1] 1.686747
```

Since this function is actually a one-liner, we can write it as


```r
hm <- function(x) 1/sum(1/x)
```

### Loops (Alternatives and Comparison with Other Languages)

In R, loops are rarely used. 

#### For loop example

A for loop to add numbers 1 through 10. 


```r
sum <- 0
for (i in 1:10){
  sum <- sum + i
}
sum
```

```
## [1] 55
```

Values to loop through can also be called from a variable. 


```r
x <- c(10, 12, 8, 19, 23, 25)
sum <- 0
for (i in x){
  sum <- sum + i
}
sum
```

```
## [1] 97
```

<span>Contents from Jafar Sir</span>

### Apply family (apply, lapply, sapply, etc.). 

