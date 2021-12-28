## Release notes
### Date December 13th to January 7th <br>
Version number <br>
## What’s new  <br>
•	KPIs are no longer required <br>
Description: It's possible to leave the kpi array empty in the JSON configuration file. It will hide the KPI banner <br>
•	Implement New Congestion Algorithm <br>
Description: Congestion is caused by Values over Max value set in tuning  <br>
Total Congestion Value: sum of all values that are above max set value <br>
Total Count Value: sum of all touchpoints values <br>
Congestion Percentage = 100 multiplied by the total congestion Value divided by the total count value <br>
•	Ability to manage JSON version in NR1 Platform <br>
Description: Loading the old config into NerdStore with a key like pathpoint_config_[datetime_archived]Intro to NerdStorage UserStorageQuery Then in the UI we can provide a config history option that shows the versions. <br>
## Resolved issues 
•	Autofit Logo Image <br>
Description: Setting logo aspect ratio 3:1 <br>
## Known issues 
•	No changes <br>
•	Documentation changes No changes <br>
## Congestion Documentation 

A new way to calculate congestion is implemented, based on the formule developed. 
•	It uses the Count touchpoints, PCC and PRC
•	It adds a new property to the tuning, defining the max acceptable value. 
## "Max transaction Count” in the figure
<img src="images/Release_note.png" align=center width="1000" height="800" />

