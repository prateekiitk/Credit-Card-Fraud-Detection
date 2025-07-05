## Credit Card Anamoly Detection

### Context
In the financial industry, accurately detecting fraudulent credit card transactions is crucial to protect consumers from unauthorized charges and maintain trust in payment systems.

### Dataset Overview
This dataset contains credit card transactions made by European cardholders in September 2013. It includes transactions over a two-day period, comprising a total of 284,807 entries, of which 492 are confirmed cases of fraud. The dataset is highly imbalanced, with fraudulent transactions representing only 0.172% of all records.

All input features are numerical and have been transformed using Principal Component Analysis (PCA) to ensure confidentiality. As a result, the original feature names and details are not disclosed. The dataset includes:

* V1 to V28: Principal components derived from the PCA transformation

* Time: Time elapsed in seconds between a transaction and the first transaction in the dataset

* Amount: Transaction amount, which may be useful for cost-sensitive modeling

* Class: Target variable indicating whether a transaction is fraudulent (1) or legitimate (0)

### Objective
The goal is to develop a model that can effectively identify fraudulent credit card transactions.

### Evaluation Metric
Due to the strong class imbalance, traditional accuracy metrics can be misleading. Instead, I recommend evaluating model performance using the Area Under the Precision-Recall Curve (AUPRC), which provides a more meaningful measure in this context.

### Acknowledgements
This dataset was compiled as part of a collaborative research project between Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of the Université Libre de Bruxelles (ULB).
