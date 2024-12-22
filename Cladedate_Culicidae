#1 Cladedate install

install.packages("devtools")
install.packages("remotes")
install.packages("sn")

library(devtools)
library(remotes)
library(sn)

remotes::install_github("evolucionario/CladeDate")
library(CladeDate)

#2 Cladedate running

set.seed(241222)

#Culex_cladedate_statistic
Culex_n_friends <- rbind(c(33.9,56.0),c(33.0,40.4),c(16.0,40.4),c(23.0,33.9),c(23.0,33.9),c(33.9,56.0))
CnF <- clade.date(ages = Culex_n_friends, KStest = TRUE, n = 10000, PDFfit = "lognormal")
summary.clade.date(CnF)
capture.output(summary.clade.date(CnF), file = "Culex_cladedate_summary.txt")


#Coq_cladedate_statistic
Coq <- rbind(c(33.9,40.4),c(23.0,33.9),c(33.9,40.4),c(23.0,28.4),c(23.0,28.4))
Cq <- clade.date(ages = Coq, KStest = TRUE, n = 10000, PDFfit = "lognormal")
