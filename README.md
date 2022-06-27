# Bootstrap-confidence-intervals-and-confidence-distritbutions-application-on-X-men-data-using-ggdist

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.

Background
===============

To generate bootstrap confidence intervals for parameters of a logistic regression model. This is a very convenient way to show the variability in model parameters, but there is another package around — ggdist — that allows estimating and visualising confidence distributions around parameter estimates, in addition to several other visualisations such as the eye plot 

Confidence Disgtribution is a distribution estimator, like the bootstrap, but is more general than it and subsumes it. It can be thought of as a (sample dependent) distribution for all levels of a parameter’s confidence intervals, at different levels of probability. As such, it can be used, then, to also calculate confidence/compatibility intervals1, statistical power, p-values, etc.

I incline towards frequentism for most analytical problems, and the classic interpretation of confidence/compatibility distribution could pose a problem because under the frequentist view, parameters are fixed (while under Bayesian view, parameters are not fixed). In other words, previously a confidence distribution was interpreted as a distribution of the parameter. The modern definition, imposes certain requirements on the confidence distribution (to ensure adherence to frequentist properties), finally interpreting the distribution as an estimator for the parameter. This also means that there can be different confidence distributions that may be good, bad, worse, or best fit for a parameter of interest.
