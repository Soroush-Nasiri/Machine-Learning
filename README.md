# Ecoli Gaussian Classifier

Gaussian classifiers implemented from scratch to predict protein localization from seven features. Retains five classes and uses the required class-wise split: 228 training and 99 test samples.

| Part | Work |
| --- | --- |
| a | Fit Gaussian Naive Bayes; count zero variances, apply variance floors, compute stable posteriors with log-sum-exp, and compare three floors. |
| b | Report the confusion matrix, per-class precision/recall/F1, and micro/macro/weighted F1; prove micro-F1 equals accuracy. |
| c | Fit full-covariance QDA with regularization, compare accuracy and parameter counts, and discuss classes with only two samples. |

Test accuracy: **81.82%** for Gaussian NB with floor `1e-4`; **80.81%** for QDA with `epsilon = 1e-4`. Confusion matrix rows are predictions and columns are true labels.
