# Miniproject 2

### [Assignment](assignment.md)

## Project/Goals
    Use recommendation apps (Foursquare, Yelp) on local business to explore the quality and type of local businesses and restaurants

## Process
    Access the API of the respective sites and store the data (json files)
    Clean up the data so it is somewhat readable, then store in a Pandas dataframe
    Put results in SQLite3 database and retrieve for exploratory data analysis

## Results
Both services provide basic information about local businesses (e.g. name, address, location) 

Foursquare has has non-restaurants listed (e.g. tattoo parlors), and you can perform a separate query for "tips", which are mini-reviews about a business (an example from a local brewery: 'Good brewery with nice sours and citrus forward IPAs. Friendly and helpful staff. Good space, but gets crowded.')

Yelp only provides data about restaurants (at least from my search), as well as a rating, in increments of 0.5.

## Challenges 
Learning curve accessing and cleaning the data, and familiarization of software tools.
About 5% of time was spent doing the Exploratory Data Analysis that was the focus of the mini-project   

Giving tables consistent properties so they can be joined and data from each API can be aggregated for a given business 
...which I finally got to, about 25 minutes before we began

## Future Goals
Connect Yelp’s Tips API, which are mini-reviews about a business.  
- an example from a local brewery: 'Good brewery with nice sours and citrus forward IPAs. Friendly and helpful staff. Good space, but gets crowded.'

Connect additional APIs to get more information (e.g. Google Maps, Untappd)
- Make more queries
- Limit of 50 results per query 
- Slightly changing the start coordinates can produce completely unique results; certain parameters can also offset this (i.e. the offset parameter)
- Making more queries will give more unique business results