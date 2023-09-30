# Contents
## data subdirectory
The R notebook ```CyclisticBike-ShareAnalysis.Rmd``` contains a code chunk
to create a data subdirectory and retrieve and store the 2022 (Divvy) bike-share
trip files in that directory.
To download them, simply set DOWNLOADED to False in the first imports code
chunk, and then run the "Retrieve Data" code chunk; there is also a subsequent
chunk which has code to rename the one file which is inconsistent in its
naming with the others.
The result is that data should contain 12 files (one per month) with a naming
convention of "2022MM-divvy-tripdata.csv" where MM is the 2 digit (zero padded)
representation of the month.

## Derived files
Running the remaining code in the R notebook will produce additional files:
- 2022-divvy-tripdata-V01.csv (an amalgamation of the 12 2022 files)
- 2022-divvy-tripdata-V02.csv (a cleaned version of the 2022 data)
- 2022-divvy-tripdata-V02.csv (a further cleaned and expanded version of
the 2022 data)

Refer to the ```DataChangelog.md``` file for more details.
