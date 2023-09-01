

<h1>Titanic_RandomForest</h1>
<h3>A machine learning model to predict the survivors who sailed in The Titanic using Random Forest Classification technique
</h3>
<h1>Dataset</h1>


<P>The dataset for this particular project was taken from Kaggle.com, a well known resource for machine learning datasets and codes. Titanic - Machine Learning from Disaster is one of if not the most popular beginners problem in Kaggle. You can access the dataset by clicking <a href="https://www.kaggle.com/competitions/titanic/data">here</a></a></P>

<h1>Correlation Matrix</h1>

<img src="https://ik.imagekit.io/xcalibers/Screenshot%202023-09-01%20102715.png?updatedAt=1693544713675" width="350" alt="correlation Matrix image">

<h1>Train-Test Split</h1>

<p>The splitting method used in this project is 'Stratified Shuffle split', with the attributes 'Survived', 'sex' and 'pclass' as test indices. The ratio of the specified records in train and test sections can be inferred below:</p>

<img src="https://ik.imagekit.io/xcalibers/Screenshot%202023-09-01%20103829.png?updatedAt=1693545059486" width="350" alt="correlation Matrix image">

<h1>Model</h1>

<p>The model used for this specific project is Random Forest Classifier which is an ensemble machine learning model from the Scikit Learn library that combines multiple decision trees to make predictions. It creates diverse trees by using random subsets of data and features, and then aggregates their predictions to achieve more accurate and robust results for classification tasks. This approach helps mitigate overfitting and enhances generalization by leveraging the wisdom of multiple trees.</p>

<h1>Hyperparameter Tuning</h1>

<p>Hyperparameter tuning is a critical step in optimizing machine learning models. The purpose of this process is to identify the best combination of hyperparameters that yield the highest model performance. In this example, the GridSearchCV technique is employed to automate the search for optimal hyperparameters.</p>

<li>n_estimators: The number of decision trees in the Random Forest ensemble.</li>
    <li>max_depth: The maximum depth of individual decision trees.</li>
    <li>max_features: The number of features considered for the best split at each node.</li>
    <li>The param_grid variable specifies different values for these hyperparameters. The Grid Search iterates through all possible combinations, evaluating each using cross-validation. The result is the set of hyperparameters that produces the highest accuracy, as measured by the specified scoring metric.

</li><br>

<p>By utilizing GridSearchCV, we automate the process of hyperparameter tuning, allowing us to efficiently explore a wide range of parameter combinations. This approach helps us uncover the best configuration for our Random Forest classifier, ultimately leading to improved classification performance.</p>

<h1>Model Performance Evaluation</h1>

<p>
    After Grid Search Cross-Validation, the Random Forest classifier achieved a commendable accuracy of approximately 81.5% on the test dataset.</p>

<p>    This accuracy score reflects the proportion of correct predictions made by the model, showcasing its ability to effectively classify instances in the given dataset.
</p>


<img src="https://ik.imagekit.io/xcalibers/Screenshot%202023-09-01%20135413.png?updatedAt=1693557355253" width="350" alt="correlation Matrix image">
