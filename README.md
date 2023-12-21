# Health_AI_project
The goal of the project is to enhance the predictive analytics capability in the context of fetal Health. The given Fetal Health dataset contains many features. On the surface, it could seem that larger number of features means better accuracy but, machine learning algorithms often tend to overfit in the context of large number of features. Each and every feature also requires expensive equipment to be captured. Thus, if we are able to reduce the number of input features to the machine learning algorithm while maintaining a high accuracy, we can lower the overall cost of fetal health prediction and make the predictions more accurate.

We are initially given a fetal health dataset that contains 28 features. These features measure different aspects of a featus's health. But, it is impossible to consider all these features in order to make an accurate prediction about the health of the featus. Thus, we aim to find the most important features that are required to make the prediction about the health of a featus. To solve this problem, we divided the input data into training and testing data, while handling the class imbalance and trained and tested the performance of various machine learning models. After that, we performed various dimensionality reduction techniques for the purpose of feature selection. With the features that we obtained from the dimensionality reduction techniques, we trained the machine learning models again and observed the increase in the accuracy of the models. This way, we were able to reduce the number of features required for the purpose of fetal health prediction.

Objective

The objective of the problem is to find the list of features that are most linearly dependent to the fetal health so that they can be used to train the machine learning algorithms instead of the complete set of attributes. The given dataset has about 28 features. These features should be reduced to a smaller set of features that can explain the maximum amount of variability. For example, we select those features that can explain upto 95% of the variance in data when we use Principal Component Analysis.

Dataset

The dataset was compiled by Ayres de Campos et al. (2000). The dataset contains 2126 measurements extracted from cardiotocograms and classified by expert obstetricians. The dataset contains 28 features which all required expensive equipment to measure.

Approach

We first measure how linearly dependent each feature is to the output feature. Then we display the coorelation matrix and identify that the features are linearly dependent. By seeing this, we decided to use Principal Component Analysis(PCA) and Linear Discriminant Analysis(LDA) for the purpose of feature selection. After doing the feature selection with the class imbalace being handled, we trained various machine learning models and compared their accuracies and various other performance metrics like precision, recall, F1 score, etc.

Conclusion

In summary, we were able to identify 16 features that are enough to make accurate predictions about the fetal health using PCA. We also showed that the models being trained with the complete set of features were being overfit to the data. LDA also proves to be a viable technique for the purpose of feature extraction.
