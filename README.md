# Drinking Water Potability: A Data Mining Case Study

## Abstract

Access to safe and potable drinking water is a fundamental human right, yet millions globally struggle with contaminated or unavailable sources. This case study delves into the complex issue of drinking water potability , examining the multifaceted challenges and potential solutions analyzing quality. Highlight the prevalence of contamination, resource scarcity, and factors contributing to non-potability. Data mining tasks in terms of clustering and prediction modeling are applied which includes the determination of potability of drinking water considering the attributes defined for taste and palatability, health risks, and equipment wear and tear.


## I. Dataset Description

Safe and healthy drinking water is the basic need for the maintenance of a healthy lifestyle. Access to safe drinking water being a fundamental right, millions are yet deprived of it. The key aspects of this case study involve the current reality, impact on health, and the resolution to maintain the supply of quality drinking water. The potability of drinking water is defined by various aspects. Unfortunately, there's no single "most affecting factor" for drinking water quality among the listed attributes as each plays a crucial role in different ways. This dataset is valuable for water quality assessment, water treatment planning, and ensuring the safety of drinking water supplies.

## II. Dataset Description

This dataset contains water quality measurements and assessments related to potability, which defines the suitability of water for human consumption. Each row in the dataset represents a water sample with specific attributes, and the “potability” column indicates whether the water is suitable for consumption or not.

## III. Data Mining Algorithms

For comparison purposes, which is the major objective of the paper, we have worked with six types of algorithms: Naïve Bayesian, K Neighbors, Support Vector Machine, Random Forest, Decision Tree Classifier, and Logistic Regression.

## IV. Data Preprocessing

### A. Data Cleaning
The data is retrieved from the Kaggle data repository, which was almost in the working form. But for better working with the data, it had to be worked with to ensure that it is in the standard quality before the model creation is initiated. The data retrieved was in the int64 format, which need not be made any changes.

### B. Data Transformation
A standard data analysis was done on the dataset to identify some patterns in the data and also present the data in tables based on attribute range and their frequencies.

### C. Outliers Evaluation
Boxplots are a standardized way of displaying the distribution of data based on a five-number summary including minimum, first quartile, median, third quartile, and maximum. This type of plot is used to easily detect outliers.

### D. Data Correlation
Each of the attributes is plotted against each of the attributes creating a pair plot which shows the data distribution graphed against those attributes. A pair plot allows us to see both the distribution of single variables and the relationship between multiple variables.

### E. Data-Set Split
The pre-processed dataset was split into two sections of varying sizes at different times for use as training and testing datasets across the different data mining classification algorithms for model creation and observation of which of the models performs best.

## V. Model

### A. Robust Scalar
Robust Scalar is used to scale features using statistics that are robust to the outliers. This removes the median and scales the data according to the quantile range.

### B. Data-Set Split
For this activity, the train_test_split method of sklearn was used, which split the data into a train to test ratio of 4:1.

### C. Model Pipelines
A pipeline is used to help automate machine learning workflows. They operate by enabling a sequence of data to be transformed and correlated together in a model that can be tested and evaluated to achieve an outcome, whether positive or negative. The pipeline includes a total of six algorithms which were to be passed through a single function to evaluate the performance of each of those algorithms.

### D. Score Machine Learning Algorithms
A function was created to fit and score machine learning algorithm models after scaling to fix the outliers. The resulted score of the method is presented where the Random Forest performs with the highest accuracy.

### E. Model Accuracy
The classified dataset result from the comparison between the six algorithms is shown. Random Forest achieved the highest overall score, followed by Naïve Bayes and then Logistic Regression, Decision Tree Classifier, K Neighbors, and finally Support Vector Machine.

## VI. Conclusion

The comparative analysis of the models used in this study shows that the accuracy gained by Random Forest was highest among the dataset. This indicates that for the categorical and numerical data, as worked with in this data, Random Forest provides with the best results among all the six algorithms compared in here. Then this is followed by Naïve Bayes and Logistic Regression with similar results. Then come Decision Tree Classifier and K Neighbors. The Support Vector Machine seems to work negatively here. Finally, from my analysis to this dataset I can conclude that the data is almost clean and there was few incorrect report the dropped them. I could not find a clear evidence that some features are redundant and can produce a biased solution.

