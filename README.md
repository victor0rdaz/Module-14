# Machine Learning Trading Bot
Instructions

The steps for this Challenge are divided into the following sections:
Establish a Baseline Performance
Tune the Baseline Trading Algorithm
Evaluate a New Machine Learning Classifier
Create an Evaluation Report
Establish a Baseline Performance

In this section, you’ll run the provided starter code to establish a baseline performance for the trading algorithm. To do so, complete the following steps.
NOTE
The provided CSV file contains open, high, low, close, and volume (OHLCV) data for a Morgan Stanley Capital International (MSCI)–based emerging markets exchange-traded fund (ETF) that iShares Links to an external site. issued. Investments in emerging markets make up an important aspect of a well-diversified investment portfolio. That’s because the included equities have potentially higher long-term returns, even though they carry more risk.
Open the provided Jupyter notebook, restart the kernel, and then run the cells that correspond with the following steps:
Import the OHLCV dataset into a Pandas DataFrame.
Generate trading signals by using short- and long-window SMA values.
Split the data into training and testing datasets.
Use the SVC classifier model from the SKLearn support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.
Review the classification report that’s associated with the SVC model predictions.
Create a predictions DataFrame that contains “Predicted”, “Actual Returns”, and “Strategy Returns” columns.
Create a cumulative return plot that shows the actual returns vs. the strategy returns. Save a PNG image of this plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm.
Write your conclusions about the performance of the baseline trading algorithm in the README.md file that’s associated with your GitHub repository. Support your findings by using the PNG image that you saved in the previous step.
Tune the Baseline Trading Algorithm

In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. (You’ll choose the best by comparing the cumulative products of the strategy returns.) To do so, complete the following steps:
Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing the training window?
HINT
Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?
Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file.
Evaluate a New Machine Learning Classifier

In this section, you’ll use the original parameters that the starter code provided. But, you’ll apply them to the performance of a second machine learning model. To do so, complete the following steps:
Import a new classifier, such as AdaBoost, DecisionTreeClassifier, or LogisticRegression. (For the full list of classifiers, refer to the Supervised learning page Links to an external site. in the scikit-learn documentation.)
Using the original training data as the baseline model, fit another model with the new classifier.
Backtest the new model to evaluate its performance. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns for this updated trading algorithm, and write your conclusions in your README.md file. Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?
Create an Evaluation Report

In the previous sections, you updated your README.md file with your conclusions. To finish this section, add a summary evaluation report at the end of the README.md file. For this report, express your final conclusions and analysis. Support your findings by using the PNG images that you created.



## Project Conclusions

[
<img width="877" alt="Screen Shot 2021-06-27 at 10 16 31 PM" src="https://user-images.githubusercontent.com/80833988/123583918-56207a00-d795-11eb-9ead-509bd9926d20.png">
](url)

[
<img width="843" alt="Screen Shot 2021-06-27 at 10 02 05 PM" src="https://user-images.githubusercontent.com/80833988/123582798-51f35d00-d793-11eb-9866-c3ee04a6a828.png">
](url)

Its very complicated to make a decision on which strategy is best to use. However in this case our first model is predicting an actual trend is better. We see that first model project results are closer to the actual ones, but the classification report shows that the first one has slightly better quality on the prediction side . Very likely that first model  simply follows the first one, in order to make a decision I would prefer to run one more version of the model to make sure my prediction is correct.




Sources- ChatGpt, Xpert learning 