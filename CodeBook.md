
Project Description
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project.
You will be required to submit:
a tidy data set as described below
a link to a Github repository with your script for performing the analysis, and
a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This file explains how all of the scripts work and how they are connected.
One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Here are the data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
You should create one R script called run_analysis.R that does the following.
Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive activity names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.



subject       | numerical      | 1:30  	     | Subject id numbers
  activityName  | factor with 6 levels        | WALKING, WALKING\_UPSTAIRS, WALKING\_DOWNSTAIRS, SITTING, STANDING, LAYING | Links the class labels with their activity name. (from: https://github.com/dholtz/GettingAndCleaningData/blob/master/project_data/activity_labels.txt)
-**Features/Measures** | numeric | Features/Measures are normalized and bounded within [-1,1]. | Mean or standard deviation of the triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration
+**Features/Measures** | **numeric** | **Features/Measures are normalized and bounded within [-1,1].** | **Mean or standard deviation of the triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration**
 tBodyAcc-mean()-X |
 tBodyAcc-mean()-Y |
 tBodyAcc-mean()-Z |
 @@ -75,4 +75,4 @@ fBodyBodyAccJerkMag-std() |
 fBodyBodyGyroMag-mean() |
 fBodyBodyGyroMag-std() |
 fBodyBodyGyroJerkMag-mean() |
-fBodyBodyGyroJerkMag-std() |
+fBodyBodyGyroJerkMag-std() |x 
