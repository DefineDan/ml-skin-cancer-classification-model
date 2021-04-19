# ML skin cancer classification model

The jupyter notebook consist of a start to finish workflow of building a machine learning classification model from around 10.000 images.  It classifies the cancer type of skin lesions in all 7 important diagnostic categories in the realm of pigmented lesions. It includes common steps like data visualizations, data preprocessing, model building with tf.keras, training, evaluation and predicting on test images, as well as exporting the model for the mobile app I built additionally (see other github repro).

The data is in form of a large collection of multi-source dermatoscopic images of common pigmented skin lesions provided by

Tschandl, Philipp, 2018, "The HAM10000 dataset, a large collection of  multi-source dermatoscopic images of common pigmented skin lesions", https://doi.org/10.7910/DVN/DBW86T, Harvard Dataverse, V3, UNF:6:/APKSsDGVDhwPBWzsStU5A== [fileUNF]

in context of the HAM10000 ("Human Against Machine with 10000 training images")  challenge in 2018.

### Current status

The precision of the model at this point is around 85%. 

### Things to improve

The classes of dataset were very imbalanced. Since some images represent the same lesion, one could be smarter about deleting certain images in the process of balancing. The same holds true for data augmentation.

The model is not perfectly accurate yet and therefor needs more time in hyperparameter tuning.

### Mobile App

In addition, I built a minimalistic mobile app with flutter which uses the tf_lite model. 
(see https://github.com/DefineDan/ml-skin-cancer-classification-app)
