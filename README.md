Background:
Ischemic heart disease remains the leading cause of death worldwide, accounting for approximately 13% of all global mortality according to the World Health Organization. In the United States, heart attack–related deaths have declined by nearly 90% since 1970, largely due to advances in prevention and treatment. Traditional cardiovascular disease (CVD) risk prediction models typically rely on established clinical predictors such as age, sex, hypertension, and smoking status.
This research project aimed to develop an enhanced machine learning–based risk prediction model that integrates traditional clinical indicators with socio-economic and environmental variables. By incorporating these additional factors, we sought to improve predictive accuracy and uncover previously underrecognized contributors to CVD risk, ultimately informing more effective prevention strategies.

Data:
 This project utilized a publicly available CVD dataset from Kaggle, comprising 5,111 individual patient records. The dataset includes 12 features, such as patient ID, BMI, average glucose level, stroke history, smoking status, hypertension, heart disease history, and sociodemographic variables including age, gender, marital status, work type, and residence type.

Methods:
 Data preprocessing involved cleaning the dataset and encoding categorical variables. Binary categories such as gender, marital status, and residence type were encoded as 0/1. Smoking status was encoded as 0, 1, and 2 (formerly smoked, never smoked, currently smoking) to assess gradations in smoking behavior and their influence on CVD risk.
Multiple supervised learning algorithms were applied, including logistic regression, k-nearest neighbors (kNN), decision trees, and random forests. Model performance was evaluated using standard classification metrics—accuracy, precision, recall, and F1 score—along with ROC–AUC analysis to assess discriminatory ability.

Results:
 Logistic regression identified several significant predictors of CVD risk, including age, glucose level, gender, and smoking status. These variables demonstrated strong associations with CVD outcomes, and the model exhibited good overall fit with statistically significant coefficients.
The kNN analysis explored performance using subsets of predictors, such as glucose level and BMI. While the model attempted to differentiate classes (0 = no CVD, 1 = CVD), the visualization did not reveal clear separation between groups, suggesting that these variables alone are insufficient for reliable classification and may lead to misclassification.
Decision tree models provided additional insights, highlighting that CVD risk increases with age and elevated glucose levels. Gender was also identified as a modifying factor among older individuals, and young individuals with high glucose levels were found to have increased risk as well.
Across models, accuracy ranged from 90% to 95%, with precision, recall, and F1 scores indicating strong performance. However, the results also suggested a tendency toward predicting the majority class, underscoring class imbalance as a limitation that may affect model reliability.

Conclusion:
 The project successfully developed and evaluated multiple machine learning models for predicting cardiovascular disease by integrating both traditional clinical factors and socio-economic/environmental indicators. Decision trees and random forests, in particular, enabled broader exploration of variable interactions and improved predictive performance.
Future directions include experimenting with alternative encoding techniques, such as target encoding or likelihood encoding, to further enhance model performance. Addressing class imbalance will also be a priority. Implementing a combination of oversampling and undersampling methods may yield a more balanced dataset and reduce the limitations inherent in using a single approach.
