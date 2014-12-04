Stata-into-latex-Assignment
===========================

Introduction to economic software
ssc install bcuse
bcuse card
reg lwage educ exper expersq black south smsa reg661-reg668 smsa66
reg educ exper expersq black south smsa reg661-reg668 smsa66 nearc4
ivreg lwage (educ=nearc4) exper expersq black south smsa reg661-reg668 smsa66
ivregress 2sls lwage (educ=nearc4 nearc2) exper expersq black south smsa reg661-reg668 smsa66
reg iq nearc4
ivreg nearc4 smsa66 reg661 reg662 reg669
