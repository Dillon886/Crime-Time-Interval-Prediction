# Crime-Time-Interval-Prediction
## Objective
Predict the time interval of the crime depending on the location of the crime (district, precinct, neighborhood) and the type of crime.
## Summary of the models built
Three classification models were built using 3 different classification algorithms and then ensembled to provide the best possible result from the three models. Decision tree classifier built a better classification model and that model is a better fit for predicting the time interval for the occurrence of a crime. The model gave an accuracy of 61% with 39% misclassification. Models built using random forest algorithm and knn algorithm gave an accuracy of 60% and 59% respectively. An ensemble classifier is formed by a set of basic classifiers, whose individual outcomes are combined by voting fashion, to give a final determination in classifying a query sample. The current ensemble classifier consists of three basic individual classifiers. The ensemble model gave an accuracy of a decent 61% with precision score of 0.64 and recall score of 0.87.
 
## Aim
Crimes are a common social problem affecting the quality of life and the economic growth of a society. With the increase of crimes, law enforcement agencies are continuing to demand advanced geographic information systems and new data mining approaches to improve crime analytics and better protect their communities. By providing a data mining approach to determine the most criminal hotspots and find the type, location and time of committed crimes, we hope to raise people’s awareness regarding the dangerous locations in certain time periods. Therefore, our proposed solution can potentially help people stay away from the locations at a certain time of the day along with saving lives. In addition, having this kind of knowledge would help people to improve their living place choices. On the other hand, police forces can use this solution to increase the level of crime prediction and prevention. Moreover, this would be useful for police resources allocation during a particular time of the day. 
## Why this topic was chosen?
Crime rate has seen a drastic increase in the past couple of years making it hard for law enforcement to keep track of them. But with the advancements in statistics and technology we can now look for crime patterns so that we can be ready for any future incidents. There is a deep relation between crime type and time of occurrence. Certain crime types happen only during the night while others don’t really have a fixed time interval. Some crime types take time to get reported from its first occurrence while others are reported immediately. Since we know that crime and time has a unique connection with each other we can look for ways to exploit this and fight crime before it even occurs. 
## DATASET DESCRIPTION
This dataset includes criminal offenses in the City and County of Denver for the previous five calendar years plus the current year to date. The data is based on the National Incident Based Reporting System (NIBRS) which includes all victims of person crimes and all crimes within an incident. The Denver Crime dataset consists of 466840 crime as well as accidents records with 19 attributes, for 5 years period from 2015 to 2020, in Denver Colorado state US. Out of 19 attributes, there were 3 attributes describing the date and time of the crime/accident, geographical location of the crime, the rest of the attributes divisions and sub divisions of the type of crime. The neighborhood attribute has 78 unique values and the crime category ID attribute was a group of 8 different types of crime.
| Fields                 | Description                                                                              | 
| ---------------------- |:-----------------------------------------------------------------------------------------| 
| INCIDENT_ID            | Unique numeric incident ID that starts with the year of the event that has occurred.     | 
| OFFENSE_ID             | Unique numeric offense ID that starts with the year of the crime that has occurred.      |   
| OFFENSE_CODE           | Unique code for the offense (values range from  902 to 7399)                             |
| OFFENSE_CODE_EXTENSION | Extension of the unique code (values ranges from 0 to 5)                                 |
| OFFENSE_TYPE_ID        | Exact crime that has occurred(values range from 1 to 197)                                |
| OFFENSE_CATEGORY_ID    | It takes category or type of crime (15 categories)                                       |
| FIRST_OCCURRENCE_DATE  | Contains the date and time of the crime that has occurred                                |
| LAST_OCCURRENCE_DATE   | Contains the date and time of the crime when it ended                                    |
| REPORTED_DATE          | The day the incident was reported (contains date and time)                               |
| GEO_X                  | Geographical location in x axis                                                          |
| GEO_Y                  | Geographical location in y axis                                                          |
| INCIDENT_ADDRESS       | Address of the incident that has occurred (block and street)                             |
| GEO_LON                | Longitudinal location of the incident                                                    |
| GEO_LAT                | Latitudinal location of the incident                                                     |
| DISTRICT_ID            | District of area where the crime has occurred(Ranges from 1 to 7)                        |
| PRECINCT_ID            | Precint code of an area of city or town (Ranges from 111 to 759)                         |
| NEIGHBORHOOD_ID        | Contains the neighborhood where the crime had occurred(78 neighborhoods)                 |
| IS_CRIME               | Is_Crime indicates whether the instance belongs to a crime or accident (0 or 1).         |
| IS_TRAFFIC             | Is_Traffic indicates whether the instance belongs to a crime or accident (0 or 1).       |
## Exploratary Data Analysis
Exploratary Data Analysis done using tableau to find insights and pattern in the data. They are found the folder named EDA on Denver Crime Dataset
## Libraries used
* numpy
* pandas
* matplotlib
* seaborn
* sklearn
## References
* https://towardsdatascience.com/ensemble-methods-bagging-boosting-and-stacking-c9214a10a205
* https://saravananthirumuruganathan.wordpress.com/2010/05/17/a-detailed-introduction-to-k-nearest-neighbor-knn-algorithm/
* https://towardsdatascience.com/all-the-annoying-assumptions-31b55df246c3
* http://bccvl.org.au/algorithms-exposed-random-forest/
* https://www.kdnuggets.com/2020/01/decision-tree-algorithm-explained.html
* https://www.kdnuggets.com/2017/10/random-forests-explained.html
* https://medium.com/@Synced/how-random-forest-algorithm-works-in-machine-learning-3c0fe15b6674
* https://towardsdatascience.com/understanding-random-forest-58381e0602d2
* https://blog.usejournal.com/a-quick-introduction-to-k-nearest-neighbors-algorithm-62214cea29c7
* https://www.geeksforgeeks.org/decision-tree-implementation-python/?ref=rp
* https://datascience.stackexchange.com/questions/12909/definition-of-a-model-in-machine-learning
* https://towardsdatascience.com/chi-square-test-for-feature-selection-in-machine-learning-206b1f0b8223
* http://www.learn4master.com/machine-learning/chi-square-test-for-feature-selection
* https://machinelearningmastery.com/feature-selection-with-categorical-data/
* https://www.geeksforgeeks.org/ml-chi-square-test-for-feature-selection/
* https://machinelearningmastery.com/imbalanced-classification-with-python/
* https://arxiv.org/ftp/arxiv/papers/1508/1508.02050.pdf
* https://towardsdatascience.com/a-starter-pack-to-exploratory-data-analysis-with-python-pandas-seaborn-and-scikit-learn-a77889485baf
* https://towardsdatascience.com/understanding-feature-engineering-part-2-categorical-data-f54324193e63
* https://www.statisticshowto.com/univariate/
* https://towardsdatascience.com/exploring-univariate-data-e7e2dc8fde80
* https://towardsdatascience.com/exploring-univariate-data-e7e2dc8fde80?gi=82077ff63536
