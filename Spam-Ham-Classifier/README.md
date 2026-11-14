# Spam/Ham Classifier

Multinomial Naive Bayes implemented from scratch to classify messages as ham or spam. Uses the supplied 5,572-message CSV with separate fitting, validation, and test sets.

| Part | Work |
| --- | --- |
| a | Lowercase and tokenize messages; build a vocabulary and count matrix using fitting data only. |
| b | Estimate priors and word probabilities with Laplace smoothing; classify in log space. |
| c | Rank the five words most associated with spam by log probability ratio. |
| d | Report the default confusion matrix, spam precision, recall, and F1. |
| e | Plot ROC and compute AUC using trapezoids and pair counting, with half credit for ties. |
| f | Choose a validation threshold maximizing recall with ham FPR at most 1%; compare test results with the default rule. |

Test accuracy: **97.94%**. ROC AUC: **0.97579**. Confusion matrix rows are predictions and columns are true labels.
