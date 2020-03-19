
##Project Introduction
The run_analysis.R script performs the data preparation and then followed by the 5 steps required as described in the course project’s definition.

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

##Datasets
- This project will use six data, which are x_train.txt, x_test.txt, y_train.txt, y_test.txt, subject_train.txt and subject_test.txt, they can all be found inside the downloaded dataset, namely URI HAR Dataset.
- The features.txt contains the correct variable name, which corresponds to each column of x_train.txt and x_test.txt. Further explanation of each feature is in the features_info.txt.
- The activity_labels.txt contains the desciptive names for each activity label, which corresponds to each number in the y_train.txt and y_test.txt.

##Files
- CodeBook.md a code book that describes the variables, the data, and any transformations or work performed to clean up and prepare the data. 
- run_analysis.R performs the data preparation and then followed by the 5 steps required as described in the course project’s definition.

##Instructions
###1. Merges the training and the test sets to create one data set

- Dataset downloaded and extracted under the folder called UCI HAR Dataset
- Merge train and test data 

###2.Extracts only the measurements on the mean and standard deviation for each measurement

- Load feature name into R
- For the column of x_data.txt, extract only the ones that have mean() or std() in their names using grep, compare it with feature.txt

###3. Uses descriptive activity names to name the activities in the data set

- Load activity labels into R 
- Match each number in the y_data column with activity_labels.txt

###4. Appropriately labels the data set with descriptive variable names

- Rename the column of y_data and subject_data, instead of using the default name given by R.

###5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject

- Write out the tidy dataset to tidydata.txt after going through all the sequences described above.



