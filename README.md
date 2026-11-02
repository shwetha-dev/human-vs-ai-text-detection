
# Human vs AI-Generated Text Detection

## Experiment: mGPT Entropy + Random Forest

### Objective
10-class classification of human-written and AI-generated text.

### Method
1. Use ai-forever/mGPT to calculate token-level predictive entropy.
2. Average token-level entropy for each text.
3. Train a Random Forest classifier using the mean entropy feature.
4. Evaluate the model on a held-out test set.

### Test Results

- Accuracy: 12.96%
- Macro F1: 12.83%
- Weighted F1: 12.86%
- Balanced Accuracy: 12.93%

### Important Note
This experiment applies an entropy-based method to a 10-class
classification task. The results indicate that mean entropy alone
has limited ability to distinguish the ten classes.

### Files
- multiclass_rf_results.json: Experiment configuration and metrics.
- multiclass_confusion_matrix.csv: Test confusion matrix.
- multiclass_rf_tuned.joblib: Trained Random Forest model.

The original dataset and text samples are not included.
