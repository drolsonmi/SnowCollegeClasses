#### Answer to Practice Problem 3
2. What is the probability that the sample mean temperature is between 158°F and 162°F?
    * The mean and standard deviation are:
        * $\mu_{\bar{x}}$ = $\mu$ = 160
        * $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{5}{\sqrt{41}} = \frac{5}{6.403} = 0.7809$
    * The probability is found by finding the area of the right tail of the sampling distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score of 158$\degree$ is $z = \frac{158 - 160}{0.7809} = \frac{-2}{0.7809} = -2.5612
            * The z-score of 162$\degree$ is $z = \frac{162 - 160}{0.7809} = \frac{2}{0.7809} = 2.5612
            * Look up area left of z = -2.5612
                * $P(z < -2.5612) = 0.00522$
            * Look up area left of z = 0.60
                * $P(z < 2.5612) = 0.99478$
            * Take the difference between the two
                * $P(-2.5612 < z < 2.5612) = P(z < 2.5612) - P(z < -2.5612) = 0.99478 - 0.00522 = 0.9896$
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(158,162,160,0.7809) if using the values from the problem
            * 2:normalcdf(-2.5612,2.5612,0,1) if using the z-score (gives the same answer)
        * __Probability = 0.9896 = 98.96\%__