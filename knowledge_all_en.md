# 📘 Part 2 (Expanded Edition): Complete Knowledge Points for All Nine Units

---

# 📊 Unit 1: Exploring One-Variable Data (Exam Weight: 15-23%)

> **Big Ideas**: VAR (Variation and Distribution) + UNC (Patterns and Uncertainty)
> **Core Skills**: Skill 2 (Data Analysis) — describing data, constructing graphs, calculating statistics, comparing distributions

---

## Topic 1.1: Introduction to Statistics — What Can Data Tell Us?

### Detailed Explanation

Statistics is not a discipline about numbers, but about **numbers with context**. The same number "42" means completely different things in "a person's age is 42 years old" versus "the maximum score on an exam is 42 points." Numbers only carry information value when placed in **context**.

The core question introduced in the course is: Is **variation** random or meaningful? We encounter variation every day — each person's height is different, each cup of coffee has a different temperature, each exam score is different. Statistics provides a systematic set of methods to help us identify **true patterns** from seemingly chaotic data, distinguishing "signal" from "noise."

### Example

> **Question**: A high school principal wants to know the average sleep time of the school's 1,200 students. He surveys Class A (30 students) and Class B (30 students) and finds that the average sleep time for Class A is 7.2 hours and for Class B is 6.8 hours. Why are the averages different? Is this 0.4-hour difference "meaningful"?
>
> **Solution Approach**: Even though both classes come from the same school, because different students are sampled from each class, the sample means will naturally differ. This is **Sampling Variability**. To determine whether the 0.4-hour difference is "meaningful," we need to check whether it is too large to be explained by random fluctuation — this is precisely what subsequent statistical inference will address.

---

## Topic 1.2: The Language of Variables

### Detailed Explanation

The first step in statistics is **identifying the type of variable**. A variable is any characteristic that changes from individual to individual. The values of a categorical variable are just "labels" — even if they are encoded as numbers (e.g., 1=male, 2=female), doing arithmetic on these numbers is meaningless. The values of a quantitative variable are obtained through **measurement or counting** and can be used in arithmetic operations.

**Distinguishing between the two** is the foundation for choosing all subsequent analysis methods.

| Variable Type | Can You Calculate the Mean? | Examples | Common Analysis Methods |
|---------------|-----------------------------|----------|-------------------------|
| Categorical | ❌ No | Blood type, major, province | Bar graph, percentages, chi-square test |
| Quantitative | ✅ Yes | Height, temperature, income | Histogram, mean, standard deviation, t-test |

A common point of confusion is "age" — it is sometimes treated as quantitative (e.g., "25 years old") and sometimes as categorical (e.g., "young/middle-aged/elderly"). This depends on how you define and use it.

### Example

> **Question**: Among the following variables, which are categorical and which are quantitative?
> (a) A movie's rating (1 star to 5 stars)
> (b) A movie's duration (in minutes)
> (c) A movie's genre (comedy, drama, action, etc.)
> (d) A movie's box office revenue (in dollars)
>
> **Solution**:
> (a) **Categorical** — star ratings are category labels (even if written as numbers 1-5, they represent rating categories; the "difference" between 1 star and 2 stars has no practical meaning)
> (b) **Quantitative** — duration is a measured value
> (c) **Categorical** — genre is a category name
> (d) **Quantitative** — revenue is a counted value

---

## Topic 1.3-1.4: Representing Categorical Variables

### Detailed Explanation

A **Frequency Table** tells us how many individuals are in each category. A **Relative Frequency Table** tells us what **proportion** each category occupies — this allows us to compare groups of different sizes.

A **Bar Graph** is the most common graph for displaying categorical data. Bars have gaps between them, emphasizing that categories are discrete and independent. The height of the bars can represent **frequency** (absolute count) or **relative frequency** (proportion/percentage).

**Important Distinction**: Do not confuse bar graphs with histograms. Bar graphs are for **categorical** data (bars have gaps), while histograms are for **quantitative** data (bars have no gaps).

### Example

> **Question**: A university surveyed 200 students about their majors. Results: Science 80, Humanities 60, Engineering 40, Business 20.
> (a) Construct a relative frequency table.
> (b) Describe what the data reveals.
>
> **Solution**:
> (a) | Major | Relative Frequency |
>     |-------|--------------------|
>     | Science | 80/200 = 0.40 (40%) |
>     | Humanities | 60/200 = 0.30 (30%) |
>     | Engineering | 40/200 = 0.20 (20%) |
>     | Business | 20/200 = 0.10 (10%) |
>
> (b) The data reveals: Science majors are the most numerous at 40%; Humanities accounts for 30%; Engineering 20%; Business is the smallest at only 10%. Science and Humanities combined make up 70% of all students.

---

## Topic 1.5: Graphical Representations of Quantitative Variables

### Detailed Explanation

Four commonly used graphs each have their strengths and weaknesses:

| Graph | Strengths | Weaknesses |
|-------|-----------|------------|
| **Dotplot** | Retains the position of each data point; good for small datasets | Crowded and messy with lots of data |
| **Stem-and-Leaf Plot** | **Preserves all original data values**; displays sorted order | Not suitable for large datasets |
| **Histogram** | Good for large datasets; flexible bin width | **Choice of bin width affects appearance**; does not preserve raw data |
| **Cumulative Graph** | Directly shows percentiles | Hard to see distribution shape intuitively |

**Discrete vs. Continuous**: Discrete variables can only take countable values (e.g., "number of children in a family" can only be 0, 1, 2, 3…). Continuous variables can take infinitely many values (e.g., "height" could be 170.1 cm, 170.11 cm, 170.111 cm…).

### Example

> **Question**: Here are the math exam scores (out of 100) for 10 students: 72, 85, 91, 85, 67, 88, 85, 73, 94, 80. Display the data using a stem-and-leaf plot (stems = tens digit, leaves = units digit).
>
> **Solution**:
> ```
> 6 | 7
> 7 | 2 3
> 8 | 0 5 5 5 8
> 9 | 1 4
> ```
> Interpretation: From the stem-and-leaf plot, we can see that most students' scores are concentrated at 80 and above; 85 appears three times (the mode); the lowest score is 67 and the highest is 94.

---

## Topic 1.6: Describing the Distribution of a Quantitative Variable — The SOCS Framework

### Detailed Explanation

This is the complete framework that must be followed when describing any univariate quantitative distribution:

| Dimension | Question to Answer | Descriptive Terms |
|-----------|-------------------|-------------------|
| **S - Shape** | Is the distribution symmetric or skewed? How many peaks? | Symmetric, skewed right, skewed left, unimodal, bimodal, uniform |
| **O - Outliers** | Are there values that clearly deviate from the rest? | Yes (specify where) / No |
| **C - Center** | What is a "typical" value for the data? | Mean or median |
| **S - Spread** | How spread out are the data values? | Range, IQR, standard deviation |

**Relationship Between Skewness and Mean vs. Median**:

| Distribution Shape | Mean vs. Median | Reason |
|-------------------|-----------------|--------|
| Symmetric | Mean ≈ Median | Both sides symmetric; extreme values balance out |
| Skewed Right (Positively Skewed) | Mean > Median | Extreme values on the right pull the mean rightward |
| Skewed Left (Negatively Skewed) | Mean < Median | Extreme values on the left pull the mean leftward |

### Example

> **Question**: Here are the monthly salaries (in thousands of dollars) of 20 employees: 28, 30, 31, 32, 32, 33, 34, 35, 35, 36, 37, 38, 38, 39, 40, 42, 45, 48, 52, 85. Describe this distribution using SOCS.
>
> **Solution**:
> - **S (Shape)**: The distribution is **skewed right** (positively skewed), because the left side has relatively concentrated data while the right side has a long tail extending to 85.
> - **O (Outliers)**: 85 thousand is noticeably higher than the rest. Using the 1.5×IQR rule: Q1=32.5, Q3=40.5, IQR=8, upper bound=40.5+1.5×8=52.5. Since 85 > 52.5, 85 is an outlier.
> - **C (Center)**: Median = (36+37)/2 = 36.5 thousand. Since the distribution is skewed right, the median is the better measure of center (the mean would be pulled upward by 85).
> - **S (Spread)**: IQR = 40.5 - 32.5 = 8 thousand. Range = 85 - 28 = 57 thousand.

---

## Topic 1.7: Summary Statistics

### Detailed Explanation

**Measures of Center**:

The **mean** is the arithmetic average of all data values. The **median** is the middle value when sorted. **The mean is heavily affected by outliers** (non-resistant), while **the median is not affected by outliers** (resistant). Therefore: use the mean for symmetric distributions, and the median for skewed distributions.

**Measures of Spread**:

The **standard deviation** measures the **average distance** of each data point from the mean. Its formula structure is: s = √[Σ(xi - x̄)²/(n-1)]. Note:
- Dividing by (n-1) instead of n — this is because using (n-1) makes the sample variance an unbiased estimator of the population variance
- The standard deviation has the **same units** as the original data (e.g., "years"), while the variance has units of "squared years"

