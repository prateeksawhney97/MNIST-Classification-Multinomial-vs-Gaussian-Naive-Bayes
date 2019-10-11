# MNIST-Classification-Multinomial-vs-Gaussian-Naive-Bayes

### Dataset is imported from sklearn.datasets by load_digits() method.

### Exploring the Dataset:

![original](https://user-images.githubusercontent.com/34116562/66628171-a2bbce80-ec1b-11e9-9daf-4ebafe850f86.png)

#### Gray

![gray](https://user-images.githubusercontent.com/34116562/66628177-a51e2880-ec1b-11e9-89f0-2259e0224cee.png)

#### HSV

![hsv](https://user-images.githubusercontent.com/34116562/66628180-a64f5580-ec1b-11e9-8953-54dee43b4012.png)


### X.shape() reveals that there are 1797 examples and each example has 64 features.

### As, there are 64 features, each image in the dataset is a 8x8 image.

### Models are trained using fit() method as shown:

#### mnb = MultinomialNB()
#### mnb.fit(X,Y)

#### gnb = GaussianNB()
#### gnb.fit(X,Y)

### Score is calculated for both the models using score() method and it shows that Multinomial Naive Bayes performs well as compared to Gaussian Naive Bayes because Multinomial Naive Bayes assumes that the features are discrete whereas Gaussian Naive Bayes assumes them to be continuous. Here, the features are discrete.

#### mnb.score(X,Y)
#### gnb.score(X,Y)

### Result: Multinomial Naive Bayes gives a better score of around 90.5%.
