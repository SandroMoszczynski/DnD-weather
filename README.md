Weather Simulator python;
--------------------

This is a small script that looks up values from a csv file and outputs them from command line. Requires numpy and argparse in python, written for python 3.7.

Usage
-----

The script can be activated from command line by calling: 

python weather.py MONTH DATE

where MONTH is saved in the table by proper names, but supports abreviations such as jan, feb, mar etc...

where DATE is the integer value of the day desired

an example of the usage would thus be:

python weather.py nov 25

which would return the weather conditions and light levels of the day in question.

Features
--------

- Has daylight times for regions above the arctic cirlce, thus can tell when the day will start, end and how much daylight, if any, will be available for the group. 
- Will give the day a random chance of rain, whicch if the temperature is cold enough will turn to snow. This will lower the temparature further.
- Will simulate wind for a day through a random roll aswell, which can compound with precipitation to give storms and further decrese the average temp for the day.
- Random temperature based on weather conditions and average temperature for the region on given date will also output.
- All region types are based on Finnish weather and day/night cycles of the Lapland region. Thus precipitation is set to an average 25% year round.