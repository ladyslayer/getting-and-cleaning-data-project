The attached R script (run_analysis.R) performs the following to clean up the data:

Merges the training and test sets to create one data set, namely train/X_train.txt with test/X_test.txt, the result of which is a 10299x561 data frame, as in the original description ("Number of Instances: 10299" and "Number of Attributes: 561"), train/subject_train.txt with test/subject_test.txt, the result of which is a 10299x1 data frame with subject IDs, and train/y_train.txt with test/y_test.txt, the result of which is also a 10299x1 data frame with activity IDs.

Reads features.txt and extracts only the measurements on the mean and standard deviation for each measurement. The result is a 10299x66 data frame, because only 66 out of 561 attributes are measurements on the mean and standard deviation. All measurements appear to be floating point numbers in the range (-1, 1).

Reads activity_labels.txt and applies descriptive activity names to name the activities in the data set:

  walking  
  
  walkingupstairs  
  
  walkingdownstairs  
  
  sitting  
  
  standing  
  
  laying  
The names of the attributes are the following:

  tbodyacc-mean-x   
  
  tbodyacc-mean-y   
  
  tbodyacc-mean-z   
  
  tbodyacc-std-x  
  
  tbodyacc-std-y  
  
  tbodyacc-std-z  
  
  tgravityacc-mean-x  
  
  tgravityacc-mean-y  
Finally, the script creates a 2nd, independent tidy data set with the average of each measurement for each activity and each subject. 
