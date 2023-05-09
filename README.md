# HomeWork
Code Task for Data Analytic position
This dataset you received contains information on over 800+ fashion products. The data includes fields such as product ID, identifier , selling_price,  original_price, currency, availability, color, category, breadcrumbs, country,language, average_rating,reviews_count.

##### Task 1: Please analyze the data in order to find which colors are the most popular among different genders and age groups, in the end please create a dashboard to show your results.

##### Task 2: Please analyze the correlation between ratings and reviews to determine which factors are most important to customers, in the end please create a dashboard to show your results.

##### Task 3: Please create a modell to predict which combinatin of selling_price,color,category,breadcrumbs could be most popular products for next year?

During examining the data, it can be seen that the data is not balanced in terms of the number of products by color, there are also missing data, and it is necessary to distinguish product groups by gender and age.
There is very little data on some product colors, some original prices are missing.

It is not possible to delete a lot of the data, as the amount of data is not so large, and further research may suffer greatly.

In this connection, we can use the approach of searching for similar colors - finding the Euclidean distance between rgb vectors - to combine less popular colors with more popular ones.

The KNN filling approach was used to fill in the missing data in the original price

After that, we can examine the data using ANOVA for the dependence of product popularity on gender and age.

The dependence of the number of reviews on the rating of the product was also checked. Dependence is not observed, perhaps the number of reviews does not entail an increase in the rating.

To predict the popularity of a product based on its price and color and category, you can use linear regression. And also try different non-linear approaches.

As you can see, the results did not show high accuracy. I would settle for linear regression, but to improve accuracy, an increase in the number of observed data is needed (for better balancing by colors and rating)

##### The organised solution is in the Siemens_homework.ipynb

##### Data file is Fashion Retail.csv

##### In the file requirements.txt there are requirements for running the code

##### File AI_homework_explanation.ipynb, AI_homework_explanation.html and AI_homework_explanation.pdf - have all code with explanations and logical reasoning



