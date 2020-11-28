# coviddata
This is a personal repo to contain helpful scripts for exploring covid data

Scripts

rotateWeeklyDeaths.php - this script pulls the weekly death data from the CDC. The data by default has one row per week/region and then multiple columns for each cause of death. This script rotates it so that it has one row per week/region/cause of death and multiple columns for deaths for each year between 2015 and 2020. It also accounts for some slight changes in the column names between the historical file and the 2019/2020 file. It ignores 2014 because in the dataset that year contains 53 weeks of data instead of 52 like the other years. The script can output the data in csv or JSON format.

It uses the following data
- 2014-2018 deaths - https://data.cdc.gov/NCHS/Weekly-Counts-of-Deaths-by-State-and-Select-Causes/3yf8-kanr
- 2019-2020 deaths - https://data.cdc.gov/NCHS/Weekly-Counts-of-Deaths-by-State-and-Select-Causes/muzy-jte6
