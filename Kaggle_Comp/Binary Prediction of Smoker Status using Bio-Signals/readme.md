# Kaggle Playground Series - Season 3, Episode 24

## [Binary Prediction of Smoker Status using Bio-Signals](https://www.kaggle.com/competitions/playground-series-s3e24/overview)

The challenge was to employ binary classification techniques to predict a patient's smoking status based on various health indicators.

### Model Performance Summary:

| Algorithm | Accuracy | Remarks |
|-----------|----------|---------|
| Logistic Regression | 0.75556 | Initial simple approach |
| NN (1) - 3 layers [10 epochs, batch size = 16, lr = 0.001] | 0.85873 | First attempt with a 3-layer NN |
| NN (2) - 4 layers [10 epochs, batch size = 16, lr = 0.001] | 0.85712 | Added a layer to assess performance |
| NN (3) - 3 layers [30 epochs, batch size = 16, lr = 0.001] | 0.85928 | Increased epochs, resulting in better accuracy |
| NN (4) - 3 layers [10 epochs, batch size = 32, lr = 1.75E-02] | 0.85022 | Used PyTorch's lr-finder; accuracy decreased |
| NN (5) - 3 layers [30 epochs, batch size = 16, lr = 0.0001] | 0.85956 | Best performance achieved |

**Evaluation Metric**: Area under the ROC curve between the predicted probability and the observed target.

### Folder Contents:

- **Training Notebooks**:
  - [Logistic Regression](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/LogisticReg.ipynb)
    
  - [Neural Network](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/NN_smoke.ipynb)
- **Data**:
  - [Train dataset](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/train.csv)
  - [Test dataset](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/test.csv)
- **Predictions**:
  - [Best prediction CSV (NN(5))](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/best_predictions.csv)
  - [Logistic Regression trial CSV](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/LogisticReg_predictions.csv)
- **Model Checkpoints**:
  - [NN(5) Checkpoint](https://github.com/Hasanmog/Journey-Through-AI-Learning/blob/main/Kaggle_Comp/Binary%20Prediction%20of%20Smoker%20Status%20using%20Bio-Signals/NN_model_checkpoint.pth)