**Two Methods for Identifying Outliers**:
1. **1.5×IQR Rule**: Any value less than Q1 - 1.5×IQR or greater than Q3 + 1.5×IQR
2. **2 Standard Deviation Rule**: Any value more than 2 standard deviations from the mean

### Example

> **Question**: Dataset: 5, 7, 8, 9, 10, 12, 15. Calculate the mean, median, range, IQR, and standard deviation. Which measure of center is more appropriate for this dataset?
>
> **Solution**:
> - **Mean**: x̄ = (5+7+8+9+10+12+15)/7 = 66/7 ≈ 9.43
> - **Median**: Sorted: 5, 7, 8, 9, 10, 12, 15. The 4th value = **9**
> - **Range**: 15 - 5 = **10**
> - **Quartiles**: Q1 = 7 (median of the lower half), Q3 = 12 (median of the upper half)
> - **IQR**: 12 - 7 = **5**
> - **Standard Deviation**: s = √[((5-9.43)²+(7-9.43)²+...+(15-9.43)²)/6] ≈ **3.41**
> - **Choice**: The mean (9.43) and median (9) are close, indicating the distribution is relatively symmetric. Both are acceptable.

---

## Topic 1.8: Boxplots

### Detailed Explanation

**Five-Number Summary**:
> Minimum | Q1 | Median | Q3 | Maximum

**Structure of a Boxplot**:
- **Box**: From Q1 to Q3, representing the middle 50% of the data
- **Median Line**: The horizontal line inside the box, representing the median
- **Whiskers**: Extend from Q1 down to the **minimum non-outlier value**, and from Q3 up to the **maximum non-outlier value**
- **Outlier Symbols**: Values beyond the whiskers are marked with individual dots or asterisks

**Graphical Inference about Mean vs. Median**:
- In a boxplot, if the median line is at the center of the box and the whiskers are roughly equal in length → symmetric distribution
- Median line closer to the bottom of the box and the upper whisker is longer → skewed right
- Median line closer to the top of the box and the lower whisker is longer → skewed left

### Example

> **Question**: Draw a boxplot from the following five-number summary: Minimum=10, Q1=20, Median=35, Q3=45, Maximum=70. Determine the approximate shape of the distribution.
>
> **Solution**:
> Boxplot structure: The box extends from 20 to 45, with the median line at 35.
> Lower whisker extends from 20 down to 10 (length=10); upper whisker extends from 45 up to 70 (length=25).
> The upper whisker is much longer than the lower whisker, indicating a **skewed right** shape.
> Check for outliers: IQR=45-20=25. Upper bound=45+1.5×25=82.5. Since 70<82.5, the maximum of 70 is not an outlier.

---

## Topic 1.9: Comparing Distributions

### Detailed Explanation

When comparing two or more distributions, you must **compare each dimension of SOCS point by point**. Do not just say "they are different" — specify **exactly how** they differ.

Tools used for comparison:
- **Side-by-side boxplots**: Most common; directly compare the five key values
- **Side-by-side histograms**: More intuitive for comparing shape
- **Back-to-back stem-and-leaf plots**: Suitable for small datasets

### Example

> **Question**: The five-number summary for Group A (n=30) is: 55, 65, 72, 80, 95. The five-number summary for Group B (n=30) is: 40, 58, 70, 82, 100. Compare the two distributions.
>
> **Solution**:
> - **Center**: Group A's median (72) is slightly higher than Group B's (70), but the difference is small.
> - **Spread**: Group A's IQR (80-65=15) is smaller than Group B's IQR (82-58=24), indicating Group A's scores are more concentrated.
> - **Shape**: In Group A, the median (72) sits within Q1=65 and Q3=80, slightly closer to the bottom edge, suggesting mild right skew. In Group B, the median (70) is between 58 and 82, close to the center, relatively symmetric.
> - **Outliers**: Neither group has any flagged outliers.

---

## Topic 1.10: The Normal Distribution

### Detailed Explanation

The **normal distribution** is the **most important theoretical distribution** in statistics. It describes many natural phenomena: height, blood pressure, measurement error, etc.

**Characteristics of the Normal Curve**:
- Bell-shaped (mound-shaped), symmetric
- Mean = Median = Mode
- Completely determined by two parameters: **μ (mean)** and **σ (standard deviation)**

**Empirical Rule (68-95-99.7 Rule)**:
- Approximately **68%** of data falls within μ ± 1σ
- Approximately **95%** of data falls within μ ± 2σ
- Approximately **99.7%** of data falls within μ ± 3σ

**z-score**: z = (x - μ)/σ
- A z-score of 1.5 means the data value is 1.5 standard deviations above the mean
- A z-score of -0.8 means the data value is 0.8 standard deviations below the mean
- **z-scores have no units**, so they can be compared across different distributions

**Percentiles**: The p-th percentile is the value below which p% of the data falls. For example, if your exam score is at the 85th percentile, you scored higher than 85% of test-takers.

### Example

> **Question**: Exam scores follow a normal distribution with μ=70 and σ=8.
> (a) Approximately what percentage of students scored between 62 and 78?
> (b) A student scored 86. Calculate his z-score and interpret its meaning.
>
> **Solution**:
> (a) 62 = 70 - 8 = μ - 1σ, 78 = 70 + 8 = μ + 1σ.
>     According to the Empirical Rule, approximately **68%** of students scored between 62 and 78.
>
> (b) z = (86 - 70)/8 = 16/8 = **2.0**
>     This student's score is 2 standard deviations above the mean. According to the standard normal distribution, a z-score of 2.00 corresponds to approximately the 97.7th percentile, meaning this student scored higher than about 97.7% of test-takers.

---

# 📈 Unit 2: Exploring Two-Variable Data (Exam Weight: 5-7%)

> **Big Ideas**: VAR (Variation and Distribution) + UNC (Patterns and Uncertainty) + DAT (Data-Based Predictions, Decisions, and Conclusions)
> **Core Skills**: Skill 2 (Data Analysis) + Skill 4 (Statistical Argumentation)

---

## Topic 2.1: Are Variables Related?

### Detailed Explanation

When we move from one-variable data to two-variable data, the core question becomes: **Is there an association between two variables?** An association means that a change in one variable accompanies a change in the other. But note: **association is not causation** — this is the most important and most frequently misunderstood principle in statistics.

In Unit 2, we will:
- Analyze associations between two categorical variables → two-way tables
- Analyze associations between two quantitative variables → scatterplots and correlation

### Example

> **Question**: A researcher finds that in months when ice cream sales are high, drowning incidents are also more frequent. Can he conclude that "eating ice cream causes drowning"?
>
> **Solution**: No. This is likely due to a **confounding variable** — hot weather leads to both increased ice cream sales and more people swimming, which increases drowning risk. There is an **association** between ice cream sales and drowning, but **no causal relationship**.

---

## Topic 2.2-2.3: Two Categorical Variables

### Detailed Explanation

A **Two-Way Table (Contingency Table)** is the core tool for simultaneously displaying two categorical variables.

Three types of frequencies:

| Frequency Type | Calculation | Purpose |
|---------------|-------------|---------|
| **Joint Frequency** | Cell count ÷ total count | Proportion of a specific combination |
| **Marginal Frequency** | Row total ÷ total OR Column total ÷ total | Distribution of a single variable |
| **Conditional Frequency** | Cell count within a row ÷ row total OR within a column ÷ column total | Distribution of one variable given a specific value of the other |

**Key Question**: Are the two variables associated? The method is to compare conditional distributions. If the distribution of one variable differs across conditions of the other variable, then the two variables are associated.

### Example

> **Question**: The table below shows data on gender and liking math for 200 people:
>
> | | Likes Math | Dislikes Math | Total |
> |---------------|------------|---------------|-------|
> | Male | 60 | 40 | 100 |
> | Female | 35 | 65 | 100 |
> | Total | 95 | 105 | 200 |
>
> Is there an association between gender and liking math?
>
> **Solution**: Calculate conditional relative frequencies:
> - Proportion of males who like math: 60/100 = **60%**
> - Proportion of females who like math: 35/100 = **35%**
>
> The proportion for males (60%) is clearly higher than for females (35%), so gender and liking math **are associated**.

---

## Topic 2.4: Scatterplots

### Detailed Explanation

A **scatterplot** is the core graphical tool for displaying the relationship between two quantitative variables. Each point represents one individual, with its x-coordinate and y-coordinate representing that individual's values for the two variables.

| Concept | Definition |
|---------|------------|
| **Explanatory Variable** | The variable used to explain or predict; placed on the x-axis |
| **Response Variable** | The variable being explained or predicted; placed on the y-axis |

**Four Dimensions for Describing a Scatterplot (F-D-S-U)**:

