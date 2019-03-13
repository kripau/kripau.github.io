---
layout: post
title: Descriptive Statistics
date: 2019-02-17
Tags: STAT
---
Statistics is a branch of mathematics that includes collection, organization, and interpretation of data. After collecting the data, it is the utmost priority to read and understand the data by using statistical technique before using an algorithm and making predictions.

Descriptive statistics and inferential statistic are two types of statistics. Descriptive statistics refers to the analysis of data that helps in organizing, showing and summarizing data in a clear and concise way, leading to some emerging pattern from the data. Inferential statistics, on the other hand, develops on the basis of probability theory and hypothesis. This blog focusses only on descriptive statistics

Descriptive statistic can be further divided into following:

1. Measures of central tendency
2. Measure of variability
3. Measure of relationship between variables

### 1. Measures of central tendency
A measure of central tendency is a summary measure that represents a whole set of data with a unique value or a point that represents the center or middle of its distribution. There are three measures of central tendency:  mean, median and mode. Each of these examples describes the central value in the distribution.

### Mean :
It is the average of all the numbers in a dataset. It is sum of all the numbers in a dataset divided by numbers of data in a dataset.


<img src="/assets/img/des_stat/1_mean.png" alt="mean" style="width:500px; margin-left: automargin-right: auto;"/>


Where X is the value of each data and n is the total number of data.

 Example: Salary of 5 employees includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. Mean salary is 7.5K

**Advantage of the mean:**  
1. The mean can be employed for both discrete and continuous numerical data.

**Limitations of the mean:**
1. The mean cannot be used for categorical data
2. The mean is highly influenced by outliers and skewed distributions.

### Median:
It is a middle value in an ordered dataset.

<img src="/assets/img/des_stat/2_median.png" alt="mean" style="width:600px; margin-left: automargin-right: auto;"/>

Example: Salary of 5 employee includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. To find the median, arrange the data in ascending order which is 6.6K, 7K, 7.5K, 7.5K, 8.9K. Median salary is (5+1)/2=3rd item in the list which is 7.5K. 

**Advantage of median:**
1. The median is less influenced by outliers and skewed data compared to that of the mean due to which it is normally the chosen measure of central tendency when the distribution is asymmetrical. 

**Limitation of the median:**
1. The median cannot be used for categorical nominal data as it cannot be ordered.

### Mode: 
It is the value of a dataset having the highest frequency. If there are no items having frequency greater than 1 then there is no mode. If there are several items having frequency greater than one, there is more than one mode, also known as bimodal or multimodal.

Example: Salary of 5 employee includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. Mode salary is 7.5K

### Influence of outliers in the measures of central tendency?

Outliers are an extreme value that is distinctly unusual from the rest of the data in a dataset.
It is essential to identify outliers present in a distribution as it can change the results of the data analysis significantly. The mean is more sensitive to the presence of outliers than the median or mode.

If the outlier is confirmed as a valid extreme value, it should not be removed from the dataset and vice versa

### 2.	Measure of variability
A measure of variability is a summary measure that represents how data is spread out or scattered. Variance, standard deviation and coefficient of variation are three measure of variability.

### Variance:
Variance measures the dispersion of a set of data points around their mean. Variance is squaring the difference between an individual data point and the mean and averaging the squares. Variance measures the average degree to which each data deviates from the mean. The higher the variance, the greater the entire data range. It’s unit is squared of the unit of dataset and it’s mean.

<img src="/assets/img/des_stat/3_Variance.png" alt="mean" style="width:600px; margin-left: automargin-right: auto;"/>

Example: Salary of 5 employee includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. Mean salary is 7.5K. Variance of the dataset is 0.755K.

### Standard deviation:
Standard deviation is simply the square root of the variance. The squared root of the variance indicates the standard deviation which returned to the original unit of measurement of the dataset making standard deviation much more meaningful than variance.

<img src="/assets/img/des_stat/4_Standard_deviation.png" alt="mean" style="width:600px; margin-left: automargin-right: auto;"/>

Example: Salary of 5 employee includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. Mean salary is 7.5K. Variance of the dataset is 0.8689K 

### Coefficient of variation :
Coefficient of variation is the relative standard deviation with respect to its mean value.

<img src="/assets/img/des_stat/5_cv.png" alt="mean" style="width:600px; margin-left: automargin-right: auto;"/>

For a single dataset, standard deviation is the most common measure of variability. However, when two or more dataset is compared, comparing standard deviation is meaningless while comparing coefficient of variation of two or more dataset is very meaningful.

Example: Salary of 5 employee includes 7K, 6.6K, 7.5K, 8.9K, 7.5K. Mean salary is 7.5K. Standard deviation of the dataset is 0.8689K. Coefficient of variation is 0.8689K / 7.5K = 0.115

### 3.	Measure of relationship between variables
Covariance and correlation are two measure of relationship between variables.

### Covariance :
Covariance is a measure indicating the degree to which two random variables changes. It can be found using the following formula. It’s value ranges from -∞ to +∞. 

<img src="/assets/img/des_stat/6_Covariance.png" alt="mean" style="width:600px; margin-left: automargin-right: auto;"/>

The two variables are correlated and the main statistics to measure correlation is covariance. Covariance gives sense of direction. If covariance is greater than zero, the two variables move together. If it is lesser than zero, the two variables move in opposite directions. If it is equal to zero, the two variables are independent. Its unit is the product of units of two variables.

### Correlation:
Correlation can be defined as a measure of the linear relationship between two quantitative variables. Correlation adjusts covariance so that the relationship between two variables becomes easy and intuitive to interpret. Correlation coefficient value ranges from -1 to +1.

There is a positive correlation when the values of one variable increase as the values of the other increase. A negative correlation is when the values of one variable decrease as the values of another increase showing an inverse relationship. A correlation of 1 means a perfect positive correlation. A correlation of -1 means a perfect negative correlation. A correlation of 0 means that there is no relationship between the different variables. Values between -1 and 1 indicate the strength of the correlation. Some of the example of correlation includes:

Positive correlation

1.	The less time I spend marketing my business, the fewer new customers I will have.
2.	The longer someone invests, the more compound interest he will earn.
3.	As you drink more coffee, the number of hours you stay awake increases.
4.	As her salary increased, so did her spending.
5.	When workers get a raise, morale improves.

Negative correlation

1.	If a train increases speed, the length of time to get to the final point decreases.
2.	As one exercises more, his body weight becomes less.
3.	The more one works, the less free time one has.
4.	As the temperature increases, fewer hot chocolate products are sold. 
5.	As more employees are laid off, satisfaction among remaining employees decreases. 
6.	As the temperature decreases, more heaters are purchased.
7.	The more one eats, the less hunger one will have. 
8.	As humidity increases, people's desire to be outside may decrease.
9.	If the temperatures outside decrease dramatically, heating bills will increase.
10.	The more alcohol one consumes, the less judgment one has.

Common problems in correlation
1.	Correlation may not be reliable when the sample size is small.
2.	If the outliers are present in the dataset, the correlation coefficient is misleading.

