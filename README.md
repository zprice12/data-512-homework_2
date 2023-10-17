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
### thank_the_academy.AUG.2023.csv
This data file includes the articles we wish to investigate in this project. It includes a name field with the name of the article and a url field with a url to each article.
### academy_monthly_mobile_201507-202309.json
This data file includes monthly mobile page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
### academy_monthly_desktop_201507-202309.json
This data file includes monthly desktop page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
### academy_monthly_cumulative_201507-202309.json
This data file includes monthly cumulative page requests for each article. It involves an article field with the name of the article, a timestamp field with year and month, and a views field that represents the total monthly views for each article.
## Special Considerations
A forward slash in article titles will cause and error with the urllib function in the API call. This can be fixed by setting safe=''.
