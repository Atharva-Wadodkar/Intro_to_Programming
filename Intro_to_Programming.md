Introduction to Programming
================
Atharva Wadodkar
2026-07-16

# This section introduces us to R by using it as a simple calculator

# Assigning Variables

``` r
Result <- 15 + 25.1 + 20.25

Second_Result <- 12 + 22.6 + 68
```

# New Functions

``` r
years_old <- 25.7
```

# Rounds up

``` r
round(years_old)
```

    ## [1] 26

# Rounds down

``` r
floor(years_old) 
```

    ## [1] 25

``` r
years_old <- 25.765
```

# Comma after the object to specify argument

``` r
round (years_old, 2)
```

    ## [1] 25.76

``` r
Bill_age <- "Bill is 25.7 years old"

Bill_age <- paste('Bill is', years_old)
```

# Misconceptions

# Variables in programs do not work the same way as they do in spreadsheets

``` r
grade <- 55
total <- grade + 10
print (total)
```

    ## [1] 65

``` r
grade <- 90
print (total) # value of total in a spreadsheet will be 100, but in programming a variable holds the value it was assigned (65)
```

    ## [1] 65

``` r
total <- grade + 10
print (total) # executed in the way it was defined
```

    ## [1] 100

# What will this code do?

``` r
p <- 2
z <- 5
out <- p * z  # What should the value of out be?
print (out) # What is the value of out? Is it the same as expected?
```

    ## [1] 10

``` r
my_quiz <- c("uno",
             "dos",
             "tres",
             "cuatro", #"," was missing after cuatros
             "cinco")
print (my_quiz) #quiz was spelled wrong
```

    ## [1] "uno"    "dos"    "tres"   "cuatro" "cinco"

``` r
str(my_quiz)
```

    ##  chr [1:5] "uno" "dos" "tres" "cuatro" "cinco"

``` r
length(my_quiz) #len function does not exist; write full length to get function
```

    ## [1] 5

``` r
my_numeric_variable = 4.2
class(my_numeric_variable)
```

    ## [1] "numeric"

``` r
typeof(my_numeric_variable)
```

    ## [1] "double"

``` r
length(my_numeric_variable)
```

    ## [1] 1

``` r
attributes(my_numeric_variable)
```

    ## NULL

``` r
list("uno", "dos",'...')
```

    ## [[1]]
    ## [1] "uno"
    ## 
    ## [[2]]
    ## [1] "dos"
    ## 
    ## [[3]]
    ## [1] "..."

``` r
y <- c(1, 2, 3)
z <- c("Sarah", "Tracy", "Jon")
class(z)
```

    ## [1] "character"

``` r
class(y)
```

    ## [1] "numeric"

``` r
x <- list(1, "a", TRUE)
x
```

    ## [[1]]
    ## [1] 1
    ## 
    ## [[2]]
    ## [1] "a"
    ## 
    ## [[3]]
    ## [1] TRUE

``` r
x[[2]]
```

    ## [1] "a"

``` r
my_dataframe <- data.frame (no = c(1,2,3), c("Tracey", "John", "Pete"), c(TRUE, FALSE, TRUE))
my_dataframe
```

    ##   no c..Tracey....John....Pete.. c.TRUE..FALSE..TRUE.
    ## 1  1                      Tracey                 TRUE
    ## 2  2                        John                FALSE
    ## 3  3                        Pete                 TRUE

``` r
str (my_dataframe)
```

    ## 'data.frame':    3 obs. of  3 variables:
    ##  $ no                         : num  1 2 3
    ##  $ c..Tracey....John....Pete..: chr  "Tracey" "John" "Pete"
    ##  $ c.TRUE..FALSE..TRUE.       : logi  TRUE FALSE TRUE
