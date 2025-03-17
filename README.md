# Sales-Forecasting-Across-Multiple-Retail-Stores
****Task 1 - Exploration of customer purchasing behaviour** **-- In this task, we seek to explore the behaviour of customers in the various stores. Our
goal is to check how some measures such as promos and opening of new stores affe
purchasing behavior.
To achieve this goal, we need to first clean the data. The data cleaning process will be
involve building pipelines to detect and handle outlier and missing data. This is
particularly important because we don’t want to skew our analysis.
Visualizing various features and interactions is necessary for clearly communicating our
findings. It is a powerful tool in the data science toolbox. Communicate the find
below via the necessary plots.
We can use the following questions as a guide during your analysis. It is important to
come up with more questions to explore. This is part of our expectation for an excellent
analysis.
● Check for distribution in both training and test sets - are the promotions
distributed similarly between these two groups?
● Check & compare sales behavior before, during and after holidays
● Find out any seasonal (Christmas, Easter etc) purchase behaviours,
● What can you say about the correlation between sales and number of
customers?
● How does promo affect sales? Are the promos attracting more customers? H
does it affect already existing customer
● Could the promos be deployed in more effective ways? Which stores shou
promos be deployed in?
● Trends of customer behavior during store open and closing times
● Which stores are opened on all weekdays? How does that affect their sales 
weekends?
● Check how the assortment type affects sal
● How does the distance to the next competitor affect sales? What if the store a
its competitors all happen to be in city centres, does the distance matter in that
case?
● How does the opening or reopening of new competitors affect stores? Check f
stores with NA as competitor distance but later on has values for competitor
distance
Deliver your exploratory analysis notebook - make sure you answer all the questions
asked in task 1 using the appropriate plots or summary tables and give useful insights. A
3 - 5 slides presentation is enough for interim submission.

****Task 2 - Prediction of store sales** --**Prediction of sales is the central task in this challenge. we want to predict daily sales in
various stores up to 6 weeks ahead of time. This will help the company plan ahead of
time.
The following steps outline the various sub tasks needed to effectively do thi
2.1 Preprocessing
It is important to process the data into a format where it can be fed to a machine learning
model. This typically means converting all non-numeric columns to numeric, handling
NaN values and generating new features from already existing features.
In our case, you have a few datetime columns to preprocess. you can extract the
following from them:
- weekdays
- weekends
- number of days to holidays
- Number of days after holiday
- Beginning of month, mid month and ending of month
- (think of more features to extract), extra marks for it
As a final thing, you have to scale the data. This helps with predictions especially wh
using machine learning algorithms that use Euclidean distances. you can use the
standard scaler in sklearn for this.
**2.2 Building models with sklearn pipelines**
At this point, all our features are numeric. Since our problem is a regression problem, you
can narrow down the list of algorithms you can use for modelling.
A reasonable starting point will be to use any of the tree based algorithms. Random
forests Regressor will make for a good start
2.6 Building model with deep learning
Deep Learning techniques can be used to predict various outcomes including but not
limited to future sales. Your task is to create a deep learning model of the Long Short
Term Memory which is a type of Recurrent Neural Network .
**Task 3 - Serving predictions on a web interface**
Use one of the platforms of your choice (Flask, Streamlit, pure javascript, etc.) to design[Uploading Task 3 - Serving predictions on a web interface.ipynb…]()
,
and build a backend to make inference using your trained model and input parameters
collected through a frontend interface.
Your dashboard should provide an easy way for a user (in this case managers of the
stores) to enter required input parameters, and output the predicted sales amount and
customer numbers.

