# Confusion Matrix for Multi Class 

## Introduction
A confusion matrix is a table that is often used to summarize the performance of a classification algorithm (or "classifier") on a set of test data whose true values are known. Confusion matrix were first discussed by Townsend [[1]](https://doi.org/10.3758/BF03213026), and it was in 1998 that the term confusion matrix became popular in Machine Learning thanks to Kohavi and Provost [[2]](http://robotics.stanford.edu/~ronnyk/glossary.html). In supervised machine learning, confusion matrix is a matrix that measures the quality of
a classification system. Each row of the matrix corresponds to an actual class and each column corresponds to a predicted class. Classification accuracy alone can be misleading if you have an unequal number of observations in each
class or if you have more than two classes in your data set. One of the advantages of the confusion matrix is that it quickly shows whether a classification system manages to classify correctly. The confusion
matrix itself is relatively simple to understand, but the associated terminology and the calculation of certain elements of the matrix can be confusing, especially in the case of multiple classes. Manliguez  [[3]](https://www.researchgate.net/publication/310799885_Generalized_Confusion_Matrix_for_Multiple_Classes) derived the generalized formula to calculate the precision, the recall, the
specificity and the global accuracy of the system having multiple classes. His results were used in eight (8) different works ([[4]](https://link.springer.com/chapter/10.1007/978-3-030-26428-4_7) , [[5]](https://ieeexplore.ieee.org/abstract/document/8938419), [[6]](https://ieeexplore.ieee.org/document/8834531), [[7]](https://doi.org/10.1007/s10772-018-9527-4), [[8]](https://www.semanticscholar.org/paper/A-Novel-Intelligent-System-for-Diagnosing-some-of-Elalfi-Elalmi/02d4c1119e9ee00ec657f591c6a59e33786e1a43), [[9]](https://iopscience.iop.org/article/10.1088/1742-6596/1417/1/012015), [[10]](https://www.mdpi.com/1424-8220/20/1/55), [[11]](https://www.atlantis-press.com/journals/ijcis/125934171/view)) to compute the overall accuracy in most cases, but we have realized that it were the only well defined generalized classification metric in Manliguez [[3]](https://www.researchgate.net/publication/310799885_Generalized_Confusion_Matrix_for_Multiple_Classes). The aim of this document is to show the evidence of the mistakes in some generalized classification metrics and also to correct them. To achieve that objective, we have used the analytical approach for binary classification case and the computational approach using python package scikit-learn for the ternary Classification case study.
