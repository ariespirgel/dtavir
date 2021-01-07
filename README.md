# Data Transformation and Visualization in R Workshop

Thank you for enrolling in this workshop! In this workshop, you will learn how to transform and visualize data in R. Specifically, we will be focusing on the [tidyverse packages](https://www.tidyverse.org/) dplyr and ggplot2.

## About This Workshop

This is a live, synchronous workshop on using the tidyverse to transform and visualize data. It is appropriate for people who have never coded or used R before, as well as those who have have some experience in R but are interested in learning more about the tidyverse.

The workshop is meant to be participatory. Throughout the workshop, you will be asked to code along with me, as well as use what you just learned to write your own code. The goal is for it to be challenging, educational, and fun!

## Pre-Workshop Installation Instructions

Prior to the workshop, please set up your computer by doing the following:

  1. Install the latest version of R from here: https://www.r-project.org/
  2. Intall RStudio Desktop from here: https://rstudio.com/products/rstudio/download/#download
  3. Open RStudio and in the console paste the following code and press Enter: **install.packages(c("devtools", "knitr", "scales", "ggthemes", "rmarkdown", "tidyverse"))**
  4. Once the packages from Step 3 are done installing, the `>` symbol will appear in the console. When that happens, paste the following code in the console and press Enter: **devtools::install_github("ariespirgel/vized")**
  5. Go to https://github.com/ariespirgel/dtavir and under the **Code** pulldown select **Download Zip**. Unzip the folder and save it to your desktop.

To make sure that everything installed properly, paste the following code into the RStudio console and press Enter. If a scatterplot appears, you are all set!

```  
library(tidyverse)
library(vized)

ipeds_sat %>% 
  ggplot(aes(x = sat_ebrw, y = sat_math, color = percentile)) +
  geom_point(alpha = .2)
```

## Copyright

All of the materials for this workshop are copyrighted under the[Creative Commons BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). The materials for this workshop are heavily influenced by [R for Data Science](https://r4ds.had.co.nz/) and [Remastering the Tidyverse](https://github.com/rstudio-education/remaster-the-tidyverse).
