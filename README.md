# data-512-a1

## Project Goal
The goal of this project is to construct and visualize Engligh Wikipedia traffic data from Jan 1 2008 to Aug 30 2019. Data is retrieved from two Wikipedia REST API endpoints:

Pagecount API documentation: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts

Pageview API documentation: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews

Data was gathered from the Wikimedia REST API, Wikimedia Foundation, 2018. CC-BY-SA 3.0
Wikimedia Foundation API Terms of Use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

The data is processed and a time-series chart is created as a result.

## Value Descriptions
The csv file 'en-wikipedia_traffic_200712-201809' has the following fields:

pageview_mobile_views: The combined mobile app and web views from the PageView API

pageview_desktop_views: The desktop views from the PageView API

pagecount_mobile_views: The mobile views from the legacy API

pagecount_desktop_views: The desktop views from the legacy API

pagecount_all_views: The combined desktop and mobile views for the legacy API

pageview_all_views: The combined desktop and mobile views for the PageView API

month: The recorded numeric month

year: The recorded year

# Other Considerations
Data from the Pageview API excludes spiders/crawlers, while legacy API data does not. This is why the numbers drop off as the switch happens.

Some months with a count of 0 have been excluded from the plot.

There is some overlap between the counts around May 2015 to July 2016.
