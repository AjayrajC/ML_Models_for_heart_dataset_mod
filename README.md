# Steps
1. ## Importing the Dataset
2. ## Checking for null values
3. ## Splitting the dataset
4. ## Models as an array
   ### models = [
    LogisticRegression(max_iter=10000),
    SVC(max_iter=10000),
    KNeighborsClassifier(),
    RandomForestClassifier(),
    GradientBoostingClassifier(n_estimators=10000),
    AdaBoostClassifier(n_estimators=10000),
    XGBClassifier(n_estimators=10000),
    DecisionTreeClassifier(),
    GaussianNB(),
    MLPClassifier(max_iter=10000)
]
5. ## Model hyperparameters
   ### model_hyperparameters = {
    'logistic': {
        'C': [1, 5, 10, 20, 25]
    },
    'svm': {
        'kernel': ['linear', 'poly', 'rbf', 'sigmoid'],
        'C': [1, 5, 10, 20, 25]
    },
    'knn': {
        'n_neighbors': [2, 3, 5, 8, 10]
    },
    'rf': {
        'n_estimators': [5, 10, 25, 50, 100]
    },
    'gradient_boosting': {
        'n_estimators': [50, 100, 150, 200, 250]
    },
    'adaboost': {
        'n_estimators': [50, 100, 150, 200, 250]
    },
    'xgboost': {
        'n_estimators': [50, 100, 150, 200, 250]
    },
    'decision_tree': {
        'max_depth': [10, 20, 30, 40, 50]
    },
    'naive_bayes': {
        'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5]
    },
    'mlp': {
        'hidden_layer_sizes': [(50,), (100,), (150,), (200,), (250,)]
    }
}
 ## Output
 
	Model used                        	              Highest score	    Best Hyperparameters
# 0	LogisticRegression(max_iter=10000)	              0.831585	        {'C': 5}
# 1	SVC(max_iter=10000)                                   0.778415	        {'C': 1, 'kernel': 'linear'}
# 2	KNeighborsClassifier()                        	      0.643880	        {'n_neighbors': 5}
# 3	RandomForestClassifier()          	              0.828415	        {'n_estimators': 50}
# 4	GradientBoostingClassifier(n_estimators=10000)	      0.811694	        {'n_estimators': 50}
# 5	AdaBoostClassifier(n_estimators=10000)	              0.785137	        {'n_estimators': 50}
# 6	XGBClassifier(base_score=None, booster=None, c...     0.795191	        {'n_estimators': 150}
# 7	DecisionTreeClassifier()	                      0.762131	        {'max_depth': 40}
# 8	GaussianNB()	                                      0.811639	        {'var_smoothing': 1e-05}
# 9	MLPClassifier(max_iter=10000)	                      0.814918	        {'hidden_layer_sizes': (50,)}




