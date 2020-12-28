monomass
================
predict diagnostic product ions for Hb variants
## Installation

Install from GitHub:

``` 

```


## Steps to get the results
### package
library(dplyr)
library(tidyr)

### Input the sequennces-monomass
recz <- monomz("VHLTPEEKSAVT", fragments = "cz")
reby <- monomz("VHLTPEEKSAVT", fragments = "by")
### Input the sequennces-monomass2
results.cz <- monomz2("VHLTPEEKSAVT", fragments = "cz")
results.by <- monomz2("VHLTPEEKSAVT", fragments = "by")

### output results in .csv
write.csv(reby,"monomz.csv", row.names = FALSE)
write.csv(results.by,"monomz2.csv", row.names = FALSE)
