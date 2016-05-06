# GettingandCleaningAssignment
**Human Activity Recognition Using Smartphones Data Set**
from: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Purpose: Develop R script that provides tidy data based on the above data set.
Background
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

Method: 
- Find all files of interest in the dataset
- Use read.table function to import the data into R
-The 'test' and 'train' data groups are worked on separately
-Read the subject numbers
-Read the data 'x' variables
-Apply the 'features' labels to the 'x' data
-Read the encoded activity labels (e.g. 1, 2, 3, etc,)
-Match the activity number to the encoded values found in 7.
-Combine all the the test data into one data frame with cbind
-Preform 2. through 9. on the 'train' data
-Combine the 'test' and 'train' data with rbind
-Find all of the mean and std variables using grep and regular expressions
-Subset the whole dataset by 12.
-Melt the data separating the subject and the activity
-Recast the data by the combinations of subject*activity reporting the mean value
-Output the final data as a text file by write.table
-The file data set can be read back into R with {data <- read.table(file="tidy.txt",row.name=FALSE)}
