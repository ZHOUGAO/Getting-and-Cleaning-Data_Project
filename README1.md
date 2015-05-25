This is the code for Getting-and-Cleaning-Data_Project.
The data is download from "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"
The purpose of the code is to produce a Tidy Data with a clean results based on the activities and subjects

The zipfile includes multiple files, so function 'unzip' was applied to produce the file list
Based on the file list, the requested table can be input using read.table()

The code includes 5 steps

Step 1 merges the training and test data, and come up with a new data set
Step 2 combine the results in feature.txt, and extracts the corresponding variabls in the previous data set
Step 3 introduce the activity name to the data from the file activity_labels.txt, and name the new label based data set
Step 4 merge the label data to the previous data set (the result of step 2)
Step 5 calculate the average values of each varibles based on each activity and subject individually.
      the final results were put together in one data set using funtion "Summarize" in package "dplyr"
