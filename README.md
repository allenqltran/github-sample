# Capstone Project - Opening a Restaurant in Toronto

## Problem
Location, location, location. Similar to looking for a place to live, the location of a new business is the most important decision an entrepreneur can make, especially for a service industry such as a restaurant or hairstylist where people will generally not travel too far from their homes to go. Where would be a good place to start a new business? Where would be a good place to start a new franchise of an existing successful business? Specifically, this assessment is targeted to help entrepreneurs who want to open a new restaurant in the City of Toronto and are looking to answer the question of where best to open the restaurant and what type of restaurant to open.

Census data provides a wealth of information including family sizes, household income, ages, etc. This information can be used to group neighbourhoods and people with similar characteristics. Neighbourhoods with similar characteristics can then be used to compare what types of restaurants are prevalent in each area and what type of restaurants may be lacking representing a good opportunity for a new business. For example, if five out of six neighbourhoods that have a high percentage of young singles with high incomes shows a prevalence of Japanese restaurants, then a Japenese restaurant might be a good business to open in the sixth neighbourhood.

## Data

### Census Data
The Government of Canada's last census data was undertaken in 2016 and has been provided on the Statistics Canada website. The data can be obtained broken down by forward sortation areas (FSA), which is the first 3 characters of a Canada postal code, and thus allows for the grouping of information by neighbourhoods. However, all the pieces of information for each FSA is stored as name/value pairs and need to be transformed into tables that can be used for neighbourhood analysis. Also, certain FSA are not residential areas so they will need to be removed.

From the Canada-wide census data, a subset of this data from Toronto FSA's can be obtained. There are over 2000 data collected per FSA and a subset, specifically age gruops, family sizes, and household income will be used to group similar neighbourhoods. Because each FSA in Toronto will have different population sizes, a percentage distribution will give us a better measure of similarity amongs neighbourhoods.

### Restaurant (Venue) Data
Foursquare data will be used to obtain common venues for grouped Toronto neighbourhoods. This can then be used to analyze whether similar neighbourhoods have a lack of venue (restaurant) and hence a potential business opportunity.

#### Supporting Data
Geo coordinate information for the forward sortation areas of Toronto is also used to be able to visualize/map the results of the analysis.

A geojson file was also obtained to also help visualize the FSA areas of Toronto.
