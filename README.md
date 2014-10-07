Getting and Cleaning Data - Project

Source dataset https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

You should create one R script called run_analysis.R that does the following.
Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive activity names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Notes

Only vaiables containing mean() & std() are used.
Requires the plyr & reshape2 packages.
Assumes the dataset is unzipped in the current directory.

$ Rscript run_analysis.R
Yields tidy.txt & tidy.mean.txt.
