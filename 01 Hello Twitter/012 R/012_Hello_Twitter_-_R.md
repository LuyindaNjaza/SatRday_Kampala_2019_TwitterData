012 Hello Twitter - R
================

## 1\. Getting started

To get started, the first section will provide a first walthrough on how
to configure the API access details as well load the required packages.
If any comment are unclear, feel free to message me either on github
directly or twitter under
@[LuyindaNjaza](https://twitter.com/LuyindaNjaza).

### 1.1 Calling the relevant R packages

``` r
# creating a vector which includes all packages relevant for this script
packages_012_Hello_Twitter_R      <- c("tidyverse",  # as standard packages to call dplyr, ggplot2, ggthemes as one
                                       "ggthemes",   # personal preference; adds further optional themes to ggplot2
                                       "rtweet",     # packages used to access the twitter API
                                       "httpuv")    # 

# unlike installing/loading the packages seperately, the following lapply function from base R passes the fector to the install.packages and library function within two lines.
#lapply(packages_012_Hello_Twitter_R  , install.packages)                # install.packages()
lapply(packages_012_Hello_Twitter_R  , library, character.only = TRUE)   # library()
```

### 1.1 Configuring the personal twitter API access

To configure the personal twitter API the following chunk provides two
solution. While the first, the in script solution, is the most
comvenient one if you just want to take a first look on the twitter data
available, the second, the external solution, provides a neat solution
if you are working on a bigger project and are goinng to use your
twitter credentials in multiple notebooks.

``` r
# In script solution:

# External solution:
source("Twitter_credentials.R", echo = TRUE , prompt.echo = "", spaced = F)
```
