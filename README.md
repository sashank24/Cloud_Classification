# Cloud Classification Prediction

This Model tries to classify the different types of cloud formation using satellite images 

There are 4 types of cloud formations:
- Fish
- Flower
- Sugar
- Gravel

In this project we are going to classify the formations between these 4 classes.

## Reason For This Project

As we all know that climate is highly unstable and there are a lot of factors influencing the change in formations. Even for humans it is a challenging task to interpret the climate and make accurate predictions.

Hence, i want see how well Neural Networks can look for and find patterns in the images which are imposible to analyze by humans and check if there are other factors/variables which impacts the overall climate and prove that even in chaotic instances where humans fail to fathom, Neural Networks can predict the patterns and produce convincing results.  

**🔑 KEY NOTE: please read this**

There are 2 notebooks in this repo.
- In the first Notebook i have performed Exploratory Data Analysis(EDA)
- In the second Notebook i have performed the Model Building

*sometimes github doesnt load the EDAnotebook inorder to get the full experience of the notebook please click this* -> [EDA_notebook](https://nbviewer.jupyter.org/github/sashank24/Cloud_Classification/blob/main/Cloud_Pattern_Prediction_EDA.ipynb) (📍wait for it load...)

*if the above method doesn't work TRY THIS* -> copy paste this link https://github.com/sashank24/Cloud_Classification/blob/main/Cloud_Pattern_Prediction_EDA.ipynb in this [nbviewer.jupyter.org](https://nbviewer.jupyter.org/) website and click the file with the '.ipynb' extension and wait for it to render (takes about 10 seconds) 


## Data Overview

- The satellite images data was provided by reasearchers from Max Planck Institute for Meteorology
- It consists of Train and Test images which are already seperated.
- There is a total of 5700 images approx in Train and around 3600 images in Test data

## Source

The Images data was obtained from the kaggle.
The link is anchored here -> [Understanding Clouds from Satellite Images](https://www.kaggle.com/c/understanding_cloud_organization)

## Imports

> *Numpy*

> *Pandas*

> *tqdm* 

> *Sklearn*

> *OpenCV*

> *Glob* 

> *Tensorflow*

> *Keras*

> *Matplotlib*

> *seaborn*

> *plotly*

> *albumentations*

## Model Overview

- Used InceptionResNetV2 a pretrained Model on ImageNet to train the data.
- Overall model took **32 hours** to train.
- The Mean PR AUC was around **61%**.
- This model's Recall was good and out of all the truth values it successfully predicted the True Positives almost perfectly
