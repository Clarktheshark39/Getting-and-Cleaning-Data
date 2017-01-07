# Getting-and-Cleaning-Data

This file describes how Project.R works.

# 1) 
Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "UCI". Make sure the folder "data" and the Project.R script are both in the current working directory.

# 2) 
Use source("Project.R") command in RStudio.

# 3)
Two output files have been created in the current working directory:
merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.
data_with_means.txt (220 Kb): it contains a data frame called result with 180*68 dimension.

# 4)

Finally, use data <- read.table("data_with_means.txt") command in RStudio to read the file. The file contains the average of each variable for each activity and each subject, for each of the 6 activities in total and 30 subjects in total, and so we have 180 rows with all combinations for each of the 66 features.
