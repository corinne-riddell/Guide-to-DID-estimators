# Guide-to-DID-estimators
### [Corinne A Riddell](https://publichealth.berkeley.edu/people/corinne-riddell/), [Dana Goin](https://profiles.ucsf.edu/dana.goin)

# Overview

This guide illustrates scenarios in which difference in differences (DID) analysis can be applied. We assume readers know what a DID design is, have some background knowledge in policy analysis, and have working knowledge of R and RStudio.

We start with the simplest of DID scenarios and slowly amp up the complexity. For each scenario we describe a target parameter to estimate and the parameter estimated by a two-way fixed effects (TWFE) model. We apply the Goodman-Bacon decomposition to this parameter to determine if the TWFE estimate is influenced by estimates that are “forbidden” (e.g., ones that compare a newly treated state to a previously treated state). The goal is to illustrate when the usual TWFE method of estimation provides suitable results and when the TWFE approach is biased and/or aggregates the individual ATTs in an unintuitive way. In the latter case, we show alternative methods to estimation to overcome these issues.

# How to use this guide

If you are interested in reading this resource online, you can find it [here](https://rpubs.com/corinne-riddell/927985).

If you would rather run the R code locally, you can download everything you need from this GitHub repository. Use this code in the R console:

install.packages("usethis") #run this line if you need to install the usethis package
usethis::use_course("corinne-riddell/Guide-to-DID-estimators")
