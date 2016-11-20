About R script

File with R code "run_analysis.R" perform 5 following steps (in accordance assigned task of course work):
  Merging the training and the test sets to create one data set.
  Reading files
  Reading trainings tables
  Reading testing tables
  Reading feature vector
  Reading activity labels
  Assigning column names
  Merging all data in one set
  Extracting only the measurements on the mean and standard deviation for each measurement
  Reading column names
  Create vector for defining ID, mean and standard deviation
  Making nessesary subset from setAllInOne
  Using descriptive activity names to name the activities in the data set
  Appropriately labeling the data set with descriptive variable names
  Creating a second, independent tidy data set with the average of each variable for each activity and each subject
  Making second tidy data set
  Writing second tidy data set in txt file

NOTE : The code takes for granted all the data is present in the same folder, un-compressed and without names altered.

                        About variables:
x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
x_data, y_data and subject_data merge the previous datasets to further analysis.
features contains the correct names for the x_data dataset, which are applied to the column names stored
activity_labels contains the data downloaded from the file
merge_train contains the merged training data
merge_test contains the merged test data
SetAllInOne contains the merge_train and merge_test data 
ColNames stores the SetAllInOne data into new table
mean_and_std contains the following vectors(activityId, SubjectId, mean..,std..) from ColNames
setForMeanAndStd contains the sorted data as per mean_and Std
setWithActivityNames contains the merge data of setForMeanAndStd and activity_list
secTidySet contains the aggregated data as per activityId and subjectId and then it is ordered in ascending order as per subjectID
