#Project Summary

Where's My Waste is designed to show New Yorkers what happens to their trash and recycling after Sanitation Workers pick it up from the curb. After waste is dropped off at a transfer station, it is brought to places around the metro area as far away as Virginia. New York City must pay for the trash's transportation, and to deposit it at most dump sites, at a cost to the tax payer. The more waste New Yorkers divert into recycling and compost, the more money the city will save.

##User Experience:
1. Enter address
2. Routes are drawn from the user's location to the respective transfer stations for waste and recycling through city streets. ⇐ [1](https://data.cityofnewyork.us/City-Government/DSNY-s-Refuse-and-Recycling-Disposal-Networks/kzmz-ivhb)
3. Routes are drawn from transfer stations to dump and recycling sites in New York and out of state.
4. A blurb appears:
..* “Your waste travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”
..* “Your paper recycling travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”
..* “Your plastic and glass recycling travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”

##Data:
###Available Data:
[DSNY Refuse and Recycling Disposal Networks - NYC Socrata](https://data.cityofnewyork.us/City-Government/DSNY-s-Refuse-and-Recycling-Disposal-Networks/kzmz-ivhb)
Shows where each type of waste from each community board goes

[DSNY Monthly Tonnage Data](https://data.cityofnewyork.us/City-Government/DSNY-Monthly-Tonnage-Data/ebb7-mvp5)
Refuse collection by type, by community board

###Necessary Data:
| Garbage Dump Sites 	 | 
|------------------------|
| Location          	 |
| End use 		 |
| Transport cost per ton |
| Payment cost per ton 	 |
	
| Recycling Sites    	 		| 
|-------------------------------|
| Location          	 		|
| Type   				|
| End use 				|
| Transport cost per ton 		|
| Payment/purchase cost per ton |

###Schema Models:
| My Trash						|
|-------------------------------|
| Address [user input]		   	|
| Initial transfer station [1](https://data.cityofnewyork.us/City-Government/DSNY-s-Refuse-and-Recycling-Disposal-Networks/kzmz-ivhb) 	|					
| End point						|
| End use					 	|
| Total distance				|	
| Total cost per ton			|		
| Transport types				|	
	
| Transport types |
|-----------------|
| Truck			  |
| Barge			  |
| Train			  |

##Additional Information
###Resources
[NYC Department of Sanitation](http://www1.nyc.gov/site/dsny/index.page)
[Where Does New York City's Trash Go? | Living City | The New York Times](https://www.youtube.com/watch?v=Y6LzB6rMDtA)
