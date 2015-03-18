# GettingData
Course Project for Getting and Cleaning Data

The aim of this project is to get the data from the URL provided and clean up the data after merging and combining the training and testing datasets. There are three components -

I. Getting the data
II. Big picture from the data
III. Read data from the files into the variables



I. Getting the data

1. Download the file and put the file in the data folder
2. Unzip the file
3. Unzipped files are in UCI HAR Dataset
4. Read data from the targeted files


II. Big picture from data

The targetted files are the following:
test/subject_test.txt
test/X_test.txt
test/y_test.txt
train/subject_train.txt
train/X_train.txt
train/y_train.txt

1. Values of Variable Activity consist of data from “Y_train.txt” and “Y_test.txt”
2. Values of Variable Subject consist of data from “subject_train.txt” and subject_test.txt"
3. Values of Variables Features consist of data from “X_train.txt” and “X_test.txt”
4. Names of Variables Features come from “features.txt”
5. Levels of Variable Activity come from “activity_labels.txt”
6. So we will use Activity, Subject and Features as part of descriptive variable names for data in data frame


III.Read data from the files into the variables

1. Read the Activity files
2. Look at the properties of the above variables
3. Merges the training and the test sets to create one data set
4. Concatenate the data tables by rows
5. Set names to variables
6. Merge columns to get the data frame Data for all data
7. Extract the measurements on the mean and standard deviation for each measurement


IV. Cleaning up the dataset basing on features

1. Subset Name of Features by measurements on the mean and standard deviation i.e taken Names of Features with “mean()” or “std()”
2. Check the structures of the data frame Data
3. Read descriptive activity names from “activity_labels.txt”
4. Use the descriptive activity names to name the activities in the data set
5. Factorize Variable activity in the data frame Data using descriptive activity names
6. Check appropriately labels the data set with descriptive variable names



Conclusion 

The variables activity and subject and names of the activities have been labelled using descriptive names. Here, the names of features are named according to their labels. Then, an independent tidy set of data is created with the average of each variable for each activity and subject and sent out as an output. 
