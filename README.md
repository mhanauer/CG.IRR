# CG.IRR
install.packages("irr")
library(irr)
data(diagnoses)
# IRR for for more than two raters and categorical data
kappam.fleiss(diagnoses)
# Citations:  
# Fleiss, J.L. (1971). Measuring nominal scale agreement among many raters. Psychological Bulletin, 76, 378-382.
# Fleiss, J.L., Levin, B., & Paik, M.C. (2003). Statistical Methods for Rates and Proportions, 3rdEdition. New York: John # Wiley & Sons.
# Similar as above just different way of calculating it
kappam.light(diagnoses)
# Light, R.J. (1971). Measures of response agreement for qualitative data: Some generalizationsand alternatives. Psychological Bulletin, 76, 365-377.
# Estimates the rater bias and is another way to estimate reliabliity
# Significant test means that there is systematic bias in the rating
rater.bias(diagnoses)
