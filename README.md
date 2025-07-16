# From Maps to Metrics: Analyzing Spatial Trends of Airbnb Listings in Bangkok – Data Analytics Project

## 1. Project Overview

This project aims to analyze the **geographic patterns of Airbnb listings in Bangkok**. Given Bangkok's status as a top tourist destination and the rapid growth of Airbnb, understanding the spatial dynamics of these rentals is crucial. We'll explore how listings are distributed, how property features like price and room type vary by location, and the relationship between location, property characteristics, and business performance. Our goal is to provide **actionable, location-based insights** for property owners, investors, and platform stakeholders, helping with everything from property placement to pricing strategies and ensuring a good balance of supply and demand. The project combines exploratory data analysis (EDA), geospatial visualization (using Folium & GeoJSON), and statistical comparisons to uncover spatial patterns and business implications of Airbnb operations in Bangkok.


### Key Objectives:

- **Map Geographical Distribution**: Pinpoint where Airbnb listings are concentrated and characterize those high-density areas.
- **Analyze Location-Based Features**: Understand how property attributes (like room type and price) are distributed across different locations.  
- **Identify Performance Relationships**: Uncover connections between property type, location, and key business performance metrics such as pricing and review counts. 

---

## 2. Data Sources

This project uses two primary datasets:

### 1. Airbnb Listings in Bangkok  
- Source: [Kaggle - Bangkok Airbnb Listings](https://www.kaggle.com/datasets/minemartin/bangkok-airbnb-listings/data)  
- Description: Contains listing-level data such as:
  - Room type
  - Price
  - Number of reviews
  - Availability (365 days)
  - Location coordinates (latitude & longitude)
  - Neighbourhood details
 
  #### Airbnb Listings Bangkok – Data Dictionary

| **Feature**                     | **Description** |
|--------------------------------|-----------------|
| `id`                           | Airbnb's unique identifier for the listing. |
| `name`                         | Name of the listing. |
| `host_id`                      | Airbnb's unique identifier for the host/user. |
| `host_name`                    | Name of the host. Usually, just the first name(s). |
| `neighborhood`                 | The neighborhood is geocoded using the latitude and longitude against neighborhoods as defined by open or public digital shapefiles. |
| `latitude`                     | Uses the World Geodetic System (WGS84) projection for latitude and longitude. |
| `longitude`                    | Uses the World Geodetic System (WGS84) projection for latitude and longitude. |
| `room_type`                    | Possible values: `Entire home/apt`, `Private room`, `Shared room`, `Hotel`. See detailed descriptions below. |
| `price`                        | Daily price in local currency. Note: `$` may be used regardless of actual currency. |
| `minimum_nights`               | Minimum number of nights required per booking. Subject to listing calendar rules. |
| `number_of_reviews`           | Total number of reviews the listing has received. |
| `last_review`                 | Date of the most recent review. |
| `calculated_host_listings_count` | Total number of listings that the host owns in this specific dataset scrape for the city/region. |
| `availability_365`            | Number of days the listing is available throughout the year, based on the host's calendar (including both bookings and blocks). |
| `number_of_reviews_ltm`       | Number of reviews received in the last 12 months. |

**Room Type Details:**

- **Entire place**: Guests have the entire space to themselves, including bedroom, bathroom, kitchen, and separate entrance. The host may or may not be on the property.
- **Private room**: Guests have a private bedroom but may share common areas with others.
- **Shared room**: Guests share the sleeping area and possibly other spaces with other people. Ideal for budget travelers.


### 2. GeoJSON: Bangkok District Boundaries  
- Source: [Kaggle - Bangkok Districts GeoJSON](https://www.kaggle.com/datasets/soeltanpasja/bangkok-districts)  
- Description:  
  Geospatial boundary file for administrative districts in Bangkok, used for mapping and choropleth visualizations.

---

## 3. Technologies Used

- **Programming Language**: Python 
- **Data Manipulation**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Geospatial Mapping**: Folium, JSON
- **Environment Control**: Warnings
- **Notebook Interface**: Jupyter Notebook
- **Version Control**: Git & GitHub
- **Documentation**: Markdown

---

## 4. Project Structure

```
├── README.md                <- Project overview and documentation
│
├── data
│   ├── raw/                 <- Original dataset (Airbnb Bangkok listings)
│   ├── cleaned/             <- Cleaned dataset after preprocessing steps
│   └── geojson/             <- Geojson Bangkok district boundaries
│
├── notebook/
│ └── From Maps to Metrics-Analyzing Spatial Trends of Airbnb Listings in Bangkok.ipynb <- Main notebook containing all analysis, visualizations, and insights
│
├── reports
│   ├── slide/               <- Presentation slides summarizing key findings
│   └── figures/             <- Saved figures used for reporting
│
├── docs/
│   └── data_dictionary.md   <- Description of all dataset features
│
└──  requirements.txt         <- Python dependencies for running the project

```

---

## 5. Summary of Findings

### 5.1 Business Insights

This analysis of Airbnb listings in Bangkok reveals actionable insights for stakeholders:

- **Location Strategy**: Focus on high-performing central districts like *Vadhana* and *Ratchathewi*, explore emerging areas with high guest engagement (e.g., *Pom Prap Sattru Phai*), and consider long-stay opportunities in low-competition zones such as *Lat Phrao*.

- **Pricing Optimization**: Hotel rooms yield the highest rates, while moderately priced listings in active neighbourhoods benefit from strong review volume — suggesting a balance of affordability and quality drives performance.

- **Operational Planning**: Availability varies significantly by district. Optimize calendars in saturated areas, and leverage high-availability districts for long-term rental strategies targeting digital nomads and extended stays.

### 5.2 Actionable Recommendations

To support data-driven decision-making for Airbnb stakeholders in Bangkok, this project suggests:

- **Invest Strategically**: Prioritize high-demand areas like *Vadhana* and *Ratchathewi*, while also exploring high-potential mid-priced districts such as *Pom Prap Sattru Phai*.

- **Price Smartly**: Set premium prices for hotel rooms and entire apartments in central zones, and adopt competitive pricing for private rooms in budget-friendly areas.

- **Optimize Availability**: In dense areas, keep calendars open year-round to boost visibility. In quieter districts (e.g., *Lat Phrao*), focus on long-term stays and stable occupancy.

- **Diversify Offerings**: Watch out for oversaturated districts and consider diversifying room types or bundling services to target niche audiences and stand out from the competition.

These actions can enhance profitability and guest experience through smarter use of location, pricing strategy, and operational planning.

---

## 6. Contact

**Name**: Rahma Sari Kusuma

**Email**: rahmasari17kp@gmail.com
