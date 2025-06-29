#### Answer to Practice Problem 1
1. What is the probability that the commute time of a single passenger is less than 33.5 minutes?
    * The probability is found by finding the area of the left tail of a standardized normal distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score is $z = \frac{33.5 - 35}{8} = \frac{-1.5}{8} = -0.1875
            * Look at the area left of z = -0.1875
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(-9999,33.5,35,8) if using the values from the problem
            * 2:normalcdf(-9999,-0.3125,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.425 = 42.5\%__