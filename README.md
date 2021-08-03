# Computer Vision

## [SIIM-FISABIO-RSNA](https://github.com/Ben-Karr/SIIM-FISABIO-RSNA)
_Object Detection| Deep Learning | CNNs | Data Preparation | Python | kaggle | fastai | torch | pandas_

[![SIIM example](assets/SIIM_example.png)](https://github.com/Ben-Karr/SIIM-FISABIO-RSNA)
_Identify and localize COVID-19 abnormalities on chest radiographs._ In this project I prepared a medical image dataset and the related dataframe to be used in a Neural Net that predicts an arbitrary number of labeled bounding boxes. These boxes are designed to assist doctors in identifying COVID-19 infections by suggesting an area of interest and a classification of these. I adjusted a lot of the fastai utility functions to be able to rapidly prototype and compare models. The backbone of this project is a RetinaNet, that makes use of _Anchor boxes_ and _Focal Loss_ and can be used with different encoders like (X)Resnets or EfficientNets.

## [Shopee Price Match](https://github.com/Ben-Karr/Shopee-PriceMatch)
_Image Recognition | Siamese Neural Net | Deep Learning | CNNs | kaggle | fastai | torch | pandas_
[![Shopee example](assets/shopee_example.png)](https://github.com/Ben-Karr/Shopee-PriceMatch)
_Decide whether two images describe the same item or not._
In this project I refined the fastai SiameseImage class and DataLoader method, to make use of a given dataframe, that contains the items labels and speed up the dataloading process. This problem is often encountered in online retail: if you can _automatically_ decide whether an image of a product your competitor offers is the same as yours, you can adjust the price of yours and gain an advantage. The advantage of the SiameseImage class is, that for every epoch, every image gets paired with a different image to augment the dataset and prevent overfitting. 

## [RoboML](https://github.com/Ben-Karr/RoboML)
_Image Classification | Data Collection/Preparation | Deep Learning | CNNs | fastai | pandas | ipywidgets | matplotlib_
[![RoboML](assets/RoboML_example.JPG)](https://github.com/Ben-Karr/RoboML)
I collected photos of electronic circuits, that were either fully functioning or broken. I cropped, resized and labeled the images with a lot of additional information to make it easy to train a CNN while accounting for different situations, that would occour in "reality". This helped to understand in which situation the classifier predicts reliably and to adapt the data collection process. 

## [Zazzup Webcam](https://github.com/Ben-Karr/zazzup-webcam-opencv)
_C++ | OpenCV | Object Detection | Cascade Classifier_
[![zazzup example](assets/zazzup_example.png)](https://github.com/Ben-Karr/zazzup-webcam-opencv)
_Add a hat and a bowtie to a face in a webcam stream._
I used `C++` and in particular the OpenCV library to dynamically find the bounding box around a face in a video. I then add pictures of a hat and a bowtie to the upper/lower edge of that box.

# Tabular Data

## [Basketball Scores](https://github.com/Ben-Karr/BasketballScores)
_Data Cleansing/Preparation/Visualization | Feature Engineering | Neural Nets | keras | pandas | XGBoost | Regex | scipy_
[![Basketball Scores example](assets/BasketballScores_example.png)](https://github.com/Ben-Karr/BasketballScores)

_Predict the scores of NCAA basketball games._
The data in this project was webscraped so a lot of data cleaning had to be done. Most team names were spelled in different ways, which needed to be fixed first. I engineered some useful features and then trained a neural net with keras. I also compared it to the results of fastai and a gradient boosting algorithm. 

## [House Pricing](https://github.com/Ben-Karr/HousePricing)
_Data Preprocessing/Visualization | Regression | Neural Nets | Gradient Boosting | Ensemble | kaggle | pandas | fastai | XGBoost | sklearn_
[![House Pricing example](assets/HousePricing_example.png)](https://github.com/Ben-Karr/HousePricing)

_Predict the housing prices in a kaggle competition classic._ The main problem with this dataset was, that both the 'none-value' (eg there is no basement) and the missing value were encoded as `nan`. I manually filled all missing values appropriately and learned a Neural Net and a Gradient Booster to predict the house prices. I also ensembled both learners to decrease the error value.

## [Titanic](https://github.com/Ben-Karr/Titanic/)
_Data Preprocessing | Feature Engineering | Classification | Neural Nets | Hyperparameter optimization | kaggle | pandas | fastai | sklearn | XGBoost_

|LName|Pclass|Sex|SibSp|Parch|Cabin|Title|Age|Fare|target|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|Vovk|3|male|0|0|N|Mr|-0.5500|-0.4892|0|
|Tobin|3|male|0|0|F|Mr|-0.0827|-0.4921|0|
|Porter|1|male|0|0|C|Mr|1.2989|0.3984|0|
|Wick|1|female|0|2|C|Miss|0.1156|2.6696|1|
|Sutehall|3|male|0|0|N|Mr|-0.3281|-0.5062|0|
|Klaber|1|male|0|0|C|Mr|0.8885|-0.1138|0|

_Predict who survived the Titanic shipwreck in another classic kaggle competition._
This dataset contains information about all passangers of the Titanic voyage. After preprocessing and condensing some features I used fastai to train a Neural Net on that data. To find the "best" hyperparameters for that Neural Net I ran a random search and stuck with the best performing. I also trained a Gradient Booster but it couldn't beat the NN by itself and ensembled.

# Visualization

## [Netflix Dash](https://github.com/Ben-Karr/NetflixDash)
_Data Visualization | Dashboard | Plotly | Dash | pandas | html_
[![NetflixDash](assets/NetflixDash_example.png)](https://netflix-viz.herokuapp.com/)

_Show and compare which countries watch which Netflix shows._ I used Plotly and Dash to build a Dashboard that lets you choose a list of countries, a list of Netflix show genres which can be visualized in different forms.

# Misc

## [RoboApp](https://github.com/Ben-Karr/RoboApp)
_Deployment | Flask | html | CSS | heroku_
[![RoboApp](assets/RoboApp_example.png)](https://robocircuit.herokuapp.com/)
_Make the Machine Learning algorithm from RoboMl accessible by a webapp._ 
This is my attempt of building a custom webpage with Flask at the backend and html, CSS and JavaScript in the frontend. The design was made to make it simple to navigate through the page with a smartphone.
