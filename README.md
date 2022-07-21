# Facial Images Data Visualization And Analysis

## Abstract
Facial image recognition has a lot of applications as it enables us to detect or verify human faces from an image or a video and therefore is one of the popular areas of research in computer vision. This also has applications in social media and e-commerce such as animoji and face ID. In this project, using state-of-the-art models, we are trying to predict a person’s age, ethnicity, and gender-based on facial features like texture, edges, and wrinkles. 
Objective
The purpose of this project is to effectively determine the age, ethnicity, and gender group of a person based on his/her facial features.
Data description
This dataset is called the UTKFace dataset which contains a large number of facial images (one face per image) and has a wide range of ages from 0 to 116 years old. This dataset includes 23479 images with labels age, ethnicity, and gender, which are approximated by the DEX algorithm and checked by a human annotator. The dataset includes a CSV of facial images that are labeled based on age, gender, and ethnicity. The columns in the dataset are age, ethnicity, gender, img_name, and pixels. 

Number of rows: 23,479
Number of columns: 5
Continuous: Age
Categorical: Gender, Ethnicity
Text: img_name, pixels
Data pre-processing and Exploratory Data Analysis
The first step in building machine learning models is to pre-process the data into a more understandable form and perform exploratory data analysis so that we can find the underlying trends and patterns and finally, they can be fed into the machine learning models for analysis.

## Results
For gender classification, our baseline model works the best. For ethnicity classification, transfer learning works better than the complex and baseline model. For predicting age, transfer learning gives the lowest RMSE of 9.792

### Gender:
Model           Train data accuracy Val data accuracy Test data accuracy
Baseline model       91.46                88.49             88.9
Complex model        97.29                86.87             87.2
Transfer learning    81.68                79.24             78.8


### Ethnicity 
Model          Train data accuracy  Val data accuracy Test data accuracy
Baseline model       84.36               76.52              76.85
Complex model        94.04               71.67              72.5
Transfer learning    81.51               79.44              79.3

### Age 
Model          Train data RMSE      Val data RMSE     Test data RMSE
Baseline model     10.8608              11.0019           10.751
Transfer learning  5.7316               10.2926           9.782

## Conclusion
By analyzing images in relation to the genders, ethnicity, and age using different approaches, we conclude that in most cases using transfer learning would have a better result. From the charts above, we see that both ethnicity and age inferred from the images using transfer learning yielded the best result. However, in the results in the classification of gender, transfer learning did not give the best accuracy. Instead, the simple baseline model did the best among the three models. We conclude that this could be a result of overfitting in this relatively simple classification. 
