012 Hello Twitter - R
================

## 1\. Getting started

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

    ## [[1]]
    ##  [1] "forcats"   "stringr"   "dplyr"     "purrr"     "readr"    
    ##  [6] "tidyr"     "tibble"    "ggplot2"   "tidyverse" "stats"    
    ## [11] "graphics"  "grDevices" "utils"     "datasets"  "methods"  
    ## [16] "base"     
    ## 
    ## [[2]]
    ##  [1] "ggthemes"  "forcats"   "stringr"   "dplyr"     "purrr"    
    ##  [6] "readr"     "tidyr"     "tibble"    "ggplot2"   "tidyverse"
    ## [11] "stats"     "graphics"  "grDevices" "utils"     "datasets" 
    ## [16] "methods"   "base"     
    ## 
    ## [[3]]
    ##  [1] "rtweet"    "ggthemes"  "forcats"   "stringr"   "dplyr"    
    ##  [6] "purrr"     "readr"     "tidyr"     "tibble"    "ggplot2"  
    ## [11] "tidyverse" "stats"     "graphics"  "grDevices" "utils"    
    ## [16] "datasets"  "methods"   "base"     
    ## 
    ## [[4]]
    ##  [1] "httpuv"    "rtweet"    "ggthemes"  "forcats"   "stringr"  
    ##  [6] "dplyr"     "purrr"     "readr"     "tidyr"     "tibble"   
    ## [11] "ggplot2"   "tidyverse" "stats"     "graphics"  "grDevices"
    ## [16] "utils"     "datasets"  "methods"   "base"
