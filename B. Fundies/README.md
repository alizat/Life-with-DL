Irrigation prediction pipeline

Files:
- irrigation.ipynb : jupyter notebook to perform EDA, train on numeric-only then include encoded categorical variables, and evaluate on test set.
- requirements.txt : Python dependencies
- irrigation.csv : dataset


Notes:
- The script will use GPU if available (torch.cuda.is_available()).
- It drops rows with missing values for simplicity.
- Adjust hyperparameters (batch size, lr, epochs) inside the script as needed.
