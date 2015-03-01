#Project Summary

##Data:
Available Data:
[1] DSNY Refuse and Recycling Disposal Networks - NYC Socrata
Says where each type of waste from each community board goes


DSNY Monthly Tonnage Data
Refuse collection by type, by community board


###Necessary Data:
| Garbage Dump Sites 	 | 
|------------------------|
| Location          	 |
| End use 				 |
| Transport cost per ton |
| Payment cost per ton 	 |
	

| Recycling Sites    	 		| 
|-------------------------------|
| Location          	 		|
| Type   				 		|
| End use 				 		|
| Transport cost per ton 		|
| Payment/purchase cost per ton |
	

###Schema Models:
| My Trash						|
|-------------------------------|
| Address [user input]		   	|
| Initial transfer station [1] 	|					
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
	

##User Experience:

1. Enter address
2. Routes are drawn for your waste, paper, and plastic recycling to its respective Transfer station through city streets. ⇐ data exists for this [1]
3. Routes are drawn from transfer stations to dump and recycling sites
4. A blurb appears:
..* “Your waste travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”
..* “Your paper recycling travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”
..* “Your plastic and glass recycling travels -distance- miles by -transport type(s)- to -end point- where it becomes -end use-”