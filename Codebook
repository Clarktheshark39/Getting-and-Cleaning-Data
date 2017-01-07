Source of the data:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

The Project.R script performs the following steps:
# 1)
Read X_train.txt, y_train.txt and subject_train.txt from the "./UCI/train" directory and store them in the trainData, trainLabel and trainSubject variables.
and 
Read X_test.txt, y_test.txt and subject_test.txt from the "./UCI/test" directory and store them in the testData, testLabel and testsubject variables.
# 2)
Merge testData with trainData to create a data frame with dimensions of 10299 and 561, joinData; Merge testLabel to trainLabel to create a data frame with dimensions of 10299 and 1, joinLabel; Merge testSubject to trainSubject to create a data frame with dimensions of 10299 and 1, joinSubject.
# 3)
Read the features.txt file from the "/UCI" folder and store the data in the variable 'features'. Only extract the measurements on the mean and standard deviation. This results in a 66 indices list. A subset of joinData with the 66 corresponding columns is created.
# 4)
Clean the column names of the subset. Remove the "()" and "-" symbols from the names, and capitalize the first letter of "mean" and "std".
# 5)
Read the activity_labels.txt file from the "./UCI" directory and store the data in a variable called activity.
# 6)
Clean the activity names in the second column of activity. Make all names lower cases. If the name has an underscore between letters, remove the underscore and capitalize the letter immediately after the underscore.
# 7)
Transform the values of joinLabel according to the activity data frame.
# 8)
Combine the joinSubject, joinLabel and joinData by column to get a new data frame with dimensions of 10299 and 68, cleanedData. Name the first two columns, "subject" and "activity". The "subject" column contains integers that range from 1 to 30 inclusive, and the "activity" column contains 6 kinds of activity names. The last 66 columns contain measurements that range from -1 to 1.
# 9)
Create the "merged_data.txt" file in current working directory from cleanedData.
# 10)
Create a second independent tidy data set with the average of each measurement for each activity and each subject. There are 30 unique subjects and 6 unique activities, which create 180 combinations. Calculate the mean of each measurement with the corresponding combination. After initializing the created data frame and performing two for loops, a data frame with dimensions of 180 and 68 is created.
# 11)
Create "data_with_means.txt" file in current working directory from the independent tidy data set just created.