1. **F - Form**: Linear? Curved? No apparent form?
2. **D - Direction**: Positive (sloping upward)? Negative (sloping downward)?
3. **S - Strength**: How tightly do points cluster around the pattern? (Strong/Moderate/Weak)
4. **U - Unusual Features**: Clusters? Points that deviate from the pattern?

### Example

> **Question**: A researcher collected data on weekly study hours and final exam scores for 10 students:
> Study hours: 2, 4, 6, 8, 10, 3, 5, 7, 9, 1
> Exam scores: 55, 60, 65, 75, 85, 58, 62, 70, 80, 50
> Describe the relationship between these two variables.
>
> **Solution**:
> - **Form**: The relationship is roughly **linear**.
> - **Direction**: **Positive** — more study hours are associated with higher exam scores.
> - **Strength**: The points cluster roughly around a line, indicating a **strong** relationship.
> - **Unusual Features**: No obvious outliers or clusters.

---

## Topic 2.5: Correlation

### Detailed Explanation

The **correlation coefficient r** (Pearson correlation coefficient) quantifies the **direction** and **strength** of a **linear** relationship between two quantitative variables.

| Property of r | Explanation |
|---------------|-------------|
| Range | **-1 ≤ r ≤ 1** |
| r > 0 | Positive correlation (x increases, y increases) |
| r < 0 | Negative correlation (x increases, y decreases) |
| r = 0 | No **linear** relationship (but there could be a curved relationship!) |
| r = 1 or -1 | Perfect linear relationship (all points lie on a straight line) |
| Units | **No units** — not affected by measurement scale |

**Important Limitations of r** (must know for the exam!):
1. r only measures the strength of **linear** relationships — even if r is small, there could be a strong curved relationship
2. r is **very sensitive to outliers** — a single outlier can dramatically change r
3. **r ≠ causation** — this is the most important limitation

### Example

> **Question**: The correlation between 10 students' high school GPA and college entrance exam scores is r = 0.65.
> (a) What does this r-value tell you?
> (b) Can you say that "high GPA causes high entrance exam scores"?
>
> **Solution**:
> (a) r = 0.65 indicates a **moderately strong positive linear relationship** between high school GPA and college entrance exam scores. Higher GPAs tend to be associated with higher exam scores.
> (b) **No**. Correlation does not imply causation. Other factors (such as family background, study motivation, etc.) could be influencing both GPA and entrance exam scores.

---

## Topic 2.6-2.8: Linear Regression

### Detailed Explanation

The **Least Squares Regression Line (LSRL)** is the equation of a straight line used to predict the response variable y:
> **ŷ = a + bx**

| Component | Definition | Interpretation |
|-----------|------------|----------------|
| **b (slope)** | Change in ŷ for a 1-unit increase in x | "For each additional hour of study time, the predicted score increases by 3.2 points" |
| **a (y-intercept)** | Value of ŷ when x = 0 | "When study time is 0 hours, the predicted score is 50 points" (Note: may not be practically meaningful) |
| **ŷ (predicted value)** | Predicted value of y for a given x | Used for prediction |
| **r² (coefficient of determination)** | Proportion of the variation in y that is explained by x | "r² = 0.81 means 81% of the variation in exam scores can be explained by study time" |

**Relationship Between the Regression Line and x̄, ȳ**: The LSRL always passes through the point (x̄, ȳ).

**Slope Formula**: b = r × (sy/sx)

**Special Role of r²**: It is the key measure for evaluating the fit of a regression model. The closer r² is to 1, the better the model fits.

### Example

> **Question**: A regression equation from a dataset is ŷ = 52.3 + 3.1x, where x = weekly study hours, and ŷ = predicted exam score. r² = 0.81.
> (a) Interpret the slope 3.1.
> (b) Predict the exam score for a student who studies 5 hours per week.
> (c) Interpret r² = 0.81.
>
> **Solution**:
> (a) For each **1-hour increase** in weekly study time, the predicted exam score **increases by 3.1 points**.
> (b) ŷ = 52.3 + 3.1(5) = 52.3 + 15.5 = **67.8 points**.
> (c) **81%** of the variation in exam scores can be explained by weekly study time. That is, 81% of the changes in exam scores is related to differences in study time.

---

## Topic 2.7: Residuals

### Detailed Explanation

**Residual** = actual value y - predicted value ŷ

- Residual > 0: Actual value is higher than predicted (model underestimated)
- Residual < 0: Actual value is lower than predicted (model overestimated)
- Residual = 0: Perfect prediction

A **Residual Plot** is the **most important tool** for determining whether a linear model is appropriate.

| Pattern in Residual Plot | Conclusion |
|-------------------------|------------|
| **Random scatter (no pattern)** | ✅ Linear model is appropriate |
| **Clear curve/pattern** | ❌ Linear model is not appropriate; a non-linear model is needed |
| **Funnel shape (spread getting wider or narrower)** | ❌ Equal variance condition is violated |

The requirement is that the sum of squared residuals is minimized — this is the origin of the name "least squares."

### Example

> **Question**: A regression model is ŷ = 2x + 1. One observation is (x=3, y=8). Calculate the residual and determine whether the prediction for this point is accurate.
>
> **Solution**:
> Predicted value ŷ = 2(3) + 1 = 6 + 1 = 7
> Residual = y - ŷ = 8 - 7 = **1**
> The actual value is 1 unit higher than the predicted value; the model underestimated the response at this point.

---

## Topic 2.9: Departures from Linearity

### Detailed Explanation

Three types of special points in regression:

| Type of Point | Definition | Effect on Regression |
|--------------|------------|---------------------|
| **Outlier** | Large residual (does not follow the overall trend) | May increase the sum of squared residuals |
| **High-Leverage Point** | x-value is far from the range of other x-values | May "pull" the regression line toward itself |
| **Influential Point** | Significantly changes the regression line when deleted | **High leverage + outlier = strong influence** |

**Dealing with Non-linear Relationships**: Use data transformations (such as taking logs, squaring, etc.) to make the relationship more linear. The criteria for success are that the residual plot becomes more random and r² increases.

### Example

> **Question**: A dataset shows a curved pattern in the scatterplot. r = 0.55. The researcher takes the natural log of y and re-fits the regression, obtaining r² = 0.92. Is this transformation effective?
>
> **Solution**: Yes. Before the transformation, r² ≈ 0.30 (0.55²), meaning the original model explained only 30% of the variation. After the transformation, r² = 0.92 — a substantial improvement. The relationship also changed from curved to linear, indicating that the log transformation was appropriate.

---

# 📋 Unit 3: Collecting Data (Exam Weight: 12-15%)

> **Big Ideas**: VAR + DAT
> **Core Skills**: Skill 1 (Selecting Statistical Methods) + Skill 4 (Statistical Argumentation)

---

## Topic 3.1: Is the Data Telling the Truth?

### Detailed Explanation

The core question of this unit is: **Can we trust the data we collect?** If the data collection method is flawed, then no matter how complex or elegant the subsequent statistical analysis is, the conclusions may be wrong.

**Fundamental Principle**: **Data collection methods that do not rely on randomness lead to untrustworthy conclusions.** All subsequent statistical inference (confidence intervals, hypothesis tests) is built on the assumption that the data were **collected randomly**.

### Example

> **Question**: A company wants to know employee satisfaction with a new work policy. They distribute questionnaires in the company cafeteria and ask employees to fill them out voluntarily. What problems might this collection method have?
>
> **Solution**: This is **Voluntary Response Bias** — only employees who feel strongly about the issue (especially those who are dissatisfied) will take the initiative to fill out the questionnaire. This sample will not represent the opinions of all employees, and the results could be severely biased.

---

## Topic 3.2: Introduction to Study Design

### Detailed Explanation

**Two Basic Types of Studies**:

**Observational Study**: The researcher **does not apply any treatment**; they simply observe and record data.
- Retrospective: Looks back at past data
- Prospective: Follows subjects into the future
- **What it can do**: Discover associations
- **What it cannot do**: Establish causation

**Experiment**: The researcher **actively applies a treatment** and then observes the results.
- **What it can do**: Establish causation (if well-designed)
- **Key requirement**: Must have **random assignment**

**Rules for Generalization**:
- Only **randomly selected** samples can be generalized to the population
- A sample can only be generalized to the **population from which it was drawn**

### Example

> **Question**: A study finds that people who drink coffee daily have a lower risk of heart disease than non-coffee drinkers. Is this an observational study or an experiment? Can we say "coffee drinking reduces heart disease risk"?
>
> **Solution**: This is an **observational study** (the researcher did not require some people to drink coffee and others not to). **We cannot** claim causation, because there may be confounding variables — for example, coffee drinkers might have higher incomes, less stress, or better access to healthcare, and these could be the real reasons for the lower risk.

---

## Topic 3.3: Random Sampling Methods

### Detailed Explanation

Comparison of five sampling methods:

**Simple Random Sampling (SRS)**: The most basic method. Every sample of size n has an equal chance of being selected. The method involves assigning each individual in the population a number, then using a random number table or random number generator to select.

