README
======

Project work for Getting and Cleaning Data offered by JHU on Coursera
Coursera_GaCD_PA
-----------------------------------------
Coursera - Getting and Cleaning Data - Peer Assesment


Overview
-----------------------------------------
One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data used in this project represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The purpose of the script in this repository is to

Create a single file containing all the train and test data (measures, activities, subject)
Construct an independent file which holds the averages of all the mean and std measures from the previous file by activity and subject for later analysis


Files in the repo
------------------------------------------
CodeBook.md: describes the variables, the data, and any transformations or work performed to clean up the data
README.md: short description of the repository contents
run_analysis.R: R script which creates the dataset containing train and test data, and the tidy dataset with average measure values


How To Use
------------------------------------------
Unzip the source data (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip or from the original site: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) into your actual working folder
Run the following command in R: source("run_analysis.R")


Ouput
------------------------------------------
The script generates two output tables:

"all_clean_data.txt": it contains all the test and train datasets (data, subjects, activities). The dimension of the file is 10299 x 69, and the size of it is ~ 8.4MB
"averages_by_activity_subject.txt": it holds the averages of all the mean and std measures from the previous file by activity and subject. The dimension of the file is 180 x 68, and the size of it is ~ 225kB


Performance
-------------------------------------------
The script normally runs about 30 seconds (it depends on your system's performance).
