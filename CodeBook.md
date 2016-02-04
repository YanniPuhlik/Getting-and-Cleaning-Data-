
This CodeBook describes the Values of the Project Variables, the Course Project Data, as well as Transformations and Work Performed to Clean-up the Data called CodeBook.md.

Values of Project Variables (please refer to greater details on each of the variables in run_analysis.R and the README.md file in this repro)

  Values of Variables Activity consist of data from "Y_train.txt" and "Y_test.txt"
  Values of Variables Subject consist of data from "subject_train.txt" and subject_test.txt"
  Values of Variables Features consist of data from "X_train.txt" and "X_test.txt"
  Names of Variables Features comes from "features.txt"
  Levels of Variable Activity comes from "activity_labels.txt"

  Details of the files that will be used to load data are listed as follows:
  
  'README.txt'
  
  'features_info.txt': Shows information about the variables used on the feature vector
  
  'features.txt': List of all features
  
  'activity_labels.txt': Links the class labels with their activity name
  
  'train/X_train.txt': Training set
  
  'train/y_train.txt': Training labels
  
  'test/X_test.txt': Test set
  
  'test/y_test.txt': Test labels
  

*Notes 1. 
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the text file.


Transformation and Work Performed to Clean-up the Data

  1. The Activity, Subject andFeatures were used as part of descriptive variable names for data in the data frames
  2. Read data from the files into the variables
  3. Read the Activity files
  4. Read theSubject files
  5. ReadFeatures files
  6. Looked at the properties of each of the variables
  7. <em> Project step #1</em> Merged the training and the test sets to create one data set
  8. Merged the data tables by rows
  9. Set names to variables
  10. Merged columns to get the data frame data for all Data
  11. <em>Project step #2</em> Extracted only the measurements on the mean and standard deviation for each measurement
  12. Subset the data frame data by selected names of Features
  13. Checked the structures of the data frame Data
  14. <em>Project step #3</em> Used descriptive activity names to name the activities in the data set
  15. Read descriptive activity names from "activity_labels.txt"
  16. Factorized variable activity in the data frame data using descriptive
    activity names check
  17. <em>Project step #4<em/> Appropriately labeled the data set with descriptive variable names
    19 Listed names of Features were labeled using descriptive variable names
  18. Data set -- replaced by -- Descriptive variable names
  19. Conducted names check
  20. <em>Project step #5<em/> Created a second, independent tidy data set and output it
  21. Conducted Data Reshaping with (reshape2) and (melt)
  22. Completed with library(knitr)
  23. Created Codebook with knit2html(input="run_analysis.R", output="codebook.Rmd")