**Stratified Random Sampling**:
- First, divide the population into homogeneous **strata** based on some characteristic (e.g., by grade level)
- Perform SRS within each stratum
- **Advantage**: Ensures representation from each stratum; reduces sampling error

**Cluster Sampling**:
- Divide the population into heterogeneous **clusters** (e.g., by classroom)
- Randomly select a few clusters; **all individuals in the selected clusters** are included in the sample
- **Advantage**: Saves time and cost

**Systematic Random Sampling**:
- Choose a random starting point, then select every k-th individual (e.g., every 10th person)
- **Advantage**: Simple to implement

| Comparison | Stratified Sampling | Cluster Sampling |
|------------|--------------------|-----------------|
| Within-group | Homogeneous (little variation) | Heterogeneous (lots of variation) |
| Between-group | Heterogeneous | Homogeneous |
| Procedure | Sample from every stratum | Randomly select whole clusters |

### Example

> **Question**: A school has 1,000 students across 5 grade levels, 200 students per grade. A researcher wants to survey students about extracurricular activities and needs a sample of 100. She randomly selects 20 students from each grade, forming a sample of 100. What type of sampling method is this?
>
> **Solution**: This is **stratified random sampling**. Grade level is the stratum. Students within the same grade are relatively homogeneous, while students across different grades are likely more different. This method ensures each grade level is represented.

---

## Topic 3.4: Potential Problems with Sampling — Bias

### Detailed Explanation

**Bias** refers to a **systematic** favoring of certain responses over others, rather than random selection.

| Type of Bias | Nature | Example |
|-------------|--------|---------|
| **Voluntary Response Bias** | Only those who actively participate are included | Online polls, call-in hotlines |
| **Undercoverage Bias** | Some groups are excluded | Using only telephone surveys; people without phones are excluded |
| **Nonresponse Bias** | Selected individuals do not respond | Mailed questionnaires with only 30% returned |
| **Response Bias** | Answers are not truthful | Leading questions, interviewer effect |
| **Convenience Sampling** | Selecting the easiest people to reach | Conducting a survey at a mall entrance |

**Key Concept**: Bias is **not** sampling variability. Bias is a systematic error. Increasing the sample size **will not** eliminate bias — it will only make the wrong result more precise.

### Example

> **Question**: A TV station sets up a call-in hotline during a news program, asking viewers "Do you think the mayor is doing a good job?" 85% of callers say "No." Is this result reliable?
>
> **Solution**: **Not reliable**. This is a classic case of **voluntary response bias** — only people with strong feelings about the mayor (especially those who are dissatisfied) would take the time to call. This cannot represent the opinions of the entire city's population.

---

## Topic 3.5-3.6: Experimental Design

### Detailed Explanation

**Core Components of an Experiment**:

| Term | Example |
|------|---------|
| **Experimental Units** (individuals receiving treatment) | Patients, plants, soil samples |
| **Treatment** (condition applied) | New drug vs. placebo |
| **Response Variable** (measured outcome) | Change in blood pressure, cure rate |
| **Factor** (the explanatory variable being manipulated) | Drug dosage |

**Four Principles of a Good Experiment (CRCC)** (must know for the exam!):

1. **C - Comparison**: At least two treatment groups, including a control group
2. **R - Random Assignment**: Randomly assign treatments to units
3. **R - Replication**: More than one experimental unit per treatment group
4. **C - Control**: Control for potential confounding variables

**Blinding**:
- **Single-blind**: Subjects do not know their treatment assignment
- **Double-blind**: Both subjects and researchers do not know the assignment

**Two Forms of Matched Pairs Design**:
1. Pair similar individuals; within each pair, one receives one treatment and the other receives the other
2. The same individual receives both treatments (in sequence)

**Placebo Effect**: Subjects may show a response simply because they believe they are receiving a treatment, even if the treatment is just a sugar pill.

### Example

> **Question**: A study wants to test whether a new fertilizer promotes plant growth. The researcher has 20 identical plants. Design a completely randomized experiment.
>
> **Solution**:
> 1. **Experimental units**: 20 plants
> 2. **Treatments**: New fertilizer (experimental group) vs. plain water (control group)
> 3. **Random assignment**: Number the 20 plants 1-20. Use a random number generator to assign 10 plants to the experimental group (new fertilizer) and 10 to the control group (plain water)
> 4. **Replication**: 10 plants per group (>1, satisfying the replication principle)
> 5. **Control**: Place both groups under the same light and temperature conditions; give them the same amount of water
> 6. **Response variable**: Height of each plant after a period of time
> 7. **Conclusion**: If the experimental group's average height is significantly greater than the control group's, it can be attributed to the new fertilizer

---

## Topic 3.7: Inference and Experiments

### Detailed Explanation

**Statistical significance** means that the observed effect is so large that it is unlikely to be due to random chance alone.

- Random assignment of treatments → the only sources of differences between groups are the **treatment** or **random chance**
- If the difference is so large that it is "unlikely to be due to random chance" → it is called **statistically significant**
- A statistically significant difference is evidence that the **treatment caused the effect**

### Example

> **Question**: In an experiment, the cure rate for the experimental group (new drug) is 75%, and for the control group (placebo) it is 50%. After a statistical test, the p-value is 0.005. Interpret this result.
>
> **Solution**:
> A p-value of 0.005 means that if the new drug actually had no effect (i.e., the two groups should have the same cure rate), the probability of observing a difference this large (or larger) is only 0.5%.
> Since this probability is very small (less than the typical significance level of 0.05), we reject the hypothesis that "the drug has no effect" and **conclude that the drug does increase the cure rate**.

---

# 🎲 Unit 4: Probability, Random Variables, and Probability Distributions (Exam Weight: 10-20%)

> **Big Ideas**: VAR + UNC
> **Core Skills**: Skill 3 (Probability and Simulation) + Skill 4 (Statistical Argumentation)

---

## Topic 4.1: Random vs. Non-Random Patterns

### Detailed Explanation

The core question in the study of probability is: **How do we distinguish random patterns from true patterns?**
- Even if a process is completely random, the data can appear to have a "pattern"
- For example, flipping a fair coin 10 times and getting "H, H, H, T, T, H, H, T, H, T" might look non-random to you, but it is just as likely as "H, T, H, T, H, T, H, T, H, T"
- The statistician's task is to determine whether an observed pattern is **too unusual** to be random

### Example

> **Question**: You flip a fair coin 10 times and get 10 heads in a row. Is this a "random" phenomenon?
>
> **Solution**: If the coin is fair and each flip is independent, the probability of 10 heads is (0.5)^10 ≈ 0.00098, less than 1 in 1,000. This is so rare that we would more likely suspect that **the coin is unfair** rather than attributing it to random fluctuation.

---

## Topic 4.2: Estimating Probabilities Using Simulation

### Detailed Explanation

**Simulation** is a method of using random processes to approximate real-world probabilities. Simulation is very useful when theoretical probabilities are difficult to calculate directly.

**Law of Large Numbers**: The more trials you run, the closer the simulated probability gets to the true probability. For example, flipping a coin 10 times might give 70% heads, but if you flip 10,000 times, the proportion of heads will be very close to 50%.

**Three Steps of Simulation**:
1. Determine the rules of the random process (e.g., use two-digit random numbers 00-99; 00-49 = heads, 50-99 = tails)
2. Repeat the process many times
3. Record the results and calculate the relative frequency

### Example

> **Question**: How would you use simulation to estimate the probability of "rolling a sum of 7 with two dice"?
>
> **Solution**: Use two-digit random numbers: the first digit represents the result of the first die (1-6), and the second digit represents the result of the second die (1-6). Each simulated trial yields a pair of numbers; record whether the sum is 7. Run a large number of trials (e.g., 10,000 times), count the number of times the sum is 7, and divide by the total number of trials. The theoretical probability is 6/36 = 1/6 ≈ 0.167. The simulation result should be close to this value.

---

## Topic 4.3-4.4: Probability Basics and Mutually Exclusive Events

### Detailed Explanation

**Basic Rules of Probability**:
- 0 ≤ P(A) ≤ 1
- The sum of probabilities of all possible outcomes = 1
- Complement Rule: P(not A) = 1 - P(A)

**Mutually Exclusive Events** are events that **cannot happen at the same time**.
- If A and B are mutually exclusive, then P(A ∩ B) = 0
- Addition Rule for mutually exclusive events: P(A ∪ B) = P(A) + P(B)

### Example

> **Question**: Draw one card from a standard 52-card deck.
> (a) Event A = "draw a heart," Event B = "draw a spade." Are A and B mutually exclusive?
> (b) Event A = "draw a heart," Event C = "draw a King." Are A and C mutually exclusive?
>
> **Solution**:
> (a) **Mutually exclusive** — a single card cannot be both a heart and a spade. P(A ∪ B) = 13/52 + 13/52 = 26/52 = 0.5.
> (b) **Not mutually exclusive** — the King of Hearts is both a heart and a King, so P(A ∩ C) = 1/52. P(A ∪ C) = 13/52 + 4/52 - 1/52 = 16/52 ≈ 0.308.

