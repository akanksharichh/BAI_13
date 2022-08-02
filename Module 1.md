# BAI_13

HPPO- Highest Paid Person's Opinion
Monty Hall Problem

What is Machine Learning?
	• Task
	• Performance
	• Learning

Case Study: Hurricanes increase pastry sales 7 times. Why?

Case Study: Target's pregnancy prediction problem:  Classification problem

Why are targets focusing on this population?
	• Price insensitive customers
	• Market size
How?
	• 25 different items when analysed together to predict pregnancy and generate pregnancy prediction score
	• Basket products together - one normal and one pregnancy related

Case Study: Big Basket forgot products feature
	• To prevent customer buying from other offline stores 
	• To reduce logistics if 2 orders need to be delivered

How to choose right models?
	• Speed
	• Cost
	• Scalability
	• Accuracy

Case Study: shorter Skirt length means economy is doing better
	• Maintenance costs are high for shorter skirts and hence customers have high disposable income and affordability

Case Study: Cholera spread: Jon Snow Diagram | air borne disease to water borne disease

Components of analytics:

	1. Descriptive: Describe data using stats/visualization (What happened)
	2. Predictive: Predict future events (What will happen)
	3. Prescriptive: Optimization and decision making ( What action to take)

Data
	• Good
	• Bad
	• Ugly

Steps in an analytics projects

	Feature Extraction | Feature engineering (developing new variables based on domain knowledge) | Model and Feature Selection | Model Deployment
	
AI Strategy and Execution Strategy
One way of feature engineering is Binning

Types of ML algorithms:

	• Supervised Learning : If algorithm has both input and output variables. 
	We try to minimize Loss function/Cost function. One definition: Loss function is nothing but difference between predicted value and actual value. y^ - Hat means that it is an estimated or predicted value. Loss function = Summation of (y-y^)^2
	Training the model using actual values of output variable is called supervising the model. Techniques like regression, logistic regression, decision trees, random forest and boosting etc are supervised learning algorithms
	• Unsupervised Learning: Data consists of features but no outcome variable. For e,g. clustering, factoring, principal component analysis, random fern
	• Reinforcement Learning: Sequence based learning to maximise return in a random environment with uncertainty of return. For example investments made by a person, WhatsApp text suggestions, spell check 
	Exploration (when uncertain) vs Exploitation (when certain based on learning)
	Models- Markov Decision Process, Dynamic Programming, Bandit Models
	• Evolutionary: Algorithms that imitate natural evolution to solve problems. For example: Travelling salesman problem solved by bee
	• Self-learning: Algorithms that are programmed to learn by itself. For example- chatbot where feedback (was it helpful) is used to solve the problem

Descriptive Analytics
	• Data Summarization
	• Descriptive Statistics
	• Data Visualization

Population vs Sample. Whenever a measure is calculated from population, it is called parameter. When measure is calculated from a sample, it is called a Statistic.

Types of Data:
	• Nominal - Names or labels for example - Marital Status converted into 0/1. Arithmetic operations cannot be done
	• Ordinal Scale- Feedback - 1-5. Arithmetic operations cannot be done. 4 is not twice as good as 2 but there is an order 
	• Interval - Temperature, IQ (Value of zero is assigned arbitrarily). Plus/Minus work but multiplication and division don’t work
	• Ratio - Ratios make sense
	• Discrete - Countable
	• Continuous - Cannot count, For e.g. time, volume
	• Time Series - Weekly demand for a product
	• Cross Sectional data - Many variables at same point in time (data is not captured over time)
	• Panel Data - Many variables with respective time stamps
	• Unstructured Data - Audios, Videos (not tabular)
	• Structured Data - Tabular form
	
Measures of Central Tendency:

	• Mean: Sensitive to outliers. Use only for interval scale and ratio scale
	Summation of (xi-mean) = 0. Hence square is required in error formulae.
	• Median: Divides population into equal parts. 50% values to the left. Arrange in desc/asc order, middle point for odd number of records or avg of middle 2 for even records. Actual values are not being used. Less sensitive to the outliers. Only used for interval scale and ratio scale
	• Mode: Number with highest frequency. Used for interval, ratio, nominal and ordinal scales

When to use median vs mean?
Depends on the problem. Also, in most cases, mean, median mode are not sufficient. Entire distribution needs to be taken into account

Measures of Variation:
Min/Max. Most analysis try to explain this variability. Why is one value = max vs other = min

	• Range = Max- Min
	• Variance
		○ Population Variance = ((Xi - u)^2 for all N records)/N
		○ Sample Variance = ((Xi - xbar)^2 for all N records)/(N-1)
		
		U = Mean of pop
		Xbar = Mean of sample
		
		○ Downward Bias: Contribution of each record to population variance gets underestimated when same calculation is done for a sample variance. This is called a downward bias. To compensate this the denominator is N-1
		If sample mean and pop mean is same, there would be no downward bias but this is just in theory. It is not practically possible for the sample and pop to have exact same mean
		○ Degrees of freedom: N-1. Flexibility the data has + restriction. Every time we calculate a measure from the data, we lose a degree of freedom.
		Data has n records. From n records we estimate k parameters. Degrees of freedom = (n-k)
	• Standard Deviation: Square root of variance
		○ Population std Dev
		○ Sample Std Dev

Measures of Shape:

Normal distribution: Bell shaped curve, symmetric, 50% points on both sides of the mean

	• Skewness: Shape of the tail
		○ Compares tail with the tail of the normal distribution
		○ Left skew: negative (Long left tail) | Right skew: positive (Long right tail) | Zero: Normal distribution
		○ In Excel, use function Skew
		○ Example of a right skewed chart below-
	
	• 
	• Kurtosis: 
		○ Compares height with the height of the normal distribution
		○ High kurtosis means the values are concentrated around mean
		○ In Excel, use function Kurt
		○ Kurtosis of a normal distribution is 3
		○ >3: Goes higher than the normal distribution. Closer to the mean value
		○ <3: Below the normal distribution

Application: Returns from a bank. Avg 10 but left skewed- Chances of losing money. Right skewed: Chances of making more money
Kurtosis high: Variation is less. Concentrated around the mean

Chapter 1/2 for above things and 3 for next
	

Questions:

	1. Rather than taking square of errors why not take MOD?
	It will make calculations very complex.
	
	For a good model, bias should be low (not too high as it would make the model very simple and underfit the model) and variance should be low (not too complex as it might overfit)
	
![image](https://user-images.githubusercontent.com/109798287/182356430-8a1e8e6f-c262-494e-886e-e1f2a07f9148.png)
