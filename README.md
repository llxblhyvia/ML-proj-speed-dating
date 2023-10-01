# ML-proj-speed-dating
>[Course project for 2020 Fall < Machine Learning >.]Predicting dating matches using semi-supervised learning on DSW platform of Ali Cloud.
## Data
The data in [data](data) is for preview and actually accessed with:
```
!wget https://pai-public-data.oss-cn-beijing.aliyuncs.com/speed_dating/Speed%20Dating%20Data%20Key.doc
!wget https://pai-public-data.oss-cn-beijing.aliyuncs.com/speed_dating/Speed%20Dating%20Data.csv
```
### Data Description
Detailed data introduction is attached in the [Speed Dating Data Key](data/Speed_Dating_Data_Key.doc)file, here we introduce some more important data items, including `participant ID`, `number of events participated`, `gender`, `age`, `SAT Score`, `race`, `department`, `school`, `attr`--attractive attractiveness index, `sinc`--sincere true Honesty index, `intel`--intelligent smart index, `fun`--interesting index, `amb`--ambitious Ambition index, `shar`--has shared interests/hobbies--the degree of having the same interests and hobbies, etc. There are 195 features, 8277 strips of labeled data in total.
## Task Description
For supervised learning, five models are used - Random Forest, Logistic Regression, BaggingClassifier, AdaBoost, SVM; semi-supervised learning is done on the first four of the above five models for comparison with supervised learning. SMOTE is used to solve the data imbalance problem. 
