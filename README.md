# Classification-Algorithm-Comparison
Here, we again use a manually labelled set of 1000 ImageJ pore samples to compare the performance of eight Parameter Optimised Classification algorithms. We then extropolate the best performing model to a larger, unlabelled 100,000 pore dataset, to assess pore distribution accross Gas Flows

Understanding how different morphologies of pores appear at different gas flow rates is an important step in the mitigation of these defects. For this project, Microscope images of cross sections of 3D printed Titanium samples were analysed using ImageJ Image processing software. This software contained a porosity analysis module which produced numeric data based on geometric features for each detected pore. 1000 pores were manually labelled into a Training dataset, which was a smaller subsection of the total of 100,000 pores. These 100,000 pores were obtained at 3 different Gas Flow rates.

In this project, 8 different classification algorithms were analysed, based on their ability to classify this training dataset. How each model classifies the samples was also investigated. Parameters for each were optimised using GridSearchCV, with cross validation. The average Accuracy was obtained, as well as Recall, Precision and F1 score for each class. The best performing model, was the Gradient Boosted Classifier. The ROC, and AUC for this model, for each class was then obtained. 

The Gradient Boosted Classifier was then used, on the 100,000 pore dataset, in order to show that the largest, and most irregular pores (Lack of Fusion) are inversely proportional to the Gas Flow rate in 3D printing. 

Models used: K-Nearest Neighbour, Naive Bayes, Decision Trees Classifier, Support Vector Machine, Logistic Regression, Multi-Layer Perceptron, Gradient Boosted Classifier, XGBoost,

Libraries used: Pandas, Numpy, Scikitlearn, Tensorflow, Pickle, Seaborn, XGBoost
