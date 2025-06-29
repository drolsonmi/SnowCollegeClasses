# 17.2 Statistics of Sampling Distributions

## Reading

## Lesson
In lesson 17.1, we saw that if we take a large enough samples to from a sampling distribution, we form a normal distribution.

Now, we need to talk about the exact shape of the normal distribution. Let's consider a new dataset. Am individual's intelligence is measured in America using the IQ test. The distribution has a population mean of 100 ($\mu = 100$) and a standard deviation of 15 ($\sigma = 15$).

Your company collects 10,000 sample averages of people's IQ scores. In the following figures, I show the sampling distributions indicated with the blue histogram and the normal distribution of the samples (red curve). I also show the normal distribution for the population (green curve). The figures show the distributions for sample sizes of 10, 25, 50, and 100.

![Sampling Distributions compared to normal distributions of the population](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/images/Fig17_2a_sampling_distributions.png?raw=true)

Notice how the mean for the population and the samples are the same. So, 
$$\mu_{\bar{x}} = \mu$$

However, the normal distributions become narrower (they have smaller standard deviations). Let's compare the standard deviations of the two normal distributions. 

When the sample size is n = 10, the standard deviation is $\sigma_{\bar{x}} = 4.748$. If we take the ratio of the standard deviations, 
$$\frac{\sigma}{\sigma_{\bar{x}}} = \frac{15}{4.748} = 3.159$$

At first this doesn't look very helpful. However, when we see that $\sqrt{10}=3.162$, then we have a possible connection! Let's see if this works for our other sample sizes.

| Sample Size ($n$) | $\sigma_{\bar{x}}$ | $\frac{\sigma}{\sigma_{\bar{x}}}$ | $\sqrt{n}$ |
| :---: | :---:|:---:|:---:|
| 10  | 4.748 |  3.159 | 3.162 |
| 25  | 3.012 |  4.980 | 5     |
| 50  | 2.117 |  7.085 | 7.071 |
| 100 | 1.494 | 10.040 | 10    |

The last two columns are the ones we want to look at. The second-to-last column is the ratio of standard deviations, and the last column is $\sqrt{n}$. And they are very close! If the number of samples increases, then the two values will get closer and closer.

So, it holds! We now have a relationship between the population and sampling standard deviations. 
$$\sqrt{n} = \frac{\sigma}{\sigma_{\bar{x}}} \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

At this point, we can use our normal distribution to calculate probabilities as we did in Lessons 15 and 16.

### Application
You administer a specialized Competency Exam. The exam takes an average of 45 minutes to complete with a standard deviation of 12 minutes.

You are asked to administer the exam in an area that you suspect will complete the exam in less than 42 minutes.
* What is the probability that one single student completes the exam in less than 42 minutes?

$$\mu = 45 \qquad \sigma = 12$$
![Normal Distribution of population](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/images/Fig17_2b_Example_PopulationNormal.png?raw=true)

$$z = \frac{42-45}{12} = \frac{-3}{12} = -0.25$$
$$P(t \le 42) = P(z \le -0.25) = 0.401 = \mathbf{40.1\%}$$

Now, instead of looking at just one student, you're going to sample 30 students. Because of this, we expect a higher probability the average is closer to the mean, and a lower probability of an extreme value.
* What is the probability that the average time for your sample of 50 students is less than 42 minutes?

$$\mu_{\bar{x}} = \mu = 45 \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{12}{\sqrt{30}} = \frac{12}{5.477} = 2.191$$

![Normal Distribution of sample](https://github.com/drolsonmi/SnowCollegeClasses/blob/main/math1040online/images/Fig17_2c_Example_SamplingNormal.png?raw=true)

$$z = \frac{42-45}{2.191} = \frac{-3}{2.191} = -1.369$$
$$P(t \le 42) = P(z \le -1.369) = 0.085 = \mathbf{8.5\%}$$

So, we see a much higher probability for a single individual, but a much lower probability for a group average.

## Practice
Below are three problems regarding sampling distributions. Work on these problems, then click on the link to get the answer.

### Practice Problem 1
The average commute time for workers in a large metropolitan area is 35 minutes with a standard deviation of 8 minutes. A researcher takes a random sample of 64 workers.
1. What is the probability that the commute time of a single passenger is less than 33.5 minutes?
2. What is the probability that the sample mean commute time is less than 33.5 minutes?

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

### Practice Problem 2
A factory produces light bulbs with a mean lifetime of 1,200 hours and a standard deviation of 100 hours. A quality control engineer selects a random sample of 36 bulbs.
1. What is the probability that the lifetime of a single bulb is greater than 1,225 hours?
2. What is the probability that the sample mean lifetime of the 36 bulbs is greater than 1,225 hours?


### Practice Problem 3
A coffee shop claims that the average temperature of its freshly brewed coffee is 160°F with a standard deviation of 5°F. A health inspector randomly samples 41 cups of coffee.
1. What is the probability that the temperature of a single cup is between 158°F and 162°F?
2. What is the probability that the sample mean temperature is between 158°F and 162°F?

#### Answer to Practice Problem 3
1. What is the probability that the temperature of a single cup is between 158°F and 162°F?
    * The probability is found by finding the area between the two values on a standardized normal distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score of 158$\degree$ is $z = \frac{158 - 160}{5} = \frac{-2}{5} = -0.40
            * The z-score of 162$\degree$ is $z = \frac{162 - 160}{5} = \frac{2}{5} = 0.40
            * Look up area left of z = -0.60
                * $P(z < -0.40) = 0.3446$
            * Look up area left of z = 0.60
                * $P(z < 0.40) = 0.6554$
            * Take the difference between the two
                * $P(-0.40 < z < 0.40) = P(z < 0.40) - P(z < -0.40) = 0.6554 - 0.3446 = 0.311$
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(158,162,160,5) if using the values from the problem
            * 2:normalcdf(0.3446,0.6554,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.311 = 31.1\%__

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

## Technology
Calculations here use normal distributions, so refer by to the Technology section in Lesson 15 lecture pages.