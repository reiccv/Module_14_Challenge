# Module 14 Challenge

# Machine Learning Trading Bot

In this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

# Table of Contents

* [Establish a Baseline Performance](#establish-a-Baseline-Performance)

* [Tune the Baseline Trading Algorithm](#tune-the-Baseline-Trading-Algorithm)

* [Evaluate a New Machine Learning Classifier](#evaluate-a-New-Machine-Learning-Classifier)

* [Create an Evaluation Report](#create-an-Evaluation-Report)


## Establish a Baseline Performance

1. Import the OHLCV dataset into a Pandas DataFrame.

2. Generate trading signals using short- and long-window SMA values. 

3. Split the data into training and testing datasets.

4. Use the `SVC` classifier model from SKLearn's support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.

5. Review the classification report associated with the `SVC` model predictions. 

6. Create a predictions DataFrame that contains columns for “Predicted” values, “Actual Returns”, and “Strategy Returns”.

7. Create a cumulative return plot that shows the actual returns vs. the strategy returns. 

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/1.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/2.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/3.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/4.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/5.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/6.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/7.PNG)


## Tune the Baseline Trading Algorithm

1. Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods.

> **Hint** To adjust the size of the training dataset, you can use a different `DateOffset` value&mdash;for example, six months. Be aware that changing the size of the training dataset also affects the size of the testing dataset.

2. Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. 

3. Choose the set of parameters that best improved the trading algorithm returns. 

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/8.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/9.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/10.PNG)



## Evaluate a New Machine Learning Classifier

1. Import a new classifier, such as `AdaBoost`, `DecisionTreeClassifier`, or `LogisticRegression`. (For the full list of classifiers, refer to the [Supervised learning page](https://scikit-learn.org/stable/supervised_learning.html) in the scikit-learn documentation.)

2. Using the original training data as the baseline model, fit another model with the new classifier.

3. Backtest the new model to evaluate its performance. 


![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/11.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/12.PNG)

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/13.PNG)


## Create an Evaluation Report

![](https://github.com/reiccv/Module_14_Challenge/blob/main/Resources/images/14.PNG)