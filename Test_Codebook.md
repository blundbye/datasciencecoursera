Codebook
========
This codebook describes the variables in the tab-delimited text file TidyData.txt.

Variables and descriptions
------------------------------

Variable name      | Description
-------------------|------------
SubjectID          | ID of the subject who performed the activity (range from 1 to 30).
Activity           | Activity name
Domain             | Time or frequency of domain signal (Time or Frequency)
Instrument         | Measuring instrument (Accelerometer or Gyroscope)
Acceleration       | Acceleration signal (Body or Gravity)
JerkFlag           | Jerk signal (yes or no)
MagnitudeFlag      | Magnitude of the signals calculated using the Euclidean norm (yes or no)
MeasureType        | Type og measure (Mean or Standard Deviation)
AxialDirection     | Direction of 3-axial signals (X, Y, or Z)
AverageValue       | Average of each measure for each activity and each subject
NumberObservations | Count of observations used to compute `average`

Dataset structure
-----------------

```{r}
str(TidyData)
```

```
## Classes ‘data.table’ and 'data.frame':	11880 obs. of  11 variables:
## $ SubjectID         : int  1 1 1 1 1 1 1 1 1 1 ...
## $ Activity          : chr  "LAYING" "LAYING" "LAYING" "LAYING" ...
## $ Domain            : Factor w/ 2 levels "Time","Frequency": 1 1 1 1 1 1 1 1 1 1 ...
## $ Acceleration      : Factor w/ 3 levels NA,"Body","Gravity": 1 1 1 1 1 1 1 1 1 1 ...
## $ Instrument        : Factor w/ 2 levels "Accelerometer",..: 2 2 2 2 2 2 2 2 2 2 ...
## $ JerkFlag          : Factor w/ 2 levels "No","Yes": 1 1 1 1 1 1 1 1 2 2 ...
## $ MagnitudeFlag     : Factor w/ 2 levels "No","Yes": 1 1 1 1 1 1 2 2 1 1 ...
## $ MeasureType       : Factor w/ 2 levels "Mean","Standard Deviation": 1 1 1 2 2 2 1 2 1 1 ...
## $ AxialDirection    : Factor w/ 4 levels NA,"X","Y","Z": 2 3 4 2 3 4 1 1 2 3 ...
## $ AverageValue      : num  -0.0166 -0.0645 0.1487 -0.8735 -0.9511 ...
## $ NumberObservations: int  50 50 50 50 50 50 50 50 50 50 ...
## - attr(*, "sorted")= chr  "SubjectID" "Activity" "Domain" "Acceleration" ...
## - attr(*, ".internal.selfref")=<externalptr> 
```
 
