

### Tidy Mean

A data.table named `tidy.mean` is set with the following columns.  All units are maintained from the original data set. A file named tidy.mean.txt is written from run_analysis.R.

| column       | description                                              | type    |
| ------------ | -------------------------------------------------------- | ------- |
| Subject      | Identifier of the subject                                | integer |
| Activity     | Label of the activity                                    | factor  |
| MeanSamples  | Mean of variables by Subject + Activity provided in tidy | numeric |

### Tidy

A data.table named `tidy` is set with the following columns.  All units are maintained from the original data set. A file named tidy.txt is written from run_analysis.R.

| Column                       | Original Name               |
| ---------------------------- | --------------------------- |
| Activity                     |  Subject                    |
| Time.BodyAcc.Mean.X          | tBodyAcc-mean()-X           |
| Time.BodyAcc.Mean.Y          | tBodyAcc-mean()-Y           |
| Time.BodyAcc.Mean.Z          | tBodyAcc-mean()-Z           |
| Time.BodyAcc.Std.X           | tBodyAcc-std()-X            |
| Time.BodyAcc.Std.Y           | tBodyAcc-std()-Y            |
| Time.BodyAcc.Std.Z           | tBodyAcc-std()-Z            |
| Time.GravityAcc.Mean.X       | tGravityAcc-mean()-X        |
| Time.GravityAcc.Mean.Y       | tGravityAcc-mean()-Y        |
| Time.GravityAcc.Mean.Z       | tGravityAcc-mean()-Z        |
| Time.GravityAcc.Std.X        | tGravityAcc-std()-X         |
| Time.GravityAcc.Std.Y        | tGravityAcc-std()-Y         |
| Time.GravityAcc.Std.Z        | tGravityAcc-std()-Z         |
| Time.BodyAccJerk.Mean.X      | tBodyAccJerk-mean()-X       |
| Time.BodyAccJerk.Mean.Y      | tBodyAccJerk-mean()-Y       |
| Time.BodyAccJerk.Mean.Z      | tBodyAccJerk-mean()-Z       |
| Time.BodyAccJerk.Std.X       | tBodyAccJerk-std()-X        |
| Time.BodyAccJerk.Std.Y       | tBodyAccJerk-std()-Y        |
| Time.BodyAccJerk.Std.Z       | tBodyAccJerk-std()-Z        |
| Time.BodyGyro.Mean.X         | tBodyGyro-mean()-X          |
| Time.BodyGyro.Mean.Y         | tBodyGyro-mean()-Y          |
| Time.BodyGyro.Mean.Z         | tBodyGyro-mean()-Z          |
| Time.BodyGyro.Std.X          | tBodyGyro-std()-X           |
| Time.BodyGyro.Std.Y          | tBodyGyro-std()-Y           |
| Time.BodyGyro.Std.Z          | tBodyGyro-std()-Z           |
| Time.BodyGyroJerk.Mean.X     | tBodyGyroJerk-mean()-X      |
| Time.BodyGyroJerk.Mean.Y     | tBodyGyroJerk-mean()-Y      |
| Time.BodyGyroJerk.Mean.Z     | tBodyGyroJerk-mean()-Z      |
| Time.BodyGyroJerk.Std.X      | tBodyGyroJerk-std()-X       |
| Time.BodyGyroJerk.Std.Y      | tBodyGyroJerk-std()-Y       |
| Time.BodyGyroJerk.Std.Z      | tBodyGyroJerk-std()-Z       |
| Time.BodyAccMag.Mean         | tBodyAccMag-mean()          |
| Time.BodyAccMag.Std          | tBodyAccMag-std()           |
| Time.GravityAccMag.Mean      | tGravityAccMag-mean()       |
| Time.GravityAccMag.Std       | tGravityAccMag-std()        |
| Time.BodyAccJerkMag.Mean     | tBodyAccJerkMag-mean()      |
| Time.BodyAccJerkMag.Std      | tBodyAccJerkMag-std()       |
| Time.BodyGyroMag.Mean        | tBodyGyroMag-mean()         |
| Time.BodyGyroMag.Std         | tBodyGyroMag-std()          |
| Time.BodyGyroJerkMag.Mean    | tBodyGyroJerkMag-mean()     |
| Time.BodyGyroJerkMag.Std     | tBodyGyroJerkMag-std()      |
| FFT.BodyAcc.Mean.X           | fBodyAcc-mean()-X           |
| FFT.BodyAcc.Mean.Y           | fBodyAcc-mean()-Y           |
| FFT.BodyAcc.Mean.Z           | fBodyAcc-mean()-Z           |
| FFT.BodyAcc.Std.X            | fBodyAcc-std()-X            |
| FFT.BodyAcc.Std.Y            | fBodyAcc-std()-Y            |
| FFT.BodyAcc.Std.Z            | fBodyAcc-std()-Z            |
| FFT.BodyAccJerk.Mean.X       | fBodyAccJerk-mean()-X       |
| FFT.BodyAccJerk.Mean.Y       | fBodyAccJerk-mean()-Y       |
| FFT.BodyAccJerk.Mean.Z       | fBodyAccJerk-mean()-Z       |
| FFT.BodyAccJerk.Std.X        | fBodyAccJerk-std()-X        |
| FFT.BodyAccJerk.Std.Y        | fBodyAccJerk-std()-Y        |
| FFT.BodyAccJerk.Std.Z        | fBodyAccJerk-std()-Z        |
| FFT.BodyGyro.Mean.X          | fBodyGyro-mean()-X          |
| FFT.BodyGyro.Mean.Y          | fBodyGyro-mean()-Y          |
| FFT.BodyGyro.Mean.Z          | fBodyGyro-mean()-Z          |
| FFT.BodyGyro.Std.X           | fBodyGyro-std()-X           |
| FFT.BodyGyro.Std.Y           | fBodyGyro-std()-Y           |
| FFT.BodyGyro.Std.Z           | fBodyGyro-std()-Z           |
| FFT.BodyAccMag.Mean          | fBodyAccMag-mean()          |
| FFT.BodyAccMag.Std           | fBodyAccMag-std()           |
| FFT.BodyBodyAccJerkMag.Mean  | fBodyBodyAccJerkMag-mean()  |
| FFT.BodyBodyAccJerkMag.Std   | fBodyBodyAccJerkMag-std()   |
| FFT.BodyBodyGyroMag.Mean     | fBodyBodyGyroMag-mean()     |
| FFT.BodyBodyGyroMag.Std      | fBodyBodyGyroMag-std()      |
| FFT.BodyBodyGyroJerkMag.Mean | fBodyBodyGyroJerkMag-mean() |
| FFT.BodyBodyGyroJerkMag.Std  | fBodyBodyGyroJerkMag-std()  |

### Description of the run_analytics.R process

1.  Loads library plyr
2.  Downloads required data from (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
3.  Creates results folder
4.  Loads feature data set features.txt used for columns
5.  Loads and appends train dataset using X_train.txt, y_train.txt, subject_train.txt
      subject_train contains the ids
      y_train contains the activity labels
      X_train contains the data using the feature data set as columns
6.  Loads and appends test dataset using X_test.txt, y_test.txt, subject_test.txt
      subject_test contains the ids
      y_test contains the activity labels
      X_test contains the data using the feature data set as columns
7.  Appends train and test data
8.  Rearrange the data using id
9.  Loading activity labels activity_labels.txt
10. Changes the data activity row to use the activity labels
11. Extracts the mean,std into tidy
12. Saves tidy into result/tidy.csv
13. Uses plur to calculate mean on activity for each id
14. appends _mean to all data columns
15. saves the tidy.mean into result/tidy.mean.csv


## tidy.csv

contains 10299 rows and 81 columns in a default csv format.

## tidy.mean.csv

contains 180 rows and 81 columns in a default csv format.





### Notes

Source data is from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.
