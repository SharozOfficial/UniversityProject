# UniversityProject

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

# Result

![Image](https://github.com/SharozOfficial/Project2/assets/158645890/05c07ed3-7eec-4397-98cf-55150f5bd75a)
