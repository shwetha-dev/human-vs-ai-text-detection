
# Human vs AI-Generated Text Detection

## Experiment:Entropy + Random Forest

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
