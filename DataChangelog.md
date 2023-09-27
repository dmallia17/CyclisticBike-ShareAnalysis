This file describes changes between the original Divvy Data and derived files.
Please refer to the DataREADME.md file for an abbreviated list of contents and
how to retrieve the Divvy data.

## V02 - 9/26/2023
An expanded and cleaned version of V01.
- **Added**:
    - ride_datetime (datetime format column based on started_at column),
        and columns derived from this: month (character), day(int),
        day_name(character), hour (int).
    - ride_length - integer difference in seconds between the end of a ride
    (ended_at) and the start of a ride (started_at)
- **Removed**:
    - Rows containing a ride_length less than 60 seconds (negative, zero or too
    little to be a real ride) (121089 rows)
    - Rows missing an end latitude and longitude (5856 rows)
- **Final dimensions**: 5,540,772 rows x 19 columns

## V01 - 9/24/2023
An amalgamation (concatenation) of the original 12 2022 Divvy files.
- **Final dimensions**: 5,667,717 rows x 13 columns