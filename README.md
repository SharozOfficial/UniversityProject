# UniversityProject - Multimedia Populatity Prediction Of Beauty Brands(Lakeme, L'Oreal and Maybelline) from Instragram.

# Techniques: Exploratory Data Analysis - (Data Imputation, Data Cleaning, Outlier Identification, Data Transformation), Feature Engineering (Likes, Views, Comments, Media), Machine Learning, NLP

# Appendix

Git Repository provide by University of Birmingham:
https://git-teaching.cs.bham.ac.uk/mod-msc-proj-2021/sxx182

The above-mentioned repository consists of the following.
1) Dataset for the all the three brands – Lakme, Loreal and Maybelline including images, json and Text (split images, split_Json & Textual_Dataset respectively)
2) Two Jupyter notebooks - The .ipynb files, one referring to popularity prediction using image and json and the other for sentiment analysis using textual data.
   
• Multimodal_popularity_prediction.ipynb
• Textual_Data_sentiment.ipynb

Steps to executing the code:
# Multimodal_popularity_prediction.ipynb – 

For ease of code run have included the labelled data after processing it for train and test. Please follow the below steps.

1) Skip the below steps while running the program
- cell [3][4] of the program which separates the files and label the dataset
- cell [6] of the program as it splits the dataset into train and test.
- cell [45] as it again split the dataset of json files into train and test.

2) Change the folder path defined in cell 5, 7, 44 & 46 as per your own system directory/path where the dataset will be downloaded.
    The above steps are the key to success of the Jupyter notebook “Multimodal_popularity_prediction.ipynb”
    If desired to run on the main dataset to prepare for test and train data without skipping any steps in the code, please      follow below steps. Download the main dataset.

    1) Create a folder Images containing three different folder(Lakme, Loreal, Maybelline)
    2) Mention the path of these folders in cell [2] (Main Dataset) and [3] for Images folder
       
3) Create a folder split_images and mention the path of it in the cell [5], run the cell [6] and rename the val folder       got created in your system to test. Mention these paths in cell [7].
       
4) Create a folder split_json and mention the path of it in the cell [44], run the cell [45] and rename the val folder got created in your system to test. Mention these paths in cell [46].
   
# Textual_Data_sentiment.ipynb

1) Change the folder path defined in cell 13 as per our own system/directory path where the dataset will be downloaded.
   
#Note: The model’s hyperparameter has been tuned using GridSearchCV, due to which it may take longer time for execution. Also, image feature extraction takes around an hour for training and testing dataset which is normal and is not alarming.

# Analysis and Result

Fig 12.1 represents the distribution of likes inclusive of all the three brands. The number of likes has been taken as the X-axis, and frequency (number of images) has been taken as the yaxis. The number of likes ranges from 0 to 60,000. As from the graph, it can be seen very few images were able to achieve the highest mark and mostly were ranged between 0 to 10,000

![Image](https://github.com/SharozOfficial/UniversityProject/assets/158645890/68e4b664-9e57-4464-b6ae-ddc4a1b2d0b3)

Fig 12.2 represents the likes distribution of L’Oreal brand, it can be seen the maximum number the images have received are in the range of 25k, whereas most number of images lies within 5k limit of number of likes.

![Image](https://github.com/SharozOfficial/UniversityProject/assets/158645890/341e9a6a-f5e0-44d0-a06c-c0a109a0ae2f)

Fig 12.3 represents the number of likes of Lakme brand. The maximum number of likes attained by Lakme brand is far less than that of L’Oreal and Maybelline and the most of images lies within the range of 2k number of likes. There were some images which recorded the 8k likes.

![Image](https://github.com/SharozOfficial/UniversityProject/assets/158645890/26bfef5b-3372-4c04-b2fe-0681a7da31c5)

Fig 12.4 represents the number of likes of Maybelline brand. Maybelline has shown better distribution of likes compared to the other two brands. The maximum number of likes attained by couple of images was 60k approximately, while few images were seen to be falling in the range of 20k to 40k number of likes. Whereas there were still quite a number of images which falls in the minimum range of 10k number of likes.

![Image](https://github.com/SharozOfficial/UniversityProject/assets/158645890/75067c42-eb1f-476b-9333-793e008b2d4f)

# Result

Likes comparision between brands - Lakme, L'Oreal and Maybelline.

![Image](https://github.com/SharozOfficial/UniversityProject/assets/158645890/100e4dc5-71ed-49d3-a9db-bf8f5ca19103)

Model Performance Metric Comparision 

![Image](https://github.com/SharozOfficial/Project2/assets/158645890/05c07ed3-7eec-4397-98cf-55150f5bd75a)

# Conclusion
Conclusion
This research presents a new multi-label multimodal, trained with multioutput for popularity prediction of top 3 beauty brands – Lakme, L’Oreal and Maybelline. The proposed method includes statistical texture feature extraction from images for each brand using skimage module features such as Local Binary Pattern (LBP), Gray Level Co-occurrence Matrix (GLCM) and Gabor Filter. 

The method also includes contextual and social feature along with image features such as likes count, comment count for each image, dimensions of an image, following and labels which altogether forms the complete dataset for our analysis to be carried out. 

The proposed method comes to the conclusion that, when compared to other baseline machine learning models like Random Forest Regressor, Support Vector Regressor (SVR), and Linear Regression, the performance of the XGBoost model—both the DMatrix and Regressor— performs best on the provided dataset. The performance of popularity prediction was measured using the metric known as RMSE, and XGBoost came out on top with a score of 0.03952. 

Furthermore, additional sentiment analysis study was carried out on textual data taken from captions, and it was determined that each brand's sentiment polarity falls within a similar range and will have no impact on the accuracy or performance of popularity prediction, if it is included. The final outcome of the predicted numbers of likes associated with each brand's (label) demonstrated that Maybelline's popularity greatly outpaced that of L'Oreal and Lakme.
