# Project 5: Brevet time calculator with Ajax and MongoDB

**Author: Jim Li**

**Contact Address: jinjiel@uoregon.edu**

## Description: 

Frequently, we get questions about how the ACP Brevet Control calculator algorithm works. The calculation is not as straightforward as it might seem.

The table below gives the minimum and maximum speeds for ACP brevets.

~~~
 Control location (km)	Minimum Speed (km/hr)	Maximum Speed (km/hr)
 0 - 200	            15	                      34
 200 - 400	            15	                      32
 400 - 600	            15	                      30
 600 - 1000	            11.428	              28
 1000 - 1300	            13.333	              26
~~~
The calculation of a control's opening time is based on the maximum speed. Calculation of a control's closing time is based on the minimum speed.

Distance, speed, and time calculation
When a distance in kilometers is divided by a speed in kilometers per hour, the result is a time measured in hours. For example, a distance of 100 km divided by a speed of 15 km per hour results in a time of 6.666666... hours. To convert that figure into hours and minutes, subtract the whole number of hours (6) and multiply the resulting fractional part by 60. The result is 6 hours, 40 minutes, expressed here as 6H40.

The calculator converts all inputs expressed in units of miles to kilometers and rounds the result to the nearest kilometer before being used in calculations. Times are rounded to the nearest minute.
