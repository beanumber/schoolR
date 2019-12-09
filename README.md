# schoolR

An R package that provides a simple and accessible approach for elementary through high school students and their educators to engage in R and solidify their understanding of mathematical concepts. 

## Installation
To install, run the following code: 
```
devtools::install_github(https://github.com/sunniraleigh/schoolR) 
```

## Getting Started
For a more detailed guide about what functions do and exmaples about how to use them, see the [vignette](./vignettes/schoolR.Rmd).

## Usage
This package should be used in a classroom setting as a supplemental material for math courses, or as part of an R group dedicated to teaching younger students.
It provides functions to help students develop a deeper understanding of how area is caclulated, and how to analyze trends in graphs.
This package also lets teachers produce practice problems, while specifying the operation, number of problems to generate, and magnitude of numbers involved. 
It will be used by teachers and students in collaboration. It will allow students to begin understanding more complex, big picture math concepts by using R without having to first learn all of the details of coding.
```
library(schoolR)
```

### Drawing squares with `square()`
```{r}

```

### Draw a circle with `circle()`
`circle` allows the user to input a desired radius length which returns the respective circle visualization along with calculations of its diameter, perimeter, and area.
```{r}
# input a single length
circle(3)

# input a vector
circle(2:5)

# input a pre-defined vector
r <- c(4,7,9)
circle(r)
```

![circle_output](https://docs.google.com/drawings/d/e/2PACX-1vRNkT32DDHY3xg3jpJMK5k_-KhrrnsbMx2K7XiYpMdcrl5OyfZE6wmUBujq1fw92TG_eHRbuFrqlBip/pub?w=4500&h=1500)

### Draw a polygon with `ngon()`
``` {r}

```

### Graphing with `graph_my_data()`
`graph_my_data` allows students and teachers to produce high-quality graphs of data that they obtain, or of data from `data.frame`s. It outputs basic simple linear regression diagnostics such as correlation coefficients, means, and medians, and interprets the r value. This allows for a deeper understanding of general trends in data for students who likely have very little statistical background.
```{r}
x <- c(1, 3, 4, 6, 2)
y <- c(2, 7, 7, 11, 4)
graph_my_data(x, y, "blue", "number of students called in sick", "total number of absences", "kids out of school on a certain day")
```
![Graphs Produced](https://docs.google.com/drawings/d/e/2PACX-1vR9_940HjbdQlwP7S1qPbF-aYOrqc2LxOAFMRF57H-eg5fLQ5C0QZN1QKP_FggSUUQlhLAB1wd9JuZ-/pub?w=1002&h=487)
![simple linear regression diagnostics](https://docs.google.com/drawings/d/e/2PACX-1vR22yeb1Qj6TKddNupsHWgjWIJHjXZtDPHQLPnfeMdDBNe8b_KbOy1WOAYRoThdiLhe_ckei4EGi6PF/pub?w=960&h=720)

### Producing Practice Problems with `generate_problems()`
`generate_problems` allows educators to produce sets of practice questions for students based on what they would like them to work on. Teachers can specify the upper and lower bounds of the numbers being chosen from to use in the equation, what operation to use, and how many problems to produce.
```
generate_problems("multiply", 5, 15, 10)
```
![Problems](https://docs.google.com/drawings/d/e/2PACX-1vSUtfCXNdIVqLs1F5DEMui6fEfAxgEuOVP3TtUfMrwLHpCrs1vYExoPrJRyk7FbSp1gYgl52vydKysg/pub?w=169&h=125)

## Authors
Natalia Iannucci, Isabel Gomez, Sunni Raleigh
