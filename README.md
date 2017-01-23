# CG.IRR
install.packages("irr")
library(irr)
data(diagnoses)
# IRR for for more than two raters and categorical data
kappam.fleiss(diagnoses)
# Similar as above just different way of calculating it
kappam.light(diagnoses)
# Estimates the rater bias and is another way to estimate reliabliity
# Significant test means that there is systematic bias in the rating
rater.bias(diagnoses)
