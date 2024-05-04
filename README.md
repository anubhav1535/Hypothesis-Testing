# Description about the data -

1. student_id – the unique identifier for each student in the dataset. The field contains IDs for students who used the 365 Data Science platform with free or paid accounts in Q4 2021 (October 1, 2021 – December 31, 2021, both included) and Q4 2022 (October 1, 2022 – December 31, 2022, both included).

2. student_country – identifies the country of each student. The field provides information about students’ geographic location and can help analyze regional differences or conduct country-specific analyses.

3. Paid – indicates whether a student had a paid account during the specified period. It is a binary variable, where '1' represents a paid account and '0' represents a free or unpaid account. It helps differentiate between students who have access to additional features or content through a paid subscription.

4. minutes_watched_21 – represents the student’s engagement level, as expressed by the number of minutes a student has watched in Q4 2021.

5. minutes_watched_22 – denotes the student’s engagement level, as expressed by the number of minutes a student has watched in Q4 2022.


# Task -1 
## Paid Plan students
 1. Mean: Among students who watched between 1 and 100 minutes in 2021, the average minutes watched by paid-plan students increased significantly from Q4 2021 to Q4 2022, from approximately 33.80 minutes to about 273.02 minutes. This suggests a substantial increase in engagement among this group of initially low-engagement-paid-plan students.
    
2. Median: The median minutes these low-engagement-paid-plan students watched increased from Q4 2021 to Q4 2022, from 26.33 minutes to 40.28 minutes. While this increase is not as dramatic as the increase in the mean, it indicates that the typical student in this group (i.e., the student in the middle of the distribution) also increased their engagement. This suggests that the increase in engagement was more widespread among paid-plan students and not solely driven by a few outliers.
   
3. Standard Deviation: The standard deviation for these low-engagement-paid-plan students increased substantially from 28.21 minutes in Q4 2021 to 854.58 minutes in Q4 2022. This indicates a much larger variability in the minutes watched by these students in Q4 2022 compared to Q4 2021. This could be due to a broader range of engagement levels among the students in Q4 2022, with some students watching very little content and others watching a lot of content.
   ![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/1bc3eedd-2879-4d67-a9aa-e1ded0e5466b)


### These results suggest a complex picture for the initially low-engagement-free-plan students. While the mean minutes watched increased—signifying an increase in overall engagement—the median minutes watched decreased, indicating that the typical student in this group did not increase their engagement. This discrepancy and the increased standard deviation suggest that a small number of students within this group might significantly increase their engagement while the majority did not. This might imply the need for targeted strategies to boost engagement among the broader population of initially low-engagement-free-plan students.

## Free plan students
1. Mean: Among students who watched between 1 and 100 minutes in 2021, the average minutes watched by free-plan students increased from about 25.39 minutes in Q4 2021 to about 117.64 minutes in Q4 2022. This suggests that overall engagement among these initially low-engagement-free-plan students increased during this period. But the extent of this increase is less than what was observed for similar low-engagement-paid-plan students, suggesting that while these free-plan students are watching more content, they're still not as engaged as the equivalent group of paid-plan students.
   
2. Median: Interestingly, the median minutes watched by these low-engagement-free-plan students decreased from Q4 2021 to Q4 2022, from 14.17 minutes to 11.83 minutes. This indicates that engagement decreased for the typical student in this group (i.e., the student in the middle of the distribution). The increase in the mean might be driven by a small number of free-plan students who significantly increased their engagement in Q4 2022, while the majority did not increase their engagement or even reduced it.
   
    Standard Deviation: The standard deviation for the low-engagement-free-plan students increased from 26.23 minutes in Q4 2021 to 468.93 minutes in Q4 2022. This indicates a more significant variability in the minutes watched by these students in Q4 2022 compared to Q4 2021. The behavior of these students then became more diverse in Q4 2022, with some watching a lot of content and others watching very little.

![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/5fc142e2-9366-405a-a46c-8478370946fc)


## On average, low-engagement-paid students initially increased their watching time more significantly than the free-plan students from Q4 2021 to Q4 2022. This could suggest that paid-plan students find more value in the platform, possibly due to premium features or content that are available to them.In contrast, the median watch time decreased for free-plan students, suggesting that the typical free-plan student in this group did not increase their engagement. This discrepancy might indicate that the strategies or features designed to increase engagement are more effective for paid-plan students. It could also suggest that the monetary investment leads to increased usage due to a desire to get their money's worth.


# Task-2
## Checking skewness

