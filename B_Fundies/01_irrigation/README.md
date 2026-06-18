Irrigation prediction pipeline

Files:
- irrigation.ipynb : jupyter notebook with the code.
- irrigation.csv : dataset

What is in the notebook?
- feed-forward network trained on a tabular dataset containing both numerical and categorical features. Target variable contains 3 different classes, so this is a multi-class classification problem:
    - a network is first trained on just the numerical features
    - a second network is then trained and then compared to the first model in terms of prediction performance (precision, recall, f-score)
- After that a few tricks are employed to improve prediction performance:
    - adjusting class weights to deal with class imbalance (one of the class has significantly fewer instances that the other two classes)
    - kaiming initialization: helps avoid gradients vanishing or exploding; although this wasn't an issue here, it did help improve the results
    - (coming soon) target-encoding of categorical variables
    - (coming soon) early-stopping to avoid over-training, so the prediction performance would be the best it could

Notes:
- The script will use GPU if available (`torch.cuda.is_available()`).
- It drops rows with missing values for simplicity.
- Adjust hyperparameters (batch size, lr, epochs) inside the script as needed.
