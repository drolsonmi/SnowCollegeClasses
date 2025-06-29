#### Answer to Practice Problem 1
2. What is the probability that the sample mean commute time is less than 33.5 minutes?
    * The mean and standard deviation are:
        * $\mu_{\bar{x}}$ = $\mu$ = 35
        * $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{8}{\sqrt{64}} = \frac{8}{8} = 1.0$
    * The probability is found by finding the area of the left tail of the sampling distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score is $z = \frac{33.5 - 35}{1.0} = \frac{-1.5}{1.0} = -1.5$
            * Look at the area left of z = -1.5
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(-9999,33.5,35,1) if using the values from the problem
            * 2:normalcdf(-9999,-1.5,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.067 = 6.7\%__