---

## Topic 4.5: Conditional Probability

### Detailed Explanation

**Conditional probability** answers: **Given some information, how does the probability change?**

Formula: P(A|B) = P(A ∩ B) / P(B)

**Multiplication Rule**: P(A ∩ B) = P(A) × P(B|A)

**Tree diagrams** are the most intuitive tool for solving conditional probability problems — they display all possible branch paths.

A classic application: **The false positive problem** — even if a test has 95% accuracy, if the disease is very rare in the population, the probability that a person who tests positive actually has the disease may still be very low.

### Example

> **Question**: In a class, 60% are female and 40% are male. Among females, 30% wear glasses. Among males, 20% wear glasses. A student is randomly selected and found to wear glasses. What is the probability that this student is female?
>
> **Solution**:
> Let A = "wears glasses," B = "is female"
> P(B) = 0.60, P(A|B) = 0.30, P(A|not B) = 0.20
> P(A) = P(A ∩ B) + P(A ∩ not B) = 0.60 × 0.30 + 0.40 × 0.20 = 0.18 + 0.08 = 0.26
> P(B|A) = P(A ∩ B)/P(A) = 0.18/0.26 ≈ **0.692**
> There is approximately a 69.2% probability.

---

## Topic 4.6: Independent Events

### Detailed Explanation

**Independence** is one of the most important concepts in probability theory.

Conditions for events A and B to be independent (three equivalent conditions; **satisfying any one is sufficient**):
1. P(A|B) = P(A) — knowing B occurs does not change the probability of A
2. P(B|A) = P(B) — knowing A occurs does not change the probability of B
3. P(A ∩ B) = P(A) × P(B) — the product rule

**⚠️ Important Distinction**:
- **Mutually exclusive events**: If A occurs, B cannot occur (strong dependence)
- **Independent events**: A occurring does not affect the probability of B (no dependence)
- Mutually exclusive events are **definitely not independent** (unless one has probability 0)

### Example

> **Question**: Flip two fair coins. Event A = "first coin is heads," Event B = "second coin is heads." Are A and B independent?
>
> **Solution**:
> P(A) = 0.5, P(B) = 0.5, P(A ∩ B) = 0.5 × 0.5 = 0.25
> Since P(A ∩ B) = 0.25 = 0.5 × 0.5 = P(A) × P(B),
> A and B are **independent**. Knowing the result of the first coin does not change the probability that the second coin will be heads.

---

## Topic 4.7-4.8: Random Variables

### Detailed Explanation

A **random variable** maps the outcomes of a random process to numbers.

A **discrete random variable** can take a countable number of values. For example, "number of heads in 3 coin flips" can only be 0, 1, 2, 3.

A **probability distribution** lists each possible value and its corresponding probability:
- All probabilities ≥ 0
- Sum of all probabilities = 1

**Mean (Expected Value)**: μ = Σ[x_i × P(x_i)]
- Interpreted as the long-run average — if the experiment is repeated infinitely many times, the average will converge to this value

**Standard Deviation**: σ = √Σ[(x_i - μ)² × P(x_i)]
- Measures the spread of the random variable

### Example

> **Question**: The probability distribution of a discrete random variable X is:
> X:   1    2    3    4
> P:  0.2  0.3  0.4  0.1
> Find the mean and standard deviation of X.
>
> **Solution**:
> Mean μ = 1(0.2) + 2(0.3) + 3(0.4) + 4(0.1) = 0.2 + 0.6 + 1.2 + 0.4 = **2.4**
> Variance σ² = (1-2.4)²(0.2) + (2-2.4)²(0.3) + (3-2.4)²(0.4) + (4-2.4)²(0.1)
>            = 1.96(0.2) + 0.16(0.3) + 0.36(0.4) + 2.56(0.1)
>            = 0.392 + 0.048 + 0.144 + 0.256 = 0.84
> Standard deviation σ = √0.84 ≈ **0.917**

---

## Topic 4.9: Combining Random Variables

### Detailed Explanation

When dealing with multiple random variables, you need to know how to compute the mean and variance of their sums, differences, and linear transformations.

**Summary of Rules**:

| Operation | Mean | Variance |
|-----------|------|----------|
| Y = a + bX | a + bμ_X | b²σ²_X |
| X + Y (independent) | μ_X + μ_Y | σ²_X + σ²_Y |
| X - Y (independent) | μ_X - μ_Y | σ²_X + σ²_Y |

**Key Insight**: Variance **always adds**, whether it's a sum or a difference. This is because variability only accumulates; it does not cancel out.

**A linear transformation Y = a + bX does not change the shape of the distribution** (as long as b > 0).

### Example

> **Question**: Random variable X (temperature in °C) has a mean of 20 and a variance of 4. Convert the temperature to Fahrenheit: Y = 32 + 1.8X. Find the mean and standard deviation of Y.
>
> **Solution**:
> Mean μ_Y = 32 + 1.8(20) = 32 + 36 = **68°F**
> Variance σ²_Y = (1.8)²(4) = 3.24 × 4 = 12.96
> Standard deviation σ_Y = √12.96 = **3.6°F**

---

## Topic 4.10-4.12: Binomial and Geometric Distributions

### Detailed Explanation

**Conditions for the Binomial Distribution (BINS)**:

| Condition | Meaning |
|-----------|---------|
| **B**inary | Each trial has only two outcomes: success/failure |
| **I**ndependent | Trials are independent of each other |
| **N**umber fixed | The number of trials n is fixed in advance |
| **S**ame probability | The probability of success p is the same for each trial |

**Key Formulas**:
- P(X=x) = C(n,x) × p^x × (1-p)^(n-x)
- Mean μ = np
- Standard Deviation σ = √[np(1-p)]

**Key Differences Between the Geometric Distribution and the Binomial Distribution**:

| Feature | Binomial | Geometric |
|---------|----------|-----------|
| Meaning of X | Number of successes in n trials | **Which trial** the first success occurs on |
| n | Fixed in advance | Not fixed |
| Meaning of mean | Expected number of successes | Expected number of trials until first success |
| Mean formula | np | 1/p |

### Example (Binomial)

> **Question**: A survey shows that 60% of residents in a city support a new policy. Randomly survey 10 residents. Assume they are independent. Find the probability that exactly 7 support it.
>
> **Solution**:
> This is binomial: n=10, p=0.60, X = "number of supporters"
> P(X=7) = C(10,7) × (0.60)^7 × (0.40)^3
> Using a calculator (binompdf(10, 0.6, 7)) gives ≈ **0.215**

### Example (Geometric)

> **Question**: Roll a fair die. How many rolls does it take to get the first 6? What is the expected number of rolls?
>
> **Solution**:
> This is geometric: p = 1/6, X = "number of rolls until the first 6"
> P(X=1) = 1/6
> P(X=2) = (5/6)(1/6) ≈ 0.139
> P(X=3) = (5/6)²(1/6) ≈ 0.116
> And so on...
> Mean μ = 1/(1/6) = **6 rolls** (on average, it takes 6 rolls to get a 6)

---

# 🎯 Unit 5: Sampling Distributions (Exam Weight: 7-12%)

> **⚠️ This is the most critical bridge unit from "descriptive statistics" to "statistical inference"!**
> **Big Ideas**: VAR + UNC
> **Core Skills**: Skill 3 (Probability and Simulation) + Skill 4 (Statistical Argumentation)

---

## Topic 5.1: Why Is My Sample Different from Yours?

### Detailed Explanation

**Core Concept**: Even when repeatedly sampling from the same population, each sample's statistic (e.g., mean, proportion) will differ. This is **Sampling Variability**.

A **Sampling Distribution** is the distribution of a statistic across **all possible samples**. It is different from:
- **Population distribution**: The distribution of all individuals in the population
- **Sample distribution**: The distribution of data within a single sample

### Example

> **Question**: A population consists of 5 numbers: {2, 4, 6, 8, 10}. Draw all possible samples of size 2 with replacement and calculate the sample mean. What kind of distribution do these sample means form?
>
> **Solution**:
> All possible samples (with replacement):
> (2,2)→2, (2,4)→3, (2,6)→4, (2,8)→5, (2,10)→6
> (4,2)→3, (4,4)→4, (4,6)→5, (4,8)→6, (4,10)→7
> ... and so on, for a total of 25 samples.
> The distribution of these means is called the **sampling distribution**. It is centered around the population mean μ=6 and has a natural amount of variability.

---

## Topic 5.2: Review of the Normal Distribution

### Detailed Explanation

A **continuous random variable** can take any value within a specified interval. Each interval has a corresponding probability.

