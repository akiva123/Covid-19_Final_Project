![image](https://user-images.githubusercontent.com/56414953/112048508-deeba200-8b24-11eb-8cfa-9b61476acc04.png)
# Covid-19 Final Project Introduction
In this report, the covid-19 pandemic test, case, recovery, death, and vaccination totals are covered followed by time-series modeling to determine the progression of the pandemic.  This report uses a logit model to determine the log odds relationship between government covid-19 regulations and cases of SARS-CoV-2.  SARS-CoV-2 symptoms, lifecycle, testing, and vaccines are explaind followed by machine learning that is used to predict the translation process of a SARS-CoV-2 genome to a polypeptide chain.  
# Covid-19 General Information
A new type of coronavirus, SARS-CoV-2, started in December 2019 and has caused the COVID-19 global pandemic. SARS-CoV-2 originated in a Chinese city called Wuhan. Coronaviruses are common in animals, and scientists hypothesize that SARS-CoV-2 may have transfered to humans, zoonosis, through the Wuhan food market. SARS stands for severe acute respiratory syndrome. In 2003, there was an outbreak of SARS in China that spread to other countries and then ended in 2004. SARS-CoV-2 has spread faster than the 2003 SARS. SARS-CoV-2 is spread when an infected person coughs or sneezes droplets of saliva or mucus with the virus into the air. The respiratory droplets usually do not go further than a few feet, are airbourne for a few moments, and then land on a surface. SARS-CoV-2 has an incubation period of 2 to 14 days and the symptoms of the virus include cough, fever or chills, shortness of breath or difficulty breathing, muscle or body aches, sore throat, loss of taste or smell, diarrhea, headache, fatigue, nausea or vomiting, congestion or runny nose, and in rare cases the virus can lead to difficulty walking, confusion, bluish face or lips, coughing up blood, severe respiratory problems, kidney failure, high fever, or death. The following is a diagram of the symptoms.
![image](https://user-images.githubusercontent.com/56414953/112048677-0b072300-8b25-11eb-8840-d80b978cf20b.png)
# Models
The time-series models suggest that, over the next month, vaccinations will trend upward by 724.7% and cases of the virus will trend upward by 12.8%. The logit model suggests that the government regulations of school closures, travel restrictions, state of emergency declarations, wage support, tax credits, and interest rate lowering decreased the log odds of the presence of virus cases.  Government regulations such as disallowing public gatherings and mandating wearing masks did not decrease the log odds of the presence of virus cases.  For the train set, the model has 20765 true positives, 20242 true negatives, 4834 false positives, 4319 false negatives, a percision score of 81, a recall score 0f 83, an f1 score of 82, an accuracy score of 82, a specificity score of 83, an roc auc score of 82.  For the test set, the model has 5233 true positives, 5043 true negatives, 1201 false positives, and 1063 false negatives, a percision score of 81, a recall score 0f 82, an f1 score of 82, an accuracy score of 82, a specificity score of 83, an roc auc score of 82.  For the machine learning translation algorithms, the decision tree, random forest, and gradient boost all predicted the train and test data with scores of 100.  
# Conclusion
The virus spread is slowing and will decrease more as more people get vaccinated.  The virus travels in sneezed or coughed droplets of mucus or saliva, is airborne for a few moments, and then lands on a surface. Instead of wearing masks and preventing gatherings, carrying handkerchiefs in which people could sneeze or cough and sanitizing areas were people gather would be sufficient in preventing the spread of SARS-CoV-2.