Skewness is a fundamental measure of probability distribution asymmetry in a dataset. It reveals whether the observations are concentrated more on one side of the distribution. This metric helps us understand how the data deviates from a normal distribution and provides insights into its underlying structure. A positive skewness value (higher than 0) indicates a right-skewed distribution, while a negative skewness value (lower than 0) points to a left-skewed distribution. A symmetrical distribution has a skewness value of 0, indicating a balanced data spread around the mean.

![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/6f6c6660-04cf-4b6a-89f8-e19a1b8b50ec)

![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/21312e6f-a816-4945-8ba6-5b5e63f36232)

## Positive skew (right-skew) occurs when the data is not symmetrical around the mean, forming a long tail on its right side. This signifies that most of the distribution's observations are concentrated to the left of the peak. Positive skewness can have several implications.

## The mean is larger than the median in a right-skewed distribution because the distribution tail pulls the mean to the right. This observation is confirmed by the mean and median values in the two years. An increasing skewness suggests that more students watch significantly more content than most over time, pulling the mean upwards.

## In both cases, the mean is higher than the median (33.80 > 26.33 in 2021 and 273.02 > 40.28 in 2022).


# Task-3 
## Confidence Intervals

![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/450e9bec-7f26-4fc3-ad03-3129328122ed)
For paid-plan students, there's an increase in engagement from Q4 2021 to Q4 2022. The confidence interval for the average minutes watched by paid-plan students increased from Q4 2021 (316.25 to 348.76 minutes) to Q4 2022 (351.91 to 384.72 minutes). This suggests that we can be 95% confident that the true average minutes watched by all paid-plan students in the population increased from Q4 2021 to Q4 2022.

![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/1c0055a4-2404-4b0e-a131-64c20faafeda)
Among free-plan students, there's a decrease in engagement from Q4 2021 to Q4 2022. The confidence interval for the average minutes watched decreased from Q4 2021 (129.92 to 137.95 minutes) to Q4 2022 (67.71 to 70.59 minutes). We then can be 95% confident that the true average minutes watched by all free-plan students in the population decreased from Q4 2021 to Q4 2022.

## Students with a paid-plan subscription watch substantially more than those without. The confidence interval for the average minutes watched in Q4 2022 was 61.71 to 70.59 minutes for free-plan students and 351.99 to 384.72 minutes for paid-plan students. We then can be 95% confident that paid-plan students watched significantly more minutes than free-plan students in Q4 2022. This aligns with the expectation that paid-plan students who have invested in the platform tend to be more engaged than free-plan users. 


# Task-4
## Hypothesis Testing
First, you must perform a two-sample f-test for variances to prove that assumption of unequal variances between the samples for free- and paid-plan subscribers:
![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/fddfc6e6-560e-4dc6-a0ea-f5183f40d1a7)
The p-value indicates the probability of obtaining the observed f-value if the null hypothesis (equal variances) were true. The sample variances are not identical since the p-value in both cases is 0.

Next, we use a left-tailed t-test assuming unequal variances for paying and free-plan students. 

## For paid plan students
![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/7215cfeb-b1b7-490e-9e26-f4c6423d4fd2)
Compare the t-statistic to the critical t-value:
![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/beb56b4e-e57f-449f-85ef-e1834a169573)

Conclusion: Reject  because the calculated t-statistic is lower than the critical value.

## Summary: With a t-statistic of -3.05 (less than the critical value of -1.645), you would reject the null hypothesis because the negative t-statistic indicates that  (the mean minutes watched by students in Q4 2021) is significantly smaller than  (the mean minutes watched by students in Q4 2022). This is contrary to the null, so we reject it. Of course, rejecting the null hypothesis does not confirm the alternative hypothesis; it suggests that the data provide enough evidence against the null hypothesis.


## For free plan students 
![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/8178ff38-b4ca-4e80-b692-ee7ed18f1222)
Compare the t-statistic to the critical t-value:
![image](https://github.com/anubhav1535/Hypothesis-Testing/assets/64795358/a581c54a-d245-423c-8897-42e25567edae)
Conclusion: Fail to Reject  because the calculated t-statistic is higher than the critical value.

## This could have the following implications.

## Market Differences: These details might indicate that the platform is more engaging or relevant to students in India than e US students. Understanding the reasons behind this could be valuable. Are the platform’s specific features, content, or aspects particularly appealing to Indian students? Such questions need to be addressed further but are beyond the scope of this analysis.

## Growth Opportunities: If US engagement is lower, this could represent a growth opportunity. The 365 company might seek ways to increase engagement among US students, involving marketing efforts, adding more content relevant to US students, or other strategies.

## Resource Allocation: This information could be helpful when deciding where to allocate resources. For example, if Indian students are more engaged, investing in more content and features targeted toward this audience might make sense.











   
