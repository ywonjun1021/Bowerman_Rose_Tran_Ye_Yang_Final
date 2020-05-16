# Analyzing Vacant Building Notices and Improving Neighborhood Health in Baltimore

## Background and Business Question

Baltimore City wants to solve the problem of having high vacant building numbers 
Baltimore specifically has been demolishing the vacant buildings, but at the same time facilitating investments in vacant lot programs and supporting large-scale redevelopments in distressed areas. 

This matters for Baltimore citizens because Baltimore wants to better the city especially when they have many people with poor health conditions. If this problem of having high vacact buildings is fixed, overall neighborhood health might improve. 
This matters for us because as student at Johns Hopkins University, if this problem is fixed, there will be a ripple effect of fixing other problems in Baltimore; thus, making Baltimore a healthier and safer place.

Thus we ask: What are the main causes of Vacant Building Notices and what is the impact of DHCD interventions, regarding VBNs, on overall neighborhood health? Which strategies, if any, are most effective?


## Data Questions
1. How many VBNs are being put back on the market, then end up back on the VBN list within 1-year increments over a 5-year period? Where is this most likely to occur?
2. Are there particular DHCD interventions – homeowner incentive grants, tax credits, etc. - that is more likely to keep a building off the VBN list?
3. How has the concentration of VBNs changed over time?
4. Is there a correlation between VBNs and Demolitions in a Neighborhood?
5. Are there any properties DHCD has spent capital on that then gets on the VBN list within five years?

## Data Answer and Visualizations
### VBN Recurrence
* 5,938 VBNs were recurrences, of which 2,314 recurred five years or more after the initial VBN's close.
* The top __FIVE?__ neighborhoods where recurrences happened were __NEIGHBORHOODS__
* According to the cluster analysis, __PLACEHOLDER__
* Main takeaway

In order to determine which properties were reappearing on the VBN list after being put back on the market, a unique ID was created for each address (e.g. 2110NFULTONAVE for the property at 2110 N. Fulton Ave.) and the dataset was organized first chronologically using the date of issue, "DateNotice," and then alpha-numberically using these IDs. 92 VBNs had no street address attached and were excluded from this analysis. The following nested IF statement was then used to count all properties which recurred in the dataset for reasons other than "Ownership Changed."

VBN_Repeats = IF(G3=G2,IF[YEAR(I3)=YEAR(AD2),0,IF{M2="OWNERSHIP CHANGED",0,1}],0),

where 1 indicates a VBN recurrence, 0 is all other possibilities such as a new property or an extension of the preceding VBN, "VBN_Repeats" is the column heading, G3 is the unique ID of the property in question (row 3), G2 is the unique ID of the preceding property in the dataset (row 2), I3 is the issue date of the VBN in row 3, AD2 is the close date of the VBN in row 2, and M2 is the reason the row 2 VBN was closed.

This produced __6,661 results__. In a separate table, VLOOKUP was used to create a table of issue date and close date for each VBN recurrence, as well as those of the initial VBN issued for each property. The years elapsed between the initial close date and the issue date of each recurence were then calculated. For 722 VBN recurences, the years elasped were less than or equal to zero. Another recurence had no close date. Excluding these 723 properties, __5,938 VBN recurrences__ remained, of which __2,314 were reissued 5 years of more after the close of the initial VBN__. The top __FIVE?__ neighborhoods where recurrences happened were __NEIGHBORHOODS__.

___Concessions to be aware of: Inflation of years elapsed if initial VBN was cancelled due to ownership change and VBN was renewed before being officially abated/cancelled.___

Additionally, a cluster analysis of the VBN count per neighborhood was also performed. 

### DHCD Interventions
* Main takeaway
* Main takeaway
* Main takeaway

Explanation

### VBN Concentration
* Main takeaway
* Main takeaway
* Main takeaway

Explanation

### VBN and Demolitions Correlation
* Main takeaway
* Main takeaway
* Main takeaway

Explanation

### VBN Recurrence and DHCD Capital
* Main takeaway
* Main takeaway
* Main takeaway

Explanation

## Business Answer and Recommendations and Impact for Baltimore City
* Main takeaway
* Main takeaway
* Main takeaway

Explanation