**Key Properties of the Continuous Normal Distribution**:
- Total area under the curve = 1
- **Area** under a specific interval = **probability** of that interval
- Given a probability, finding the corresponding boundary → use the **inverse of the standard normal table** or a calculator's invNorm function

### Example

> **Question**: For a normal distribution with μ=100, σ=15, find the probability of a value less than 85.
>
> **Solution**:
> z = (85-100)/15 = -15/15 = -1.0
> P(Z < -1.0) ≈ **0.1587** (about 16%)
> That is, about 16% of values in this distribution are less than 85.

---

## Topic 5.3: The Central Limit Theorem (CLT)

### Detailed Explanation

The **Central Limit Theorem (CLT)** is the **foundational theorem** of all statistics.

> **Core Statement of the CLT**: Regardless of the shape of the population distribution, when the sample size n is large enough, the **sampling distribution of the sample mean** is approximately **normal**.

More precisely:
- Mean of the sampling distribution = population mean μ
- Standard deviation of the sampling distribution = σ/√n (called the **Standard Error**)
- When **n ≥ 30**, the approximation is typically quite good

**⚠️ Two prerequisites for the CLT**:
1. **Independence**: Sample observations must be independent of each other (typically ensured by random sampling; check the 10% condition when sampling without replacement)
2. **Sufficient sample size**: Typically n ≥ 30 (but a more skewed population may require a larger n)

Only when **both** conditions are satisfied does the CLT apply.

**The Power of the CLT**: Even if the population is heavily skewed, bimodal, or even "U-shaped," as long as n is large enough, the distribution of sample means is (approximately) normal. This explains why the normal distribution is so important in statistics.

**Two Cases for the CLT**:

| Scenario | Normality Condition |
|----------|-------------------|
| Population is normal | Any n (n ≥ 2) — the sampling distribution of x̄ is exactly normal, but a t-test requires n ≥ 2 to estimate s |
| Population is not normal | Need n ≥ 30 (rule of thumb) |

### Example

> **Question**: A population distribution is **skewed right**, with mean μ=50 and standard deviation σ=20. If we randomly draw a sample of n=50 from this population, find the mean and standard deviation of the sampling distribution of the sample mean. What is the **shape** of this sampling distribution?
>
> **Solution**:
> Mean μ_x̄ = μ = **50**
> Standard deviation σ_x̄ = σ/√n = 20/√50 ≈ 20/7.07 ≈ **2.83**
> Since n=50 ≥ 30, by the **Central Limit Theorem**, the shape of the sampling distribution is **approximately normal** (even though the population is skewed right).

---

## Topic 5.4: Biased and Unbiased Point Estimation

### Detailed Explanation

**Point Estimate**: Using a single value from a sample statistic to estimate a population parameter.

**Unbiased Estimator**: If the average value of the statistic across all possible samples equals the population parameter, then the statistic is unbiased.

| Statistic | Parameter Estimated | Unbiased? |
|-----------|-------------------|-----------|
| Sample mean x̄ | Population mean μ | ✅ Unbiased |
| Sample proportion p̂ | Population proportion p | ✅ Unbiased |
| Sample standard deviation s | Population standard deviation σ | Biased (but the bias is small; negligible for large n) |
| Sample median | Population median | ✅ Roughly unbiased |

### Example

> **Question**: Explain why the sample mean x̄ is an unbiased estimator of the population mean μ.
>
> **Solution**: If you took all possible samples of the same size from a population, calculated the mean of each sample, and then averaged those sample means, the result would be exactly equal to the population mean μ. This is the meaning of unbiased — "on average," the estimator equals the parameter being estimated. Although an individual sample mean may overestimate or underestimate μ, the **long-run average** is accurate.

---

## Topic 5.5-5.6: Sampling Distribution of a Sample Proportion

### Detailed Explanation

**Sampling Distribution of p̂**:

| Property | Formula |
|----------|---------|
| **Mean** | μ_p̂ = p |
| **Standard deviation** | σ_p̂ = √[p(1-p)/n] |
| **Normality condition** | np ≥ 10 and n(1-p) ≥ 10 |
| **10% condition** | n ≤ 0.10N (when sampling without replacement) |

**Sampling Distribution of the Difference Between Two Proportions (p̂₁ - p̂₂)**:

| Property | Formula |
|----------|---------|
| **Mean** | μ = p₁ - p₂ |
| **Standard deviation** | √[p₁(1-p₁)/n₁ + p₂(1-p₂)/n₂] |
| **Normality condition** | All four quantities are ≥ 10 |
| **Independence** | The two samples must be independent of each other |

### Example

> **Question**: In a population, 40% support a certain policy. A random sample of n=100 is drawn.
> (a) What are the mean and standard deviation of the sampling distribution of p̂?
> (b) Can this sampling distribution be approximated by a normal distribution?
>
> **Solution**:
> (a) Mean = p = **0.40**
>     Standard deviation = √[0.40(0.60)/100] = √[0.24/100] = √0.0024 ≈ **0.049**
> (b) np = 100 × 0.40 = 40 ≥ 10 ✅
>     n(1-p) = 100 × 0.60 = 60 ≥ 10 ✅
>     Both conditions are satisfied, so a normal approximation is appropriate.
>
> For the normality condition of the sampling distribution, we check np and n(1-p), where p is the **population proportion**. Here p=0.40 is a known population proportion, so this is fine. When p is unknown, we use p̂ instead.

---

## Topic 5.7-5.8: Sampling Distribution of a Sample Mean

### Detailed Explanation

**Sampling Distribution of x̄**:

| Property | Formula |
|----------|---------|
| **Mean** | μ_x̄ = μ |
| **Standard deviation (Standard Error)** | σ_x̄ = σ/√n |
| **Normality condition** | Population is normal (any n) or n ≥ 30 (CLT) |
| **10% condition** | n ≤ 0.10N |

**Sampling Distribution of the Difference Between Two Means (x̄₁ - x̄₂)**:

| Property | Formula |
|----------|---------|
| **Mean** | μ₁ - μ₂ |
| **Standard deviation** | √(σ₁²/n₁ + σ₂²/n₂) |
| **Normality condition** | Both populations are normal OR both sample sizes are ≥ 30 |

### Example

> **Question**: The length of parts produced in a factory follows a distribution with mean μ=10 cm and standard deviation σ=0.5 cm. A random sample of n=36 parts is drawn. Find the mean, standard deviation, and shape of the sampling distribution of the sample mean x̄.
>
> **Solution**:
> Mean μ_x̄ = **10 cm**
> Standard deviation σ_x̄ = 0.5/√36 = 0.5/6 ≈ **0.083 cm**
> Shape: Although the problem does not state that the population is normal, n=36 ≥ 30, so by the **CLT**, the sampling distribution is approximately **normal**.

---

# ✅ Unit 6: Inference for Categorical Data — Proportions (Exam Weight: 12-15%)

> **⚠️ This is the first "real inference" unit — the process must be second nature!**
> **Core Process**: **Check Conditions → Calculate → Conclude**
> **Big Ideas**: VAR + UNC + DAT

---

## Topic 6.1: Building a Confidence Interval for a Population Proportion

### Detailed Explanation

A **Confidence Interval** uses **sample data** to provide a **plausible range of values** for a population parameter.

**General Formula**: **Statistic ± Critical Value × Standard Error**

**Confidence Interval for a Single Population Proportion**:
- **Formula**: p̂ ± z* × √[p̂(1-p̂)/n]
- z* depends on the confidence level: 90%→1.645, 95%→1.96, 99%→2.576

**Three Conditions That Must Be Checked (R.N.I.)** (must know for the exam!):

| Condition | How to Check |
|-----------|-------------|
| **R - Random** | Data come from a random sample or a randomized experiment |
| **N - Normal** | np̂ ≥ 10 and n(1-p̂) ≥ 10 (large counts condition) |
| **I - Independent** | n ≤ 0.10N (10% condition, when sampling without replacement) |

**Correct Interpretation of a Confidence Interval** (⚠️ Common Mistake):
- ✅ **Correct**: "We are 95% confident that the population proportion **lies in** this interval."
- ✅ **Correct**: "If we repeatedly took samples of the same size and constructed 95% confidence intervals, **about 95%** of those intervals would contain the true population proportion."
- ❌ **Incorrect**: "There is a 95% probability that the population proportion falls within this interval." (The population proportion is a fixed value, not a random variable!)

### Example

> **Question**: 200 residents were surveyed, and 120 support a new policy. Construct a 95% confidence interval for the population proportion in favor.
>
> **Solution**:
> **Check Conditions**:
> - Randomness: Assume the sample was randomly selected ✅
> - Normality: np̂ = 200 × 0.6 = 120 ≥ 10, n(1-p̂) = 200 × 0.4 = 80 ≥ 10 ✅
> - Independence: Assume the population > 2000 people, satisfying the 10% condition ✅
>
> **Calculate**:
> p̂ = 120/200 = 0.60
> SE = √[0.60 × 0.40/200] = √[0.24/200] = √0.0012 ≈ 0.0346
> z* = 1.96 (for 95% confidence)
> Interval = 0.60 ± 1.96 × 0.0346 = 0.60 ± 0.0678
> **Conclusion**: We are 95% confident that the proportion of all residents who support the policy is between **53.2% and 66.8%**.

