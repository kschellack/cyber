[Go back to Readme](./README.md)


# Project:  Build an application that will
# allow monitoring of power production


## This project is a very practical in that it provides further insight to my solar system. 
## As PGE will continue to shut off power, I will be able to view, with granular detail,
## the energy production of the solar system (soon to have a battery attached). 

## It represents a collective summarization of the recent eight classes I have taken
## at Sierra in Applied Computer Science, Networking 
## and (some) security.

Solar system was installed in April 2018. Happily, at the end of the first year, my total PGE bill was $150. The minimum monthly bill is $10.00. The solar project was a success. The below picture was taken on a rainy day (today), but shows the data available (251.8 watts is enough to run a few incandescent lights).

![Test Image 1](C:\Users\Administrator\Pictures\inverter)

 
PGE published solar energy data quantized hourly. The below spreadsheet is a sample of PGE solar energy posted in November 2019. The rightmost numbers is the month to data accumulative power. Positive numbers mean I generated more than I used…..please note that the numbers are negative in July and August when the AC is running   ;-) .

 

The project idea was to capture the data posted from the inverter and put it in a file. That file was to be manipulated in Excel and published in graphical and tabular format. 

Project information sources >>>>>  SolarEdge (the inverter manufacturer) and jbuehl/solaredge (on githup). Unfortunately, the project got deeper and more time consuming than I thought it would. I thought it would be as simple as opening the inverter, connecting to the RJ-45 jack and running 50ft of cat 5E cable.  This was not to be.

The pieces in progress are:

1) getting an internet connection from the inverter to SolarEdge, this will allow some data collection
2) working with SolarEdge to determine the limits of the data collection
3) investigating the information published on Github by jbuehl

I was given a “get out of jail” opportunity (by instructor, Jared). That is to learn and use CSV (comma separated values) to represent, manipulate and publish the data I have already accumulated.

CSV is a pragmatic data representation format as it is simply a flat, text file. It can be read with Notepad and has methods / objects that can read, modify and write to the CSV file. In addition, applications like Excel have options that can easily save a spreadsheet (workbook) in “comma delimited format”. Below is a sample of my spreadsheet data in CSV format.

  


Using the Idle Python Shell. The below commands show a non-formated version of the CSV file.

 

Creating a file (.py) and running it did not show the same result.

