# R Programming Class
  
  
## Day One:

### Preliminaries:

##### Introductions
* Your area of expertise
* Your current job tasking
* Your amount of experience with programming and R 
* Expectations for the class
  
##### Course Materials
* Several online books will be referenced
  * Hands-On Programming with R: https://rstudio-education.github.io/hopr/
  * https://swcarpentry.github.io/r-novice-inflammation/
* Other materials are available at:
  * https://github.com/ExgnosisClasses/R-Programming
  * These will be added to during the class
  * The repo will be available for 30 days after the last session


##### Virtual Machines
* These will be assigned shortly
  * A Protech instruction sheet is in the repo for reference
* You will have the same virtual machine for every class
  * Any time you log on, you can just carry on from where you were previously as long as you saved your work
* Because the class is spread out:
  * The machines may or may not be available outside
of class hours – the physical resources may be needed for
other classes
  * However, the image you were using will be saved and restored
for each class

##### R Studio
* R has a intimidating learning curve
* R Studio is an R development environment that makes learning and using R a LOT more user friendly
* Everything we do in R Studio in class can also be done at the R command line prompt
  
##### Downloading R and R Studio
* Free to use
  * Current R release is "Lost Library Book"
  * Previous Version is "Bunny-Wunnies Freak Out"  (seriously)
  * Available at: https://cran.r-project.org/
* R Studio is available at: https://rstudio.com/
---


## Intro to R
* Open source collaborative project
* Supported by CRAN - the comprehensive R archive network
* Core R is written in C and Fortran for speed
  * Parts of R are written in R
* It's worth the time to look at the resources available at CRAN
* R is primarily for data analytics / python is ML and Matlab modeling

## R Sessions and R Environment
Main points for this session
* The R session
* Saving and Restoring R session
* Navigating around the file system
* Getting online help
* Creating and removing objects
* Understanding the concept of an object
* Atomic data types
* Arithmetic and relational operators
  
---
## Atomic Vectors
* Creating and building vectors
* Generating sequences
* Operations between vectors
* Missing values
* Implicit type conversions
* Basic functions on vectors

---

creating a vector of different types
experiment with NA
basic arithmetic operations
use some byyasic attributes


---
# Day Two:
* vectors and arrays
* Projects 
* Packages
* programming in R
* dataframes 
* lists

1. data - measurements - vectors
2. information - organize - data frames
3. knowledge - gain insights
4.  Wisdom - being able to apply knoweldge

arrays are the primitive 

-------
# Day Three;
### Recap:
#### vectors or arrays
* primitive data type is a vector
* all elements of a vector are of the same type
* a scalar (3.8) is a vector of length 1
* we create a vector from atomic values by using c(... which combines elements)
* R will try and guess at what the type of vector is
  * numeric(n) creates a numeric vector of type numeric
* we reference individual elements with [] notation
  * R allows us to put elements anywhere
* Functions operate on arrays
  * eg sum()
#### Lists
* Used to hold heterogenous data
* Usually represents some sort of entity
* We will look at working with lists later

#### Dataframes
* Think of it as table in a date base
* Each column is of the same type
* We can name the rows and columns
* We can access columns using df$colname or df[,colnum]]

**We wll return to more detailed work with data later**

---------------

# Functions
* There are build in functions that operate on arrays
* They return either another vector or a statistic 

#### Functional Programming
* A function doesn't change anything but produces something new
* Can think of a function as a transformation of one piece of data to another

-----

Code used in class
x <- numeric(5)

bob <- list("name"="bob","male"=TRUE,"age"=45, "child_ages"=c(12, 14, 18))
str(bob)
ellen <- list("name"="ellen","male"=FALSE,"age"=22, "child_ages"=NA)

###

name <- c("Jon", "Bill", "Maria")
age <- c(23, 41, 32)
df <- data.frame(name, age)
df2 <- data.frame(name = c("Jon", "Bill", "Maria"),
                 age = c(23, 41, 32)
)

colnames(df) <- c("FirstName", "Age")
rownames(df) <- c("Subject 1", "Subject 2", "Subject 3")
###
order(cyl)
sort(cyl)
rev(cyl)
sum(cyl), man, min
cos(cyl)
f <- function(x) (cos(x)*cos(x))+(sin(x)*sin(x))
f(cyl)
##
cyl[6]=NA
sum(x, na.rm=T)

"%a2b%" <- function(a,b) return(a+2*b)
x <- c(4:6)
y <- c(1:3)
x %a2b% y

====================

# Day Four

We start working putting together the material we have learned so far by walking through a simple project.

1. Understand the R community standard for reproducible research in terms of R markdown
2. Import data from a csv file
3. Do a preliminary analysis of the data
4. Clean and transform the data
5. Do some statical analysis
6. 
