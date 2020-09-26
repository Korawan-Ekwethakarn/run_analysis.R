# run_analysis.R
Getting and Cleaning Data Course Project
Korawan Ekwethakarn 
September 26, 2020

This is the codebook for the dataset that describes the variables, the data, and any transformations or work that were performed to clean up the Smartphone data obtained from the UCI Machine Learning Repository as part of the final assignment in the course "Getting And Cleaning Data" from Coursera.

subject                    1..30
    Subject number
                           1..30 Unique identifier assigned to each subject

activitylabel              "walking"
                           "walking_upstairs"
                           "walking_downstairs"
                           "sitting"
                           "standing"
                           "laying"

tbodyaccmeanx              Signed value between 0 and 1
    Described below

tbodyaccmeany              Signed value between 0 and 1
    Described below

tbodyaccmeanz              Signed value between 0 and 1
    Described below

tbodyaccstdx               Signed value between 0 and 1
    Described below

tbodyaccstdy               Signed value between 0 and 1
    Described below

tbodyaccstdz               Signed value between 0 and 1
    Described below

tgravityaccmeanx           Signed value between 0 and 1
    Described below

tgravityaccmeany           Signed value between 0 and 1
    Described below

tgravityaccmeanz           Signed value between 0 and 1
    Described below

tgravityaccstdx            Signed value between 0 and 1
    Described below

tgravityaccstdy            Signed value between 0 and 1
    Described below

tgravityaccstdz            Signed value between 0 and 1
    Described below

tbodyaccjerkmeanx          Signed value between 0 and 1
    Described below

tbodyaccjerkmeany          Signed value between 0 and 1
    Described below

tbodyaccjerkmeanz          Signed value between 0 and 1
    Described below

tbodyaccjerkstdx           Signed value between 0 and 1
    Described below

tbodyaccjerkstdy           Signed value between 0 and 1
    Described below

tbodyaccjerkstdz           Signed value between 0 and 1
    Described below

tbodygyromeanx             Signed value between 0 and 1
    Described below

tbodygyromeany             Signed value between 0 and 1
    Described below

tbodygyromeanz             Signed value between 0 and 1
    Described below

tbodygyrostdx              Signed value between 0 and 1
    Described below

tbodygyrostdy              Signed value between 0 and 1
    Described below

tbodygyrostdz              Signed value between 0 and 1
    Described below

tbodygyrojerkmeanx         Signed value between 0 and 1
    Described below

tbodygyrojerkmeany         Signed value between 0 and 1
    Described below

tbodygyrojerkmeanz         Signed value between 0 and 1
    Described below

tbodygyrojerkstdx          Signed value between 0 and 1
    Described below

tbodygyrojerkstdy          Signed value between 0 and 1
    Described below

tbodygyrojerkstdz          Signed value between 0 and 1
    Described below

tbodyaccmagmean            Signed value between 0 and 1
    Described below

tbodyaccmagstd             Signed value between 0 and 1
    Described below

tgravityaccmagmean         Signed value between 0 and 1
    Described below

tgravityaccmagstd          Signed value between 0 and 1
    Described below

tbodyaccjerkmagmean        Signed value between 0 and 1
    Described below

tbodyaccjerkmagstd         Signed value between 0 and 1
    Described below

tbodygyromagmean           Signed value between 0 and 1
    Described below

tbodygyromagstd            Signed value between 0 and 1
    Described below

tbodygyrojerkmagmean       Signed value between 0 and 1
    Described below

tbodygyrojerkmagstd        Signed value between 0 and 1
    Described below

fbodyaccmeanx              Signed value between 0 and 1
    Described below

fbodyaccmeany              Signed value between 0 and 1
    Described below

fbodyaccmeanz              Signed value between 0 and 1
    Described below

fbodyaccstdx               Signed value between 0 and 1
    Described below

fbodyaccstdy               Signed value between 0 and 1
    Described below

fbodyaccstdz               Signed value between 0 and 1
    Described below

fbodyaccjerkmeanx          Signed value between 0 and 1
    Described below

fbodyaccjerkmeany          Signed value between 0 and 1
    Described below

fbodyaccjerkmeanz          Signed value between 0 and 1
    Described below

fbodyaccjerkstdx           Signed value between 0 and 1
    Described below

fbodyaccjerkstdy           Signed value between 0 and 1
    Described below

fbodyaccjerkstdz           Signed value between 0 and 1
    Described below

fbodygyromeanx             Signed value between 0 and 1
    Described below

fbodygyromeany             Signed value between 0 and 1
    Described below

fbodygyromeanz             Signed value between 0 and 1
    Described below

fbodygyrostdx              Signed value between 0 and 1
    Described below

fbodygyrostdy              Signed value between 0 and 1
    Described below

fbodygyrostdz              Signed value between 0 and 1
    Described below

