# 📄 Data Documentation

## Dataset Overview

This project uses the **AB_NYC_2019** dataset, a publicly available dataset containing Airbnb listing information for New York City. The dataset includes details about listing locations, hosts, room types, pricing, availability, and customer reviews, making it suitable for exploratory data analysis and business intelligence applications.

## Source File

**Dataset Used:** `AB_NYC_2019.xlsx`

The dataset contains Airbnb listings from all five boroughs of New York City and provides information about hosts, pricing, booking availability, and customer interactions.

## Key Fields

| Field                          | Description                                                                              |
| ------------------------------ | ---------------------------------------------------------------------------------------- |
| id                             | Unique identifier for each Airbnb listing                                                |
| name                           | Name of the Airbnb listing                                                               |
| host_id                        | Unique identifier for the host                                                           |
| host_name                      | Name of the listing host                                                                 |
| neighbourhood_group            | Borough where the listing is located (Bronx, Brooklyn, Manhattan, Queens, Staten Island) |
| neighbourhood                  | Specific neighborhood within the borough                                                 |
| latitude                       | Geographic latitude of the listing                                                       |
| longitude                      | Geographic longitude of the listing                                                      |
| room_type                      | Type of accommodation (Entire home/apartment, Private room, Shared room)                 |
| price                          | Price charged per night                                                                  |
| minimum_nights                 | Minimum number of nights required for booking                                            |
| number_of_reviews              | Total customer reviews received                                                          |
| last_review                    | Date of the most recent review                                                           |
| reviews_per_month              | Average reviews received per month                                                       |
| calculated_host_listings_count | Number of listings managed by the same host                                              |
| availability_365               | Number of days the listing is available during the year                                  |

## Data Preparation

Before visualization, the dataset was processed in Tableau by:

* Filtering records with null or missing values where necessary.
* Creating calculated fields for analytical purposes.
* Organizing geographic information using neighbourhood hierarchies.
* Aggregating pricing information for borough-level comparisons.

## Dashboard Metrics

The dashboard analyzes:

* Average Price by Borough
* Geographic Distribution of Listings
* Price vs Reviews Per Month
* Neighborhood-wise Airbnb Performance

## Purpose of the Dataset

The dataset enables exploration of Airbnb market dynamics across New York City by combining pricing, location, and customer review information. It supports analysis of regional pricing strategies, customer engagement patterns, and geographic trends within the short-term rental market.

## Applications

The data can be used for:

* Market research
* Pricing strategy analysis
* Tourism analytics
* Real estate insights
* Geographic visualization
* Business Intelligence dashboards
* Exploratory data analysis

## Note

The dashboard focuses on providing a high-level overview of Airbnb market performance through spatial visualization and pricing analysis, enabling users to identify trends and compare neighborhoods efficiently using interactive Tableau visualizations.
