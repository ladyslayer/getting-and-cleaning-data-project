# getting-and-cleaning-data-project
I have created a R program to clean and tidy the given data. I have been successful in obtaining clean and tidy data to help in future analysis by running the run_analysis.R code.

The data given represents data obtained from the accelerometers from the Samsung Galaxy S smartphone. 

There are three parts of my submission :
1. Readme.md which briefly describes the contents of this project
2. CodeBook.md Describes the data and process of tidying data.
3. run_analysis.R R program to implement the required tidying of data the output of which is submitted separately
It performs the following operations :
      Getting and Cleaning Data
      Merges the training and the test sets to create one data set.
      Extracts the measurements of mean and standard deviation for each measurement.
      Names the activities in the data set
      Labels the data set with descriptive variable names.
      Creates a second, independent tidy data set with the average of each variable for each activity and each subject.


To run the code and get the output follow these steps:
Unzip the source (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) into a folder on your local drive, say C:\Users\yourname\Documents\R\

Put run_analysis.R into C:\Users\yourname\Documents\R\UCI HAR Dataset\

In RStudio: setwd("C:\\Users\\yourname\\Documents\\R\\UCI HAR Dataset\\"), followed by: source("run_analysis.R")

Use data <- read.table("data_set_with_the_averages.txt") to read the data. It is 180x68 because there are 30 subjects and 6 activities, thus "for each activity and each subject" means 30 * 6 = 180 rows. Note that the provided R script has no assumptions on numbers of records, only on locations of files.
