# Getting-and-Cleaning-Data

A description of how Project.R works:

# 1) 
Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder "UCI". Make sure the folder "UCI" and the Project.R script both are in the current working directory.

# 2) 
Use the source("Project.R") function in RStudio.

# 3)
Two output files have been created in the current working directory:
data_with_means.txt : containing a data frame with dimensions of 180 and 68.
merged_data.txt : containing a data frame called cleanedData with dimensions of 10299 and 68.

# 4)

Finally, use data <- read.table("data_with_means.txt") command in RStudio to read the file. The file contains the average of each variable for each activity and each subject, for each of the 6 activities in total and 30 subjects in total, and so we have 180 rows with all combinations for each of the 66 features.
