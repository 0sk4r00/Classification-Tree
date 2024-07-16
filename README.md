# Heart Disease Classification using Decision Trees

This project demonstrates how to use decision trees to classify heart disease using the Cleveland heart disease dataset. The process involves loading the data, preprocessing it, training a decision tree, evaluating its performance, and optimizing the model through cost-complexity pruning.

## Steps:

### 1. Importing Libraries:
- `pandas`: For data loading and manipulation, and for One-Hot Encoding.
- `numpy`: To calculate the mean and standard deviation.
- `matplotlib`: For plotting graphs.
- `scikit-learn`: For building the decision tree classifier, splitting the dataset, cross-validation, and creating confusion matrices.

### 2. Loading and Preprocessing Data:
- The dataset is loaded from a URL.
- Missing values in the 'ca' and 'thal' columns are handled by removing rows containing '?'.
- The target variable 'hd' is converted into a binary classification (0 for no heart disease, 1 for heart disease).
- One-Hot Encoding is applied to categorical features.

### 3. Splitting the Data:
- The dataset is split into training and testing sets.

### 4. Building and Visualizing the Decision Tree:
- A decision tree classifier is created and trained on the training data.
- The decision tree is visualized using `plot_tree`.

### 5. Evaluating the Model:
- The model's performance is evaluated using a confusion matrix.

### 6. Cost-Complexity Pruning:
- Cost-complexity pruning is used to find the optimal value of the pruning parameter alpha.
- Multiple decision trees are created for different values of alpha.
- The accuracy of each tree is plotted against the alpha values to identify the optimal tree.

### 7. Cross-Validation:
- 5-fold cross-validation is used to validate the performance of the decision tree for different alpha values.
- The mean accuracy and standard deviation for each alpha are calculated and plotted.

### 8. Training the Pruned Tree:
- A new decision tree is trained using the optimal value of alpha identified through cross-validation.
- The pruned tree's performance is evaluated using a confusion matrix.
