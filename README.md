The day.csv dataset contains daily aggregated bike-sharing system usage data. It records how many bikes were rented each day along with important environmental and seasonal factors that influence demand. This dataset is widely used in machine learning for regression, time-series analysis, and forecasting tasks.

Each row represents one day, and the dataset captures:

Date & time features (season, year, month, weekday)

Weather conditions (temperature, humidity, windspeed, weather category)

Operational indicators (holiday, working day)

Demand counts (casual users, registered users, total rentals)

This makes the dataset ideal for exploring how weather, seasonal trends, and day type affect bike rental usage.

Column Descriptions
1. instant

A unique record index for each day

Simply acts as a row number (1, 2, 3…)

2. dteday

Date of the record (YYYY-MM-DD)

3. season

Season of the year (categorical, encoded as numbers):

1 = Spring

2 = Summer

3 = Fall

4 = Winter

4. yr

Year of the record:

0 = 2011

1 = 2012

5. mnth

Month of the year (1–12)

6. holiday

1 = Holiday, 0 = Non-holiday
Indicates whether the day was a public holiday.

7. weekday

Day of the week (0–6), where:

0 = Sunday, 1 = Monday, …, 6 = Saturday

8. workingday

1 = Working day, 0 = Weekend or holiday
Indicates if it was a typical working day.

9. weathersit

Weather situation (categorical):

1 = Clear / Few clouds

2 = Mist / Cloudy

3 = Light Snow or Rain

4 = Heavy Rain / Ice (rare)

10. temp

Normalized temperature in Celsius

Ranges from 0 to 1 (actual temp × 41)

11. atemp

Normalized feeling temperature (“feels-like” temp)

Also ranges from 0 to 1

12. hum

Normalized humidity level

Values ≈ 0 to 1 (1 = very humid)

13. windspeed

Normalized wind speed

Values ≈ 0 to 1

14. casual

Number of casual users (non-registered customers) renting bikes that day

Usually higher on weekends

15. registered

Number of registered users (subscribed members) renting bikes

Usually higher on working days

16. cnt

Total bikes rented on that day

cnt = casual + registered# pandas_day
