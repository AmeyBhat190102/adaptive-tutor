# Statistics and Probability

## Descriptive Statistics

### Measures of Central Tendency
These describe the "centre" of a dataset.

**Mean (Average)**
Sum of all values divided by the count.
- Mean = Σx / n
- Example: {4, 7, 2, 9, 3} → Mean = (4+7+2+9+3)/5 = 25/5 = 5
- Sensitive to outliers

**Median**
The middle value when data is sorted. If there is an even number of values, take the mean of the two middle values.
- Example (odd): {2, 3, 4, 7, 9} → Median = 4
- Example (even): {2, 3, 4, 7} → Median = (3+4)/2 = 3.5
- Not affected by outliers — useful for skewed data (e.g., income)

**Mode**
The most frequently occurring value. A dataset can have no mode, one mode, or multiple modes.
- Example: {2, 3, 3, 5, 7, 3, 9} → Mode = 3

### Measures of Spread
These describe how spread out the data is.

**Range**
Range = Maximum - Minimum
- Simple but sensitive to outliers

**Variance**
Average of the squared differences from the mean.
- Population variance: σ² = Σ(x - μ)² / N
- Sample variance: s² = Σ(x - x̄)² / (n-1)

**Standard Deviation**
Square root of variance. Same units as the original data.
- σ = √(σ²)
- Small SD → data clustered near mean
- Large SD → data spread out

**Interquartile Range (IQR)**
IQR = Q3 - Q1 (middle 50% of data)
- Q1: median of lower half
- Q3: median of upper half
- Resistant to outliers

## Probability

### Basic Probability
Probability measures how likely an event is to occur.
P(A) = Number of favourable outcomes / Total possible outcomes

Rules:
- 0 ≤ P(A) ≤ 1
- P(impossible event) = 0
- P(certain event) = 1
- P(A) + P(not A) = 1

### Types of Events

**Independent events** — outcome of one does not affect the other
P(A and B) = P(A) × P(B)
- Example: flipping a coin twice — P(H and H) = 0.5 × 0.5 = 0.25

**Mutually exclusive events** — cannot both occur at the same time
P(A or B) = P(A) + P(B)
- Example: rolling a 3 or a 5 on a die = 1/6 + 1/6 = 2/6

**General Addition Rule:**
P(A or B) = P(A) + P(B) - P(A and B)

**Conditional Probability:**
P(A|B) = P(A and B) / P(B)
The probability of A given that B has already occurred.

### Distributions

**Binomial Distribution**
Used when: fixed number of trials (n), each trial has two outcomes (success/failure), probability of success (p) is constant, trials are independent.

P(X = k) = C(n,k) × pᵏ × (1-p)ⁿ⁻ᵏ

Mean = np, Variance = np(1-p)

Example: Probability of exactly 3 heads in 5 coin flips:
P(X=3) = C(5,3) × (0.5)³ × (0.5)² = 10 × 0.125 × 0.25 = 0.3125

**Normal Distribution**
Bell-shaped, symmetric distribution. Described by mean (μ) and standard deviation (σ).

The **68-95-99.7 Rule:**
- 68% of data falls within 1σ of the mean
- 95% of data falls within 2σ of the mean
- 99.7% of data falls within 3σ of the mean

**Standard Normal Distribution (Z-distribution):**
Z = (X - μ) / σ
Converts any normal distribution to one with mean 0 and SD 1.
Z-scores tell you how many standard deviations a value is from the mean.

## Correlation and Regression

### Correlation
Measures the strength and direction of a linear relationship between two variables.

**Pearson correlation coefficient (r):**
- r = 1: perfect positive correlation
- r = -1: perfect negative correlation
- r = 0: no linear correlation
- |r| > 0.7: strong; 0.4-0.7: moderate; < 0.4: weak

**Important:** Correlation does not imply causation.

### Linear Regression
Finds the best-fit line through data points.
Line equation: ŷ = a + bx

Where:
- b = r × (sy/sx) — slope
- a = ȳ - bx̄ — y-intercept
- x̄, ȳ are means; sx, sy are standard deviations

The line minimises the sum of squared residuals (differences between actual and predicted values).

## Hypothesis Testing

### The Process
1. State null hypothesis H₀ (no effect) and alternative hypothesis H₁
2. Choose significance level α (usually 0.05)
3. Collect data and calculate test statistic
4. Find p-value: probability of observing results at least this extreme if H₀ is true
5. Decision: if p < α, reject H₀; otherwise fail to reject H₀

### p-value
- Small p-value (< 0.05): strong evidence against H₀
- Large p-value: insufficient evidence to reject H₀
- p-value is NOT the probability that H₀ is true

### Type I and Type II Errors
- **Type I error (false positive)** — rejecting H₀ when it is actually true. Probability = α
- **Type II error (false negative)** — failing to reject H₀ when it is actually false. Probability = β
