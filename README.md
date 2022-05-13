Final project
Shelby, Imani, Maitreyi, Hannah
5/13/2022

[Github Pages](https://github.com/hill-hannah/final_project_hh_is_sl_mn.git)

The libraries loaded in include:
library(tidyverse)
library(lubridate)
library(tidymodels)
library(rsample)
library(parsnip)
library(recipes)
library(workflows)
library(tune)
library(yardstick)
library(rpart)
library(themis)
library(rpart.plot)
library(randomForest)
library(glmnet)
library(ranger)
library(dplyr)
library(factoextra)
library(broom)
library(lubridate)
library(dplyr)
library(anytime)
library(tidytext)
library(igraph)
library(ggraph)
library(rpart)

First, we carried out exploratory data analysis. We used geospatial analysis to understand trends over different populations in California. This helped us understand how people in different counties availed of WIC and SNAP services. 

Data cleaning: 
Cleaned all names with janitor package. We removed all the NAs. Columns were mutated to be numeric instead of character vectors. We removed commas and dollar signs in the columnns. 

Geospatial Analysis: 
*imani

Unsupervised Machine Learning:
We then moved on to supervised and unsupervised machine learning. Our models helped inform our policy questions, and provided several insights as to store locations in counties in California, and stores that were sources of WIC and SNAP.
Unsupervised machine learning: 
We used text analysis to understand the types of stores that provided these services to the people of California. To break this down further, we then compared the most common store locations in the top 6 urban counties, the top 6 rural counties, and the smallest 6 rural counties. 
  a. We ran a text analysis that gave us a word jumble graph as to the major stores in California. This helped us see how often words are used, and how they are connected with one another. We used ggraphs and igraphs to run these facet wraps.
  b. Once this was done, we created a model that told us the 15 most common store locations across important counties. This helps us understand how people get access to these stores, and the types of stores that exist in rural areas versus the types of stores that exist in urban areas. 
  
Supervised Machine Learning:
Cluster Analysis: 

Regression Models:
We used a linear regression model to predict the number of vouchers redeemed, based on county, date, and number of families in California. 
We used cross-variation within this regression, and created 10 folds to verify the model on. The final best rmse value told us the lasso coefficient to be used for the best possible prediction regression, which we then ran on the training data.

