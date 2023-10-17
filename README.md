# Data 512 - Homework 2
## Project Goal
The goal of this project is to create informative tables to investigate Wikipedia article quality for states and regions across the US, considering potential bias throughout the project.
## Licenses and Links
Source Data License -  
https://creativecommons.org/licenses/by/4.0/  
Wikipedia Crawl -  
https://en.wikipedia.org/wiki/Category:Lists_of_cities_in_the_United_States_by_state  
Census Data -  
https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html  
Wikipedia US Regions -  
https://en.wikipedia.org/wiki/List_of_regions_of_the_United_States#Census_Bureau%E2%80%93designated_regions_and_divisions  
ORES Information -  
https://www.mediawiki.org/wiki/ORES  
Wikipedia Content Assessment -  
https://en.wikipedia.org/wiki/Wikipedia:Content_assessment  
MediaWiki API Information -  
https://www.mediawiki.org/wiki/API:Info
## Data Files
### state_pops.csv
This data file includes census data with each state's population. It includes a state field with the name of the state and a population field with the population of the state.
### us_regions.csv
This data file includes data on each state's region. It includes a DIVISION field with the regional division of the state and a STATE field with the name of the state.
### us_cities_by_state_SEPT.2023.csv
This data file includes the articles we wish to investigate in this project. It includes a state field with the name of the state, a page_title field with the name of the article, and a url field with a url to the article.
### wp_scored_city_articles_by_state.csv
This data file includes information on article quality for each of the articles. It includes a state field with the name of the state, a regional_division field with the region that article belongs to, a population field with the population of the state, an article_title field with the title of the article, a revision_id field with the revision version of the article, and an article_quality field with the ORES score for the article.
## Special Considerations
A forward slash in article titles will cause and error with the urllib function in the API call. This can be fixed by setting safe=''.
