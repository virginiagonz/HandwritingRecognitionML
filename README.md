# HandwritingRecognitionML
The dataset includes 1797 small images (8x8 pixels), each one includes a hand-written digit (0-9). You have to download the corresponding csv file that includes the labels of the images. The goal is to build a Machine Learning Algorithm that can recognize the hand-written digits!

## Part A
Download the dataset “Digit” and its label from this link:  https://app.box.com/s/sogk96kukv6ayyyy6ym63a2nu3aozif7 Links to an external site.

Check out the dataset. It includes 1797 small images (8x8 pixels), each one includes a hand-written digit (0-9). You have to download the corresponding csv file that includes the labels of the images. The goal is to build a Machine Learning Algorithm that can recognize the hand-written digits!

Import the following two libraries to work with images:

  import matplotlib.image as mpimg

  import matplotlib.pyplot as plt

you can use:

  mpimg.imread(file_name)   to load an image, and

  plt.imshow(image_name, cmap=plt.cm.gray_r, interpolation='nearest')  to show an image.

  Add   %matplotlib inline   at top of your code to make sure that the images will be shown inside the Jupyter explorer page.

## Part B
Build the feature matrix and label vector: Each image is considered as a data sample with pixels as features. Thus, to build the feature table you have to convert each 8x8 image into an array of 64 elements (i.e. 64 pixels), and put it as a row of the feature matrix with 64 feature columns.

## Part C
Use sklearn functions to split the dataset into testing and training sets with the following parameters: test_size=0.1, random_state=2.

## Part D 
Use scikit-learn “Random Forest” classifier to recognize the hand-written digits based on the training/testing datasets that you built in part (c). Use this command to import and define your classifier:

  from   sklearn.ensemble    import    RandomForestClassifier

  my_RandomForest =

  RandomForestClassifier(n_estimators = 19, bootstrap = True, random_state=2)

Use my_RandomForest.fit for training your random forest classifier and my_RandomForest.predict  for prediction. Test your Machine Learning Algorithm on testing set (from part(c)), and calculate and report the accuracy.

## Part E
Write some codes to find which one of the data samples (i.e. which images) have been misclassified (classified incorrectly) in your testing set. Then, use the following command to show the misclassified images:   

  plt.imshow(image_name, cmap=plt.cm.gray_r, interpolation='nearest')  