---

## Topic 6.3: Making Claims Based on a Confidence Interval

### Detailed Explanation

**Using a Confidence Interval to Test a Claim**:
- If a hypothesized value is **not** inside the confidence interval → there is evidence to reject that hypothesis
- If a hypothesized value **is** inside the confidence interval → there is not enough evidence to reject it

### Example

> **Question**: In the previous problem, someone claims "the support rate is exactly 50%." Does the confidence interval [0.532, 0.668] support this claim?
>
> **Solution**: **No**. 0.50 is not within the confidence interval [0.532, 0.668]. We are 95% confident that the true support proportion is between 53.2% and 66.8%. Since 50% lies below the lower bound, there is evidence that the support rate is not 50%.

---

## Topic 6.4-6.6: Hypothesis Testing

### Detailed Explanation

**Process of a Hypothesis Test (Significance Test)**:

**Step 1: State the Hypotheses**
- **Null Hypothesis H₀**: A statement of "no effect" or "no difference"
- **Alternative Hypothesis Hₐ**: The statement we are looking for evidence to support

For example, testing whether the support rate is 50%:
- H₀: p = 0.50
- Hₐ: p ≠ 0.50 (two-sided test)

**Step 2: Check Conditions** (same as for confidence intervals)

**Step 3: Calculate the Test Statistic and p-value**
- Test statistic: z = (p̂ - p₀) / √[p₀(1-p₀)/n]
- p-value: The probability of observing the current result (or something more extreme), assuming H₀ is true

**Step 4: Make a Conclusion**
- p-value < α → Reject H₀; there is statistically significant evidence supporting Hₐ
- p-value ≥ α → Fail to reject H₀; there is not enough evidence

**Important Distinction**:
- **α (significance level)**: The threshold set **before** collecting data, representing "the maximum Type I error risk I am willing to accept." Usually 0.05.
- **p-value**: The probability **computed after** collecting data, representing "the probability of observing the current or more extreme results, assuming H₀ is true."
- **Comparison rule**: Compare the p-value to α to make a decision. **Do not confuse the p-value with α!**

**⚠️ Correct Understanding of the p-value** (extremely important!):
- ✅ p-value = **P(observed result or more extreme | H₀ is true)**
- ❌ p-value ≠ **P(H₀ is true | data)**

### Example

> **Question**: Test whether the support rate is 50%. 120 out of 200 people support. Use α = 0.05.
>
> **Solution**:
> **H₀**: p = 0.50
> **Hₐ**: p ≠ 0.50
>
> **Check Conditions** (same as previous problem, satisfied) ✅
>
> **Calculate**:
> p̂ = 0.60
> z = (0.60 - 0.50) / √[0.50 × 0.50/200] = 0.10/0.0354 ≈ **2.83**
> p-value (two-sided) = 2 × P(Z > 2.83) ≈ 2 × 0.0023 ≈ **0.0046**
>
> **Conclusion**: p-value (0.0046) < α (0.05), reject H₀. There is statistically significant evidence that the support rate is **not 50%** (in fact, it is higher than 50%).

---

## Topic 6.7: Potential Errors

### Detailed Explanation

| Error Type | Definition | Analogy | Probability |
|-----------|------------|---------|-------------|
| **Type I Error** | Rejecting a true H₀ | Convicting an innocent person | α (significance level) |
| **Type II Error** | Failing to reject a false H₀ | Letting a guilty person go free | β |

**Power of a Test** = 1 - β = The probability of correctly rejecting a false H₀

**Trade-off Between α and β**:
- Decreasing α → harder to reject H₀ → β increases (Type II error increases)
- Increasing sample size n → standard error decreases → easier to detect a real difference → β decreases → Power increases

### Example

> **Question**: When testing whether a new drug is effective, the researcher sets α = 0.05.
> (a) What is a Type I error?
> (b) What does α = 0.05 mean?
>
> **Solution**:
> (a) A Type I error would be: The drug is actually ineffective (H₀ is true), but the test concludes it is effective (rejects H₀).
> (b) α = 0.05 means that if the drug is truly ineffective, the researcher has at most a 5% chance of incorrectly concluding that it is effective.

---

## Topic 6.8-6.11: Comparing Two Proportions

### Detailed Explanation

**Confidence Interval for the Difference Between Two Proportions**:
- (p̂₁ - p̂₂) ± z* × √[p̂₁(1-p̂₁)/n₁ + p̂₂(1-p̂₂)/n₂]

**Test for the Difference Between Two Proportions**:
- H₀: p₁ - p₂ = 0 (or p₁ = p₂)
- For the test, use the **pooled proportion**: p̂_c = (total successes)/(total trials)

### Example

> **Question**: Compare the pass rates of two teaching methods. Method A: 48 out of 60 pass (80%). Method B: 35 out of 50 pass (70%). Construct a 95% confidence interval for the difference in proportions.
>
> **Solution**:
> p̂₁ = 0.80, p̂₂ = 0.70
> Difference = 0.80 - 0.70 = 0.10
> SE = √[0.80 × 0.20/60 + 0.70 × 0.30/50] = √[0.00267 + 0.00420] = √0.00687 ≈ 0.0829
> Interval = 0.10 ± 1.96 × 0.0829 = 0.10 ± 0.1625 = **[-0.0625, 0.2625]**
> Since the interval contains 0, we cannot say there is a statistically significant difference.

---

# 📏 Unit 7: Inference for Quantitative Data — Means (Exam Weight: 10-18%)

> **Big Ideas**: VAR + UNC + DAT
> **Core Skills**: Skills 1, 3, 4

---

## Topic 7.2-7.5: One-Sample t-Test and Confidence Interval

### Detailed Explanation

**Key Difference**: When making inferences about **means**, we use the **t-distribution** instead of the normal distribution. This is because the population standard deviation σ is unknown, and we estimate it with the **sample standard deviation s**, which introduces additional uncertainty.

**Characteristics of the t-distribution**:
- Similar shape to the normal distribution (bell-shaped, symmetric)
- Has **thicker tails** (reflecting greater uncertainty)
- Shape is determined by **degrees of freedom df = n-1**
- As df increases, the t-distribution approaches the normal distribution

**One-Sample t Confidence Interval**:
> x̄ ± t* × (s/√n)

**One-Sample t-Test**:
> t = (x̄ - μ₀) / (s/√n), df = n-1

**Check Conditions**:
1. **Randomness**: Random sample
2. **Normality**: Population is normal OR n ≥ 30 (CLT). If n is small and the population is clearly not normal, the t method is not appropriate
3. **Independence**: 10% condition

### Example

> **Question**: Math scores for 10 students: 72, 85, 91, 67, 88, 73, 94, 80, 79, 86. Test whether the mean score is 80 (α = 0.05).
>
> **Solution**:
> **H₀**: μ = 80, **Hₐ**: μ ≠ 80
>
> **Check Conditions**: Assume random sample ✅. n=10 < 30, so we cannot rely on the CLT. We need to check whether the sample data appear to come from an approximately normal population. The scores range from 67 to 94, the median is about 82.5, the mean is 81.5, the distribution is roughly symmetric with no obvious outliers. The t method is approximately reasonable. 10% condition ✅.
>
> **Calculate**:
> x̄ = (72+85+91+67+88+73+94+80+79+86)/10 = 815/10 = **81.5**
> s = √[Σ(xi-x̄)²/(n-1)] = √[702.5/9] = √78.056 ≈ **8.84**
> t = (81.5 - 80) / (8.84/√10) = 1.5/2.795 ≈ **0.537**
> df = 10 - 1 = 9
> Two-sided p-value ≈ **0.604**
>
> **Conclusion**: p-value (0.604) > α (0.05), **fail to reject H₀**. There is not enough evidence to conclude that the mean score differs from 80.

---

## Topic 7.6-7.9: Comparing Two Means

### Detailed Explanation

**Independent Two-Sample t-Test**:
- H₀: μ₁ - μ₂ = 0
- Formula: t = (x̄₁ - x̄₂) / √(s₁²/n₁ + s₂²/n₂)
- Degrees of freedom use the Welch-Satterthwaite approximation (handled automatically by calculators)
- **For small n (<30)**: We need to check whether the sample data themselves appear to come from approximately normal populations. A more rigorous approach is to check for strong skewness or outliers in the data.

**Matched Pairs t-Test**:
- This is a method for **paired data**, not independent two-sample data!
- Compute the difference d = x₁ - x₂ for each pair
- Perform a **one-sample t-test** on the differences
- H₀: μ_d = 0

