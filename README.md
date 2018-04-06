# Getting-and-Cleaning-data-project
Cleaning wearable computing dataset 

==================================================================
Human Activity Recognition Using Smartphones Dataset
Getting and Cleaning Data into tidier data
==================================================================
Originally by-Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Università degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws

Cleaned by-Aditya Gudal for the course Getting and Cleaning data by John Hopkins University(Coursera)
email-adityagudal29@gmail.com
==================================================================

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 
Dimension of the dataset named fit_set is 68 columns with 180 rows - Dimension(180x68)
The first column being the subject aka the volunteer,the second column being the activity label.
The rest of the columns are independent feature variables
The test aand training sets given were merged and then cleaned using different functions for reference please see the R_fit_analysis.R code as well as Codebook provided.
For each record it is provided:
======================================

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration for each dimension X,Y,Z JERKACC FOR EACH DIMENSION,
MAGNITUDE wherein the body as well as the gravity acceleration is taken into consideration.
- Triaxial Angular velocity from the gyroscope for each dimension X,Y,Z ,JERKGYRO, MAGNITUDE wherein the body as well as the gravity angular velocity(gyroscope readings) is taken into consideration.
- A 66-feature vector with time and frequency domain variables wherein fast fourier transform was used by using a butterworth(FIR) filter with a cutoff frequency of 0.3HZ
- Its activity label-'WALKING','WALKING_UPSTAIRS','WALKING_DOWNSTAIRS','SITTING','STANDING','LAYING' 
- An identifier(Volunteers) of the subject who carried out the experiment.
Total 30 Volunteers ,performed each action or activity given above

The dataset includes the following files:
Notes: 
======
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the text file.

For more information about this cleaned dataset contact: adityagudal29@gmail.com

License:
========
Use of this dataset in publications must be acknowledged by referencing the following publication [1] 

[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012

This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. Any commercial use is prohibited.

Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.
