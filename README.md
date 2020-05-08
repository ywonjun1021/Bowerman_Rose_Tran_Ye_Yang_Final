# Analyzing Vacant Building Notices in Baltimore as an Indicator of Neighborhood Health

## Background and Business Question


## Data Questions
1. How many VBNs are being put back on the market, then end up back on the VBN list within 1-year increments over a 5-year period? Where is this most likely to occur?
2. Are there particular DHCD interventions – homeowner incentive grants, tax credits, etc. - that is more likely to keep a building off the VBN list?
3. How has the concentration of VBNs changed over time?
4. Is there a correlation between VBNs and Demolitions in a Neighborhood?
5. Are there any properties DHCD has spent capital on that then gets on the VBN list within five years?

## Data Answer and Visualizations
### VBN Reoccurence
In order to determine which properties were reappearing on the VBN list after being put back on the market, a unique ID was created for each address (e.g. 2110NFULTONAVE for the property at 2110 N. Fulton Ave.) and the dataset was organized first chronologically using the date of issue, "DateNotice," and then alpha-numberically using these IDs. The following IF statement was then used to count all properties which reoccurred in the dataset for reasons other than "Ownership Changed" - 

### DHCD Interventions

### VBN Concentration

### VBN and Demolitions Correlation

### VBN Reoccurrence and DHCD Capital

## Business Answer and Recommendations and Impact for Baltimore City
