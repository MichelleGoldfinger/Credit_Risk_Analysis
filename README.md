# Credit_Risk_Analysis
## Overview of the analysis: Explain the purpose of this analysis. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. My boss, asked me to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. 

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results. 


### Deliverable 1 

#### RandomOverSampler:
* Accuracy: 0.628723142809948
* Precision: High- Risk: .01, Low-Risk: 1.00
* Recall Scores: High-Risk: .62, Low-Risk: .64

<img width="743" alt="Screen Shot 2021-04-25 at 8 03 31 AM" src="https://user-images.githubusercontent.com/75905911/115992671-d90e3400-a59c-11eb-92b7-0ba1d8260f7e.png">

#### SMOTE:
* Accuracy: .60
* Precision: High-Risk: .01, Low-Risk: 1.00
* Recall: High-Risk: .52, Low-Risk: .69

<img width="737" alt="Screen Shot 2021-04-25 at 8 04 41 AM" src="https://user-images.githubusercontent.com/75905911/115992685-ed523100-a59c-11eb-9c49-c5d8637403b4.png">

#### ClusterCentriods
* Accuracy: .51
* Precision: High-Risk: .01,Low-Risk: 1.00
* Recall: High-Risk: .56, Low-Risk: .46

<img width="758" alt="Screen Shot 2021-04-25 at 8 05 14 AM" src="https://user-images.githubusercontent.com/75905911/115992693-00fd9780-a59d-11eb-8e36-81618fa605d7.png">


### Deliverable 2
#### SMOTEENN
* Accuracy: .64
* Precision: High_Risk: .01, Low_Risk: 1.00
* Recall: High_Risk: .7, Low_Risk: .58

<img width="729" alt="Screen Shot 2021-04-25 at 8 05 50 AM" src="https://user-images.githubusercontent.com/75905911/115992710-14a8fe00-a59d-11eb-9ee3-f78b2f9d86fc.png">

### Deliverable 3
#### BalancedRandomForestClassifier
* Accuracy: .79
* Precision: High-Risk: .03 , Low-Risk: 1.00
* Recall: High-Risk: .7 , Low-Risk: .87

<img width="745" alt="Screen Shot 2021-04-25 at 8 06 30 AM" src="https://user-images.githubusercontent.com/75905911/115992730-2be7eb80-a59d-11eb-83f9-c203dc77d3a6.png">

#### EasyEnsembleClassifier
* Accuracy: .93
* Precision: High-Risk: .9, Low-Risk: 1.00
* Recall: High-Risk: .92, Low-Risk: .94

<img width="747" alt="Screen Shot 2021-04-25 at 8 07 04 AM" src="https://user-images.githubusercontent.com/75905911/115992742-40c47f00-a59d-11eb-8044-1918f9e8255b.png">


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning. 
The accuracy scores for: RandomOverSampler is 62%, ClusterCentriods is 51%, SMOTE is 60%, SMOTEEN is 64%, BalancedRandomForestClassifier is 79% and EasyEnsembleClassifier is 93%. Therefore, the EasyEnsembleClassifier has the greatest accuracy the credit loan status.

The precision score for: RandomOverSampler is .01 for high-risk and for low-risk 1.00, ClusterCentriods is high-risk .01 and for low-risk 1.00, SMOTE is .01 for high-risk and for low-risk 1.00, SMOTEEN is .03 for high-risk and for low-risk 1.00, BalancedRandomForestClassifier is .03 for high-risk and for low-risk 1.00 and EasyEnsembleClassifier is .09 for high-risk and for low-risk 1.00. Therefore, RandomOverSampler, ClusterCentriods and SMOTE all have the highest precision in deciding credit risk.

The recall score for RandomOverSampler is High-Risk: .62, Low-Risk: .64. For SMOTE the recall score is High-Risk: .52, Low-Risk: .69. ClusterCentriods’ recall scores are High-Risk: .56, Low-Risk: .46. For SMOTEEN the recall score is  High_Risk: .7, Low_Risk: .58. Recall for  BalancedRandomForestClassifier is High-Risk: .7 , Low-Risk: .87 and lastly the recall for EasyEnsembleClassifier is High-Risk: .92, Low-Risk: .94. Thus, EasyEnsembleClassifier is the most sensitive at predicting credit risk with 92% of predictions for high-risk and 94% correct predictions for low-risk.

I would recommend the EasyEnsembleClassifier for the model to use for correctly predicting high and low credit risk because its accuracy score is 93%, its precision is .09 for high-risk and 1.00 for low-risk. Lastly, EasyEnsembleClassifier’s recall is 92% of predictions for high-risk and 94% correct predictions for low-risk.
