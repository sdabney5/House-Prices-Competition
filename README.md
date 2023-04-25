# House-Prices-Competition
Kaggle Competition. House Prices - Advanced Regression Techniques


## Overview:  
The challenge for this project is to build a ML model to predict Real Estate Sales Prices. It was built for two purposes:

- First, this is my Capstone Project for certification through Elite Data Science's Machine Learning course. As such, it should demonstrat 'sufficient proficiency in applied machine learning' as verified by Elite Data Science  
  
- Second, it was built to make a submission to the Kaggle Competition 'House Prices- Advanced Regression Techniques'. I used 'The Ames Housing dataset' from Dean De Cock to train the model and submitted predictions for a Test Set through Kaggle.



## Conclusion and Insights:
### At a glance:
- My model's predictions placed 1239/4357 !

- My model's RMSE (Root Mean Squared Error) was 0.13255.  
___  
  
### Important Notes:  
**Original work**    
There are many examples and tutorials on Youtube that walk-through this competition. My goal was to build a model on my own, using only the knowledge I gained from my ML course. I did allow myself to refer to previous work I did in the course, as well as relevent video lessons.

(N.B. I did end up borrowing code in two places. First, the only code I copied for my first submission was in the final code block, which concatenated my predictions with the submission ID list. This did not impact my model at all. It was copied because this was my first Kaggle submission, and I was not sure about the correct submission format. Second, after submiting the first predictions, I explored further tweaks to my model such as removing additional outliers. The idea for the outlier detection loop was taken from somewhere else. However, this ended up hurting my model.)

**Cleaning and Augmenting Data**  
A summary of my approach to cleaning and augmenting the data is provided after each section. The long list of outliers was added after the initial submission in hopes that it would improve my model. It did not, so these code blocks were commented out.

**Approach to Test Data**  
I did view many other video tutorials on this competition to compare my approach with that of others. Most (all?) began by combining test and train data and then performing the data cleaning and alterations on both at once. One benefit of this approach is that both with have the same final shape. In my approach, I did not touch the test data until my model was built, since this seems to be best practice.

This did lead to some problems (see code comments). The test data and the train data had some different classes in their categorical variables. So when I created dummy variables, the train and test data had different shapes. My solution was to drop these observations. A better approach may have been to loop through the categorical variables, and replace any novel classes with "other". This would ensure that the cleaning and augmenting functions could work for any new unseen data.

**Adjustments made and resubmitted**   
I resubmitted many different versions of the model: with different hyperparameters, with different potential outliers removed, etc. The original model performed the best.

**Conclusion**   
Overall, I set out to build a "good" model. Its performance surpassed my expectations

