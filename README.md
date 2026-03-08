# econ0019
ECON0019 Empirical Project

QUESTION:
Many U.S. states have adopted “shall-issue” laws, requiring permits for concealed weapons to be issued to all qualified citizens without a felony or mental health history. While proponents argue these laws deter crime by arming potential victims, opponents suggest they may inadvertently increase violence through accidental or spontaneous use. In this exercise, you will be asked to examine the relationship between these concealed carry policies and violent crime statistics using a panel data set from I. Ayres and J. Donohue (2003) “Shooting Down the ‘More Guns Less Crime’ Hypothesis,” Stanford Law Review 55: 1193–1312. The data set records violent crime and gun access in the 50 U.S. states plus the District of Columbia 1977–1999. The data set comes in two formats: A Stata data file version, ECON0019 empirical project 2026.dta, and a Excel version, ECON0019 empirical project 2026.xlsx. The data files contain annual observations of the following variables of interest for the period 1977–1999 for the 50 U.S. states plus the District of Columbia:
• viorate - violent crime rate (incidents per 100,000 members of the population)
• robrate - robbery rate (incidents per 100,000)
• murrate - murder rate (incidents per 100,000)
• shallcarry = 1 if the state has a shall-carry law in effect in that year, = 0 otherwise
• incarrate - incarceration rate in the state in the previous year (sentenced prisoners per 100,000 residents; value for the previous year)
• popdens - population per square mile of land area, divided by 1000
• avginc - real per capita personal income in the state, in thousands of dollars
• popul - state population, in millions of people
• pctmale - percent of state population that is male, ages 10 to 29
• pctwhite - percent of state population that is white, ages 10 to 64
• pctblack - percent of state population that is black, ages 10 to 64
• state - ID number of states (Alabama = 1, Alaska = 2, etc.)
• year - Year (1977-1999)
Answer all the following questions using clustered standard errors unless told otherwise:
1. Carry out an initial examination of the relationship between shall-carry and violent crime: compute the summary statistics (i.e. mean, quantiles, standard deviation) for the variables shallcarry and (the natural) logarithm of violent crime, log (viorate), for each year of the sam- ple. Do you see any patterns in the (average) levels of violent crimes and shall-carry? Explain.
2. Run the following two regressions and report the estimated models with clustered standard errors:
(I) Regress log (viorate) on shallcarry
(II) Regress log (viorate) on shallcarry together with all demographic and economic controls, popdens, avginc, popul, pctmale, pctwhite and pctblack
(a) How do you interpret the estimated shallcarry coefficient in model (II), and is the magnitude practically meaningful?
(b) Compare the results of model (I) and (II). In particular, does the inclusion of control variables alter the magnitude of the estimated effect and the precision of the estimated ”deterrence” effect of the law?
(c) Also interpret the estimated effects of the control variables. Do their signs make sense? Explain.
3. It could be that the effect of adoption of a shall–carry law comes with a time lag. Estimate model (II) where you add the first lag of shallcarry as a regressor. What do you conclude?
4. Go back to the baseline version of model (II). What happens to the estimated model when you account for unobserved state characteristics using a fixed effects estimator? Which of the four estimated models, (I), (II) and the ones in Questions 3. and 4, provides the most reliable estimate of the law’s impact on violent crimes, and why?
5. Does the “shall-issue” effect hold up for the fixed effects model in Question 4. when you also control for year-specific shocks that affected all states simultaneously (time fixed effects)? Are the time dummies jointly significant? Do you find this version to be superior to the one in Question 4? Explain.
6. Consider the residuals from the regression you ran in Question 5. for the state of Alabama. Plot the sample autocorrelations of these residuals. Based on these estimates, do you conclude that clustered standard errors are needed in the regression?
7. Re-run the model in Question 4. but now with log (robrate) and log (murrate) as the dependent variable, respectively. Are the results consistent across different types of violent crime?
8. It is possible that the adoption of “shall-issue” laws is endogenous: a rise in violent crime might lead state legislatures to pass concealed carry laws to appease a frightened public. To address this, suppose you use the political composition of the state legislature (e.g., the percentage of seats held by the party traditionally more supportive of gun rights) as an instrument for the shallcarry variable. What does it mean for an instrument to be exogenous and relevant? Do you believe it is likely that the instrument is exogenous and relevant in this setting? Why/why not?
9. Next, we wish to better understand which factors influence a state’s decision to adopt a shall-issue law. To this end, estimate and report the average partial effect of log (viorate) on shallcarry using logit, probit, and the linear probability models, and interpret their magnitudes. Control for popdens, avginc, popul, pctmale, pctwhite and pctblack and the year dummies in all three models.
10. For how many observations does each of these three estimated models predict a conditional probability of shallcarry = 1 which is outside the [0, 1] interval?
11. Compute the sample mean of shallcarry. We say that each of the models makes a mistake if it predicts a probability of success above the sample mean while shallcarry = 0, or the other way around. (Note that we use the sample mean, rather than 0.5, as a threshold.) Report the number of mistakes each of the three models makes. Based on this, which of the three models is the preferred one?
