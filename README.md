# Task6

 Task 6: K-Nearest Neighbors (KNN) Classification – Explanation
Objective:
To understand and implement the K-Nearest Neighbors algorithm for solving classification problems using the Iris dataset.

Step-by-Step Breakdown of What I Did:
Step 1: Imported Required Libraries
I started by importing all necessary Python libraries:
pandas and numpy for data handling.
matplotlib for plotting graphs.
scikit-learn modules for loading datasets, building models, scaling features, evaluating performance, and visualization.

Step 2: Loaded the Dataset
I used the built-in Iris dataset from sklearn.datasets.
Extracted features (X) and target labels (y).
Explored the dataset structure and confirmed it has 150 samples and 3 classes (Setosa, Versicolor, Virginica).

Step 3: Normalized the Features
Since KNN is a distance-based algorithm, it is very sensitive to feature scales.
I used StandardScaler to normalize the features so they all have mean = 0 and standard deviation = 1.

Step 4: Split the Data into Training and Testing Sets
Used train_test_split to split data into 70% training and 30% testing.
I used stratify=y to ensure each class is proportionally represented in both sets.
This helps in fair evaluation of the model.

Step 5: Trained KNN Models with Multiple K Values
Built multiple KNN models using different values of K (from 1 to 10).
For each K, I trained the model on training data and evaluated it on test data.
Calculated the accuracy for each value of K.
Observed how model performance varies with different K values.

Step 6: Selected the Best K and Evaluated the Model
Based on the accuracy scores, I selected the best-performing K (e.g., K=3).
Re-trained the model using this K value and made final predictions.
Evaluated the model using:

Accuracy score
Confusion matrix to visualize misclassifications.
Used ConfusionMatrixDisplay to show predictions vs actual labels.

Step 7: Visualized Decision Boundaries (2D)
For visualization, I used only the first two features of the dataset.
Plotted the decision boundary created by KNN using contourf() and a mesh grid.
Overlaid the test samples on this plot to show how the classifier is separating the classes.
This helped visualize how well the model can classify different classes in 2D space.

Conclusion:
The KNN algorithm was successfully implemented and evaluated using the Iris dataset. I experimented with different K values and visualized the results effectively. The Iris dataset was ideal for this task because it is clean and easy to interpret, helping to focus on understanding the working of KNN.