fbodyaccmagmean            Signed value between 0 and 1
    Described below

fbodyaccmagstd             Signed value between 0 and 1
    Described below

fbodybodyaccjerkmagmean    Signed value between 0 and 1
    Described below

fbodybodyaccjerkmagstd     Signed value between 0 and 1
    Described below

fbodybodygyromagmean       Signed value between 0 and 1
    Described below

fbodybodygyromagstd        Signed value between 0 and 1
    Described below

fbodybodygyrojerkmagmean   Signed value between 0 and 1
    Described below

fbodybodygyrojerkmagstd    Signed value between 0 and 1
    Described below
    
Codebook for the original dataset
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz.

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals).

These signals were used to estimate variables of the feature vector for each pattern: '-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ tGravityAcc-XYZ tBodyAccJerk-XYZ tBodyGyro-XYZ tBodyGyroJerk-XYZ tBodyAccMag tGravityAccMag tBodyAccJerkMag tBodyGyroMag tBodyGyroJerkMag fBodyAcc-XYZ fBodyAccJerk-XYZ fBodyGyro-XYZ fBodyAccMag fBodyAccJerkMag fBodyGyroMag fBodyGyroJerkMag

The set of variables that were estimated from these signals are:

mean: Mean value std: Standard deviation

All the values are means, aggregated over 30 subjects and 6 activities, hence the resulting dataset is 180 rows by 68 columns.

# Overview
• finding and extracting raw data
• today any how to make data tiny
• Raw data → processing script → tidy data → data analysis → data communication

##---------------------------------------------------
## Load both datasets and label them with feature names
##---------------------------------------------------

test <- read.table("./test/X_test.txt")
train <- read.table("./train/X_train.txt")
featname  <- read.table("features.txt", colClasses = "character")
featvec <- featname$V2
featvec <- tolower(featvec)
featvec <- gsub("\\()","",featvec)
featvec <- gsub("-","",featvec)
names(test) <- featvec
names(train) <- featvec
rm(featname,featvec)

##---------------------------------------------------
## Select columns of mean and std from the 561 columns
##---------------------------------------------------
a <- grep("mean",names(test))
b <- grep("meanfreq",names(test))
c <- grep("angle",names(test))
x <- setdiff(a,b)
colselectmean <- setdiff(x,c)
colselectstd <- grep("std",names(test))
test <- test[,c(colselectmean,colselectstd)]

a <- grep("mean",names(train))
b <- grep("meanfreq",names(train))
c <- grep("angle",names(train))
x <- setdiff(a,b)
colselectmean <- setdiff(x,c)
colselectstd <- grep("std",names(train))
train <- train[,c(colselectmean,colselectstd)]
rm(a,b,x,c,colselectstd,colselectmean)

##---------------------------------------------------
## Add activitylabel column to both the datasets
##---------------------------------------------------
testact <- read.table("./test/y_test.txt")
trainact <- read.table("./train/y_train.txt")
names(testact) <- "activitylabel"
names(trainact) <- "activitylabel"
test <- cbind(test, testact)
train <- cbind(train, trainact)
rm(trainact,testact)

##---------------------------------------------------
## Add descriptive names to content of activitylabel column
##---------------------------------------------------

test$activitylabel <- sub("1","walking",test$activitylabel)
test$activitylabel <- sub("2","walking_upstairs",test$activitylabel)
test$activitylabel <- sub("3","walking_downstairs",test$activitylabel)
test$activitylabel <- sub("4","sitting",test$activitylabel)
test$activitylabel <- sub("5","standing",test$activitylabel)
test$activitylabel <- sub("6","laying",test$activitylabel)

train$activitylabel <- sub("1","walking",train$activitylabel)
train$activitylabel <- sub("2","walking_upstairs",train$activitylabel)
train$activitylabel <- sub("3","walking_downstairs",train$activitylabel)
train$activitylabel <- sub("4","sitting",train$activitylabel)
train$activitylabel <- sub("5","standing",train$activitylabel)
train$activitylabel <- sub("6","laying",train$activitylabel)

##---------------------------------------------------
## Add subject column to both the datasets
##---------------------------------------------------

testsub <- read.table("./test/subject_test.txt")
trainsub <- read.table("./train/subject_train.txt")
names(testsub) <- "subject"
names(trainsub) <- "subject"
test <- cbind(test, testsub)
train <- cbind(train, trainsub)
rm(trainsub,testsub)

##---------------------------------------------------
## Merge both the datasets together 
##---------------------------------------------------

data <- rbind(test,train)
rm(test,train)

##---------------------------------------------------
## Find average values wrt subject and activity
##---------------------------------------------------

library(plyr)
library(dplyr)

act <- data %>% 
group_by(activitylabel,subject) %>% 
summarise_each(funs(mean))

write.table(act, "./tidyset.txt", row.names = FALSE)

##---------------------------------------------------
