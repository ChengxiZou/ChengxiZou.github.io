ST558 RandomForestBlogPost
================
Chengxi Zou
2022-07-10

# What method did you find most interesting? Write a little about the method, fit the model on some data, and provide any relevant output.

I think the random forest method is very inspiring.

Generally, the random forest method is better than bagging. If we care
mostly about prediction rather than interpretation, we could average
across many fitted trees, decreases variance over an individual tree
fit. We could create multiple trees and average results. The difference
is that we don’t use all predictors, we use a random subset of
predictors for each fit.

    ## # A tibble: 6 × 10
    ##   carat cut       color clarity depth table price     x     y     z
    ##   <dbl> <ord>     <ord> <ord>   <dbl> <dbl> <int> <dbl> <dbl> <dbl>
    ## 1  0.23 Ideal     E     SI2      61.5    55   326  3.95  3.98  2.43
    ## 2  0.21 Premium   E     SI1      59.8    61   326  3.89  3.84  2.31
    ## 3  0.23 Good      E     VS1      56.9    65   327  4.05  4.07  2.31
    ## 4  0.29 Premium   I     VS2      62.4    58   334  4.2   4.23  2.63
    ## 5  0.31 Good      J     SI2      63.3    58   335  4.34  4.35  2.75
    ## 6  0.24 Very Good J     VVS2     62.8    57   336  3.94  3.96  2.48

    ## 
    ## Call:
    ##  randomForest(formula = price ~ ., data = diamondsTrain, mtry = ncol(diamondsTrain)/3,      ntree = 200, importance = TRUE) 
    ##                Type of random forest: regression
    ##                      Number of trees: 200
    ## No. of variables tried at each split: 3
    ## 
    ##           Mean of squared residuals: 299206.1
    ##                     % Var explained: 98.1

    ## [1] 554.6379
