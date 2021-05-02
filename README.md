![image](https://user-images.githubusercontent.com/56414953/112048508-deeba200-8b24-11eb-8cfa-9b61476acc04.png)
# Business Case
In this report, the following topics regarding covid-19 are covered:
  - The covid-19 pandemic test, case, recovery, death, and vaccination totals are put into a relational database and analyzed followed by a polynomial regression with lasso regularization model to determine the relationship between cases of and vaccination for the virus, and SARIMA models to determine the progression of cases and vaccinations.  
  - A logit model is used to determine the log odds relationship between government covid-19 regulations and the presence of cases of SARS-CoV-2, and an XGBoost model is used to determine the feature importance of government covid-19 regulations to cases of SARS-CoV-2, which are separated into three calsses: large, medium, and small amount of cases.  
  - NLP is used to analyze the words from a CNBC article about covid-19 for document importance.  This report uses K-means clustering to determine the document importance classes, and multinomial naive bayes to classify the words for document importance. 
  - SARS-CoV-2 symptoms, lifecycle, genetics, testing, and vaccines are explained followed by a CNN model that is used to determine whether SARS-CoV-2 is present in CT-scans, and a bidirectional RNN model that is used to predict the next nucleotide in the sequence of a SARS-CoV-2 genome.  
# Covid-19 General Information
A new type of coronavirus, SARS-CoV-2, started in December 2019 and has caused the COVID-19 global pandemic. SARS-CoV-2 originated in a Chinese city called Wuhan. Coronaviruses are common in animals, and scientists hypothesize that SARS-CoV-2 may have transferred to humans, zoonosis, through the Wuhan food market. SARS stands for severe acute respiratory syndrome. In 2003, there was an outbreak of SARS in China that spread to other countries and then ended in 2004. SARS-CoV-2 has spread faster than the 2003 SARS. SARS-CoV-2 is spread when an infected person coughs or sneezes droplets of saliva or mucus with the virus into the air. The respiratory droplets usually do not go further than a few feet, are airbourne for a few moments, and then land on a surface. SARS-CoV-2 has an incubation period of 2 to 14 days and the symptoms of the virus include cough, fever or chills, shortness of breath or difficulty breathing, muscle or body aches, sore throat, loss of taste or smell, diarrhea, headache, fatigue, nausea or vomiting, congestion or runny nose, and in rare cases the virus can lead to difficulty walking, confusion, bluish face or lips, coughing up blood, severe respiratory problems, kidney failure, high fever, or death.  
# Analytics 
Built a SQL database that holds two tables of Covid-19 totals for both countries and the United States, and conducted various queries.  
# Models
- Machine Learning:
  - Regression:  
    - The polynomial regression model with lasso regularization suggests that cases of and vaccinations for the virus are inversely related, and has a train r-squared of 71, and a train mse of 3, a cross validated mse of 4, a test r-squared of 100, and a test mse of .7.  
    - The SARIMA models suggest that, over the next month, vaccinations will trend upward by 83.3% and cases of the virus will trend upward by 12.8%. 
  - Classification: 
    - The logit model suggests that the government regulations of school closures, travel restrictions, state of emergency declarations, wage support, tax credits, and interest rate lowering decreased the log odds of the presence of virus cases.  Government regulations such as disallowing public gatherings and mandating wearing masks did not decrease the log odds of the presence of virus cases.  For the train set, the model has a percision score of 81, a recall score of 83, an f1 score of 82, an accuracy score of 82, a specificity score of 83, an roc auc score of 82, and a cross validated negative log loss score of -.48.  For the test set, the model has a percision score of 81, a recall score 0f 82, an f1 score of 82, an accuracy score of 82, a specificity score of 83, an roc auc score of 82.  
    - The XGBoost model indicates that no statistically significant feature had significantly more importance than the others in classifying the amount of cases.  For the train set: class 0 has a precision score of 89, a recall score of 88, an f1 score of 88, an accuracy score of 90, a specificity score of 91, an roc auc score of 89; class 1 has a precision score 83, a recall score of 87, an f1 score of 85, an accuracy score of 87, a specificity score of 90, and an roc auc score of 87; class 2 has a precision score of 88, a recall score of 78, an f1 score of 83, an accuracy score of 95, a specificity score of 96, and an roc auc score of 88.  Cross validated roc auc score for class 0 is 89, for class 1 is 86, and for class 2 is 88.  For the test set: class 0 has a precision score of 89, a recall score of 88, an f1 score of 88, an accuracy score of 90, a specificity score of 91, and a roc auc score of 90; class 1 has a precision score 83, a recall score of 87, an f1 score of 85, an accuracy score of 87, a specificity score of 90, and a roc auc score of .87; class 2 has a precision score of 89, a recall score 77, f1 score 83, accuracy score 95, a specificity score 96, and a roc auc of 88.  
- Deep Learning: 
  - Neural Networks:  
    - The CNN model classified whether a CT-scan has SARS-CoV-2 in it for the train set with a loss score of 1, an accuracy score of 100, a precision score of 100, a recall score of 100, a specificity score of 100, an f1 score of 100, a validation loss score of 32, a validation accuracy score of 87, a validation precision score of 89, a validation recall score of 86, a validation specificity score of 87, and a validation f1 score of 87.  The CNN model has an roc auc of 100 and a mean cross validate accuracy score of 84.  The CNN model performed on the test set with a loss score of 36, an accuracy score of 87, a precision score of 92, a recall score of 78, a specificity score of 95, an f1 score of 84, and an roc auc score of 86.  
    - The bidirectional RNN model predicted the next nucleotide in the sars-cov-2 genome train set with a loss score 40, an accuracy score of 82, a precision score of 94, a recall score of 73, a validation loss score of 37, a validation accuracy score of 87, a validation precision score of 95, a validation recall score of 76, a test loss score of 38, an accuracy score of 85, a precision score of 93, and a recall score of 76.  The bidirectional RNN model has an roc auc score for class 0 of 85, for class 1 of 87, for class 2 of 85, and for class 3 of 86.  The bidirectional RNN model has a mean cross validated accuracy score of 82.  The bidirectional RNN model predicted the test set with a loss score of 38, an accuracy score of 84, a precision score of 94, a recall score of 75, a specificity score of 98, an f1 score of 83, for class 0 an roc auc score of 88, for class 1 an roc auc score of 88, for class 2 an roc auc score of 89, and for class 3 an roc auc score of 88. 
  - Clustering: 
    - The NLP model uses K-means clustering to make term document importance class labels from the tf-idf matrix, and determines that three classes are optimal.  Then, KNN oversampling is used to resolve class imbalance followed by multinomial naive bayes machine learning to determine the posterior probababilty of each word belonging to a document importance class.  For the train set: class 0 has a precision score of 100, a recall score of 92, an f1 score of 96, an accuracy score of 97, a specificity score of 96, a ROC AUC score of 96, and a cross validated ROC AUC score of 85;  class 1 has a precision score of 93, a recall score of 100, an f1 score of 96, an accuracy score of 97, a specificity score of 100, a ROC AUC score of 98, and a cross validated ROC AUC score of 96; and class 2 has a precision score of 100, a recall score of 100, an f1 score of 100, an accuracy score of 100, a specificity score of 100, a ROC AUC score of 100, and a cross validated ROC AUC score of 97. For the test set, all classes have a precision score of 100, a recall score of 100, an f1 score of 100, an accuracy score of 100, a specificity score of 100, and ROC AUC score of 100.  
# Conclusion
Classifying whether a CT-scan has SARS-CoV-2 in it will increase clinical efficiency, and predicting the next nucleotide in a genome will be useful in reconstructing fragmented genomes.  Dose, country, and pause are the words with the greatest document importance.  The virus spread is slowing and will decrease more as more people get vaccinated.  The virus travels in sneezed or coughed droplets of mucus or saliva, is airborne for a few moments, and then lands on a surface. Instead of wearing masks and preventing gatherings, carrying handkerchiefs in which people could sneeze or cough and sanitizing areas where people gather would be sufficient in preventing the spread of SARS-CoV-2.
