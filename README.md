# SVM-GMM---EECE5644
Here a support vector machine (SVM) classifier with a Gaussian kernel was trained to classify data generated.
In the 10-fold cross validation we would perform a fitting procedure a total of 10 times, in which the dataset is divided into 10 folds or subsets.
Each iteration selects 90% of the dataset for training and the remaining 10% for the validation. With each iteration we select a different 90% of the dataset at random and take the remaining 10% for the validation and we calculate the minimum probability of error across the cross validation runs.
Once we conclude on the number to perceptron to use then we can run it again on the full dataset and calculate the probability of error.
In this section, we use GMM-based clustering to segment colour image. The image below shows the RGB colour image and its corresponding grayscale image after clustering with K = 2 components.
The following process was performed on the colour images:
1.
  For preprocessing, generate a 5-dimensional feature array (comprising of row index, column index, r, G, B values)
2.
  For each pixel:
Append row index, column index, red, green and blue values to a feature array
Normalize each feature to [0, 1], i.e., the feature vectors fit in the 5-dimensional hypercube
Run segmentation algorithm on normalized feature vectors
