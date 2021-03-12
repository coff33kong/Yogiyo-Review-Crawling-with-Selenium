# Yogiyo-Review-Crawling-with-Selenium

## Version 1 

### Yogiyo-crawler

- Arguments for Crawler  
    - --order : required=False, default='distance'  
    option for restaurant list order  
    choose one -> [rank, review_avg, review_count, min_order_value, distance, estimated_delivery_time]')
    - --num : required=False, default=100  
    option for restaurant number
    - --lat : required=False, default=37.560873  
    latitude for search
    - --lon : required=False, default=126.9353833  
    longitude for search


- command  
    You can run the crawler with a command like the following:
    > python3 yogiyo-crawler.py --lat 37.5608 --lon 126.9353

    Geocoding is not done separately, so use Google Maps etc to find out your latitude and longitude.  
    By default, you will receive a list of 100 restaurants close to that location.  
    See options above to change.


- Structure of received data

    - Restaurant : Restaurant name
    - UserID : User ID, partially masked
    - Menu : Food name
    - Review : Review content
    - Total : Overall rating (5 out of 5)
    - Taste : Taste rating (5 out of 5)
    - Quantity : Quantity rating (5 out of 5)
    - Delivery : Delivery service rating (5 out of 5)
    - Date : Date of review
    - OperationTime : Restaurant operating hours
    - Address : Restaurant address