| Distinction | Independent Two-Sample | Paired |
|------------|----------------------|--------|
| Data relationship | Two independent groups | Paired/related (same individual or matched pairs) |
| Analysis method | Two-sample t-test | One-sample t-test on differences |
| Degrees of freedom | Approximate formula | n_d - 1 |

### Example (Paired)

> **Question**: Scores for 8 athletes before and after training:
> Before: 65, 72, 68, 70, 66, 74, 69, 71
> After: 67, 75, 70, 73, 68, 76, 72, 73
> Did training significantly improve performance? (α = 0.05)
>
> **Solution**:
> This is **paired data** (the same person measured before and after training).
> Differences d = After - Before: 2, 3, 2, 3, 2, 2, 3, 2
> x̄_d = 19/8 = **2.375**
> s_d ≈ **0.518**
>
> **H₀**: μ_d = 0, **Hₐ**: μ_d > 0 (one-sided)
> t = 2.375/(0.518/√8) = 2.375/0.183 ≈ **12.98**
> df = 8 - 1 = 7
> p-value ≈ **0.000003** (extremely small)
>
> **Conclusion**: p-value is far less than α = 0.05, reject H₀. There is extremely strong statistical evidence that **training did improve performance**.

---

# 🔤 Unit 8: Inference for Categorical Data — Chi-Square Tests (Exam Weight: 2-5%)

> **Big Ideas**: VAR + UNC + DAT
> **Core Skills**: Skills 1, 3, 4

---

## Topic 8.2-8.3: Chi-Square Goodness of Fit Test

### Detailed Explanation

The **Chi-Square Goodness of Fit Test** answers: Does the distribution of a categorical variable match a theoretical distribution?

- **H₀**: The variable's distribution matches the theoretical distribution
- **Hₐ**: The variable's distribution does not match the theoretical distribution

**Formula**: χ² = Σ[(O - E)²/E]
- O = Observed frequency
- E = Expected frequency
- df = (number of categories) - 1

**Condition**: All expected frequencies E ≥ 5

### Example

> **Question**: A die is rolled 60 times with the following results:
> Face:    1    2    3    4    5    6
> Count:   8    9    11   10   12   10
> Test whether the die is fair (α = 0.05).
>
> **Solution**:
> **H₀**: The die is fair (each face has probability 1/6)
> **Hₐ**: The die is not fair
>
> Expected frequency: 60 × (1/6) = 10 for each face (all E=10 ≥ 5 ✅)
>
> χ² = (8-10)²/10 + (9-10)²/10 + (11-10)²/10 + (10-10)²/10 + (12-10)²/10 + (10-10)²/10
>    = 0.4 + 0.1 + 0.1 + 0 + 0.4 + 0 = **1.0**
> df = 6 - 1 = 5
> p-value ≈ **0.963**
>
> **Conclusion**: p-value (0.963) is much larger than α (0.05), fail to reject H₀. **There is no evidence that the die is unfair.**

---

## Topic 8.5-8.6: Test of Homogeneity and Test of Independence

### Detailed Explanation

| Test | Question | Data | H₀ |
|------|----------|------|-----|
| **Goodness of Fit** | Does the distribution match a theory? | Single variable, single sample | Follows the theoretical distribution |
| **Test of Homogeneity** | Are the distributions across different groups the same? | Single variable, multiple groups | All groups have the same distribution |
| **Test of Independence** | Are two variables independent? | Two variables, single sample | The two variables are independent |

**Both Tests Use the Exact Same Formula**:
- χ² = Σ[(O-E)²/E]
- df = (number of rows - 1)(number of columns - 1)
- Condition: All E ≥ 5

**Expected Frequency Formula**: E = (Row Total × Column Total) / Grand Total

### Example (Test of Independence)

> **Question**: Data from 200 people: Gender (Male/Female) and whether they like sports (Like/Dislike). Test whether gender and liking sports are independent (α = 0.05).
>
> Data:
> | | Like | Dislike | Total |
> |---|------|---------|-------|
> | Male | 70 | 30 | 100 |
> | Female | 50 | 50 | 100 |
> | Total | 120 | 80 | 200 |
>
> **Solution**:
> **H₀**: Gender and liking sports are independent
> **Hₐ**: Gender and liking sports are not independent (associated)
>
> **Expected Frequencies** (using "Male & Like" as an example):
> E = (100 × 120)/200 = 12000/200 = 60
> Similarly: E(Male, Dislike) = 40, E(Female, Like) = 60, E(Female, Dislike) = 40
>
> χ² = (70-60)²/60 + (30-40)²/40 + (50-60)²/60 + (50-40)²/40
>    = 100/60 + 100/40 + 100/60 + 100/40
>    = 1.667 + 2.5 + 1.667 + 2.5 = **8.334**
> df = (2-1)(2-1) = 1
> p-value ≈ **0.004**
>
> **Conclusion**: p-value (0.004) < α (0.05), reject H₀. There is statistically significant evidence that gender and liking sports **are associated**.

---

# ⛰️ Unit 9: Inference for Quantitative Data — Slopes (Exam Weight: 2-5%)

> **Big Ideas**: VAR + UNC + DAT
> **Core Skills**: Skills 1, 3, 4

---

## Topic 9.2-9.5: Inference for Regression Slopes

### Detailed Explanation

This unit answers: **Is there a statistically significant linear relationship between two quantitative variables?**

**Confidence Interval for the Slope**:
> b ± t* × SE(b)
> df = n - 2

**Hypothesis Test for the Slope**:
- **H₀**: β = 0 (there is **no linear relationship** between the explanatory variable x and the response variable y)
- **Hₐ**: β ≠ 0 (there is a linear relationship)
- **Test statistic**: t = (b - 0) / SE(b)
- df = n - 2

**Four Conditions for Regression Inference (LINE)** (must know for the exam!):

| Condition | Check | Result |
|-----------|-------|--------|
| **L – Linearity** | Scatterplot shows a **linear trend**; residual plot shows **random scatter** (no obvious curved pattern) | ✅ Satisfied |
| **I – Independence** | Data come from a random sample; observations are **independent** of each other | ✅ Satisfied |
| **N – Normality** | For n < 30, check the residual distribution; the histogram/normal probability plot of residuals is **roughly symmetric** | ✅ Approximately satisfied |
| **E – Equal Variance (Homoscedasticity)** | Residual plot shows residuals have **roughly the same spread** across all x values (no funnel shape) | ✅ Satisfied |

### Example

> **Question**: From 10 data points, the regression output is: ŷ = 3.2 + 1.5x, with standard error of the slope SE(b) = 0.35.
> (a) Test whether there is a linear relationship (α = 0.05).
> (b) Construct a 95% confidence interval for the slope.
>
> **Solution**:
> **Check LINE Conditions** (see table above — all satisfied) ✅
>
> (a) **H₀**: β = 0, **Hₐ**: β ≠ 0
>     t = (1.5 - 0)/0.35 ≈ **4.286**
>     df = 10 - 2 = 8
>     Two-sided p-value ≈ **0.0026**
>     **Conclusion**: p-value (0.0026) < α (0.05), reject H₀. There is statistically significant evidence of a linear relationship between x and y.
>
> (b) t* (df=8, 95% confidence) = 2.306
>     Confidence interval = 1.5 ± 2.306 × 0.35 = 1.5 ± 0.807 = **[0.693, 2.307]**
>     Since 0 is not in the interval, this supports the conclusion that a linear relationship exists.

---

# Part 3: Complete Guide to Choosing an Inference Method

The biggest challenge on the exam: **Given a problem, choose the correct inference method!**

Here is a decision tree based on **data characteristics**:

## Identify by Outcome

| Data Type | Question | Method |
|-----------|----------|--------|
| **One categorical variable** | Does it follow a certain distribution? | **Chi-square goodness of fit test** |
| **One categorical variable** | What is the population proportion? | **One-proportion z confidence interval** |
| **One categorical variable** | Is the population proportion equal to a certain value? | **One-proportion z-test** |
| **Two categorical variables (one sample)** | Are the two variables independent? | **Chi-square test of independence** |
| **Two categorical variables (multiple samples)** | Are the distributions the same across groups? | **Chi-square test of homogeneity** |
| **One quantitative variable** | What is the population mean? | **One-sample t confidence interval** |
| **One quantitative variable** | Is the population mean equal to a certain value? | **One-sample t-test** |
| **One quantitative variable (paired data)** | Is the mean of the paired differences zero? | **Paired t-test** |
| **Two quantitative variables (independent)** | Are the two population means equal? | **Independent two-sample t-test** |
| **Two categorical variables (two proportions)** | What is the difference between two proportions? | **Two-proportion z-test/confidence interval** |
| **Two quantitative variables (regression)** | Is the slope zero (is there a linear relationship)? | **Slope t-test/confidence interval** |

---

This completes the full English translation of your AP Statistics knowledge guide. The content preserves all original structure, formatting, equations, and examples while maintaining statistical precision in English terminology.
