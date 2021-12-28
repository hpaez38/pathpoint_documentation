## Release notes
### Date December 13th to January 7th <br>
Version number <br>
## What’s new  <br>
- ***KPIs are no longer required***<br>
Description: It's possible to leave the kpi array empty in the JSON configuration file. It will hide the KPI banner <br>
- ***Implement New Congestion Algorithm*** <br>
Description: Congestion is caused by Values over Max value set in tuning  <br>
Total Congestion Value: sum of all values that are above max set value <br>
Total Count Value: sum of all touchpoints values <br>
Congestion Percentage = 100 multiplied by the total congestion Value divided by the total count value <br>
- ***Ability to manage JSON version in NR1 Platform*** <br>
Description: Loading the old config into NerdStore with a key like pathpoint_config_[datetime_archived]Intro to NerdStorage UserStorageQuery Then in the UI we can provide a config history option that shows the versions. <br>
## Resolved issues 
- ***Autofit Logo Image*** <br>
Description: Setting logo aspect ratio 3:1 <br>
## Known issues 
- ***No changes*** <br>
- ***Documentation changes No changes*** <br>
## Congestion Documentation 

A new way to calculate congestion is implemented, based on the formule developed. 
- ***It uses the Count touchpoints, PCC and PRC***<br>
- ***It adds a new property to the tuning, defining the max acceptable value.*** <br>
## "Max transaction Count” in the figure <br>
<img src="images/TransactionsCount.png"> <br>
- ***It is required at least 2 count touchpoints in a stage for the formule to work.***<br> 
It is defined that a touchpoint is congested when its value is over the max defined in the tuning, the more it is over that value, the more congested the touchpoint is.<br> 
***Example:*** <br>
In the graphic it is shown in red all the values generating congestion<br>
<img src="images/Example_graphic.png"> <br>
***Formula***<br>
What is causing Congestion: Values over Max value set in tuning <br>
- ***Total Congestion Value:	 Sum of all values that are above max set value*** <br>
- ***Total Count Value: Sum of all touchpoints values*** <br>
- ***Congestion Percentage = Hundred multiplied by the total congestion Value divided by the total count value*** <br>
<img src="images/Formula.png"> <br>
