# Financial-Markets-Regression-Analysis
My role in this group project was to perform regression analysis on quarterly financial data to predict a company's market capitalization. I used R to develop ordinary least squares (OLS), stepwise, ridge, lasso, relaxed lasso, and elastic net regression models. I first used stepwise and OLS regression to develop a model and examine its residual plots. The plot displaying the residuals against the predicted values indicated multiplicative errors. I, therefore, took the natural log transformation of the dependent variable. The resulting model's R2 was significantly, negatively impacted. After examining scatter plots between the log transformation of market capitalization and the independent variables, I discovered the independent variables also had to be transformed to produce a linear relationship. Using the log transformation of both the dependent and independent variables, I developed models using all the regression techniques mentioned to strike a balance between R2 and producing a parsimonious model. All the models produced similar results, with an R2 of around .80. Since OLS is easiest to explain, had similar residual plots, and the highest R2 of all the models, it was the best model developed.

The data set is from Quandl & Sharadar containing historical financial information for public firms. The data consisted of 3 tables:  
  1) The core fundamentals data, which included 20 years of financial statement history on more than 14,000 companies (111 variables), 
  2) The Daily table, which contained daily variables like price, volume, and enterprise values (8 variables), and 
  3) The Tickers table which included metadata like firm size, industry, and sector (34 variables). 

Unfortunately, I do not have permission to share the dataset used.

The attached R Markdown file includes analysis not described above, for example correspondence analysis, that I tested but did not pursue further to include in the final project submission. 

Libraries included in the file include: Amelia (1.7.6), ca (0.71.1), car (3.0.10), caret (6.0.88),  corrplot (0.84), dplyr (1.0.2), glmnet (4.1), leaps (3.1), psych (2.1.3), stringr (1.4.0),  tidyr (1.1.2), vcd (1.4.8)
