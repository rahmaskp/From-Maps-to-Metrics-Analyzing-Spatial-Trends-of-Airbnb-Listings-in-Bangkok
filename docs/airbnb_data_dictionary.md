#### Airbnb Listings Bangkok – Data Dictionary

**Feature Descriptions**

`id`  
Airbnb's unique identifier for the listing.

`name`  
Name of the listing.

`host_id`  
Airbnb's unique identifier for the host/user.

`host_name`  
Name of the host. Usually, just the first name(s).

`neighborhood`  
The neighborhood is geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles.

`latitude`  
Uses the World Geodetic System (WGS84) projection for latitude and longitude.

`longitude`  
Uses the World Geodetic System (WGS84) projection for latitude and longitude.

`room_type`  
Possible values: `Entire home/apt`, `Private room`, `Shared room`, `Hotel`.

Details of room types:
- **Entire place**  
  Guests have the entire space to themselves, including bedroom, bathroom, kitchen, and separate entrance. The host may or may not be on the property and should disclose this.

- **Private room**  
  Guests have a private bedroom but may share common spaces (like bathroom or kitchen) with others.

- **Shared room**  
  Guests share the entire sleeping area and other spaces with other people. Ideal for budget travelers.

`price`  
Daily price in local currency. Note: `$` may be used regardless of actual currency.

`minimum_nights`  
Minimum number of nights required per booking. Subject to listing calendar rules.

`number_of_reviews`  
Total number of reviews the listing has received.

`last_review`  
Date of the most recent review.

`calculated_host_listings_count`  
Total number of listings that the host owns in this specific dataset scrape for the city/region.

`availability_365`  
Number of days the listing is available throughout the year, based on the host's calendar (including both bookings and blocks).

`number_of_reviews_ltm`  
Number of reviews received in the last 12 months.
