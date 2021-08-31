# Bootstrap-confidence-intervals-and-confidence-distritbutions-application-on-X-men-data-using-ggdist

The details of the codeset and plots are included in the attached Adobe Acrobat reader (.pdf) file in this repository. 
You need to download the same to view the contents. There are referrals to other contents in BLUE colour also to follow.

Background

Back in June, Julia Silge analysed the uncanny X-men comic book series. If, perchance, you are not familiar with her work, check out her blog and Youtube screencasts – invaluable resources for when I want to learn about any new tidyverse packages!

In her analyses of X-men comic series data from #tidytuesday, she proceeded to generate bootstrap confidence intervals for parameters of a logistic regression model. This is a very convenient way to show the variability in model parameters, but there is another package around — ggdist — that allows estimating and visualising confidence distributions around parameter estimates, in addition to several other visualisations such as the eye plot from the inimitable David Spiegelhalter.
But what is a confidence distribution?

It is a distribution estimator, like the bootstrap, but is more general than it and subsumes it. It can be thought of as a (sample dependent) distribution for all levels of a parameter’s confidence intervals, at different levels of probability. As such, it can be used, then, to also calculate confidence/compatibility intervals1, statistical power, p-values, etc.

I incline towards frequentism for most analytical problems, and the classic interpretation of confidence/compatibility distribution could pose a problem because under the frequentist view, parameters are fixed (while under Bayesian view, parameters are not fixed). In other words, previously a confidence distribution was interpreted as a distribution of the parameter. The modern definition, as outlined in this paper from Min-ge Xie and Kesar Singh, imposes certain requirements on the confidence distribution (to ensure adherence to frequentist properties), finally interpreting the distribution as an estimator for the parameter. This also means that there can be different confidence distributions that may be good, bad, worse, or best fit for a parameter of interest.
