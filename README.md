# 📊 Airbnb Listings Analysis Dashboard | Tableau

## 📌 Project Overview

This project presents an interactive **Airbnb Listings Analysis Dashboard** built using **Tableau** to explore pricing patterns, neighborhood trends, occupancy rates, and revenue insights across different Airbnb listings.

The dashboard combines calculated fields, hierarchies, maps, bar charts, line charts, and interactive actions to help users analyze listing performance and compare neighborhoods effectively. It demonstrates the use of Tableau's data visualization and analytical capabilities to transform raw Airbnb data into meaningful business insights.

The project aims to answer questions such as:

* How do listing prices vary across different neighborhood groups?
* What is the relationship between price and customer reviews?
* Which neighborhoods generate higher potential revenue?
* How does a listing's price compare with the average price in its neighborhood?
* What are the occupancy trends across different locations?

---

# 📂 Dataset Description

The dataset contains information about Airbnb listings, including pricing, availability, room types, neighborhood information, reviews, and host details.

## 📋 Key Fields Used

| Field Name                         | Description                                       | Data Type |
| ---------------------------------- | ------------------------------------------------- | --------- |
| **Neighbourhood Group**            | Major area where the listing is located           | Text      |
| **Neighbourhood**                  | Specific neighborhood of the listing              | Text      |
| **Room Type**                      | Type of accommodation offered                     | Text      |
| **Price**                          | Price charged for the listing                     | Number    |
| **Minimum Nights**                 | Minimum nights required for booking               | Number    |
| **Reviews Per Month**              | Average monthly reviews received                  | Number    |
| **Availability 365**               | Number of days the listing is available in a year | Number    |
| **Calculated Host Listings Count** | Total listings managed by the host                | Number    |

---

# 🛠️ Project Workflow

## 1️⃣ Data Preparation

* Imported the Airbnb dataset into Tableau.
* Filtered null values from important fields such as:

  * Price
  * Occupancy Rate
  * Minimum Nights
* Prepared the data for visualization and analysis.

## 2️⃣ Hierarchy Creation

Created custom hierarchies for better drill-down analysis:

### 📍 Neighbourhood Hierarchy

* Neighbourhood Group
* Neighbourhood

### 🏠 Room Type Hierarchy

A calculated field **Room Category** was created using IF-THEN-ELSE logic to classify listings into categories such as:

* Entire Home/Apt
* Private Room
* Shared Room

This field was then used to build the **Room Type Hierarchy**.

## 3️⃣ Calculated Fields

Several calculated fields were created to enhance analysis:

### Average Price per Night

```
Price / Minimum Nights
```

### Total Revenue

```
Price * Minimum Nights
```

### Occupancy Rate

```
Availability 365 / 365
```

### Price Difference (LOD Calculation)

Calculates the difference between an individual listing's price and the average price within its neighborhood using Tableau's Level of Detail (LOD) expressions.

---

# 📈 Visualizations Created

## 📉 Line Chart

Shows the relationship between:

* Price
* Reviews Per Month

to understand whether higher-priced listings receive more customer reviews.

## 🗺️ Interactive Map

Displays listings based on:

* Neighbourhood Group
* Neighbourhood

The map includes enhanced tooltips showing:

* Calculated Host Listings Count
* Price Difference
* Total Revenue
* Occupancy Rate

## 📊 Bar Chart

Compares **Average Price per Night** across different **Neighbourhood Groups**, making it easy to identify expensive and affordable locations.

---

# 🎛️ Interactive Dashboard Features

The dashboard includes several interactive components:

* Dynamic filters for cleaner analysis.
* Filter actions allowing users to select a **Neighbourhood Group** and view related information across visualizations.
* Highlight actions that emphasize listings belonging to the selected neighborhood group.
* Customized titles, labels, and annotations for improved readability.
* Rich tooltips providing additional listing details on hover.

---

# 🔍 Key Insights

* Average prices vary significantly across different neighborhood groups.
* Some neighborhoods consistently charge prices above the neighborhood average.
* Occupancy rates provide valuable insight into listing utilization throughout the year.
* Price and review patterns help identify customer preferences and market demand.
* Interactive filtering enables focused exploration of neighborhood-specific trends.

---

# 💻 Tools & Technologies Used

* Tableau Public / Tableau Desktop
* Calculated Fields
* Level of Detail (LOD) Expressions
* Hierarchies
* Interactive Maps
* Dashboards
* Filter Actions
* Highlight Actions
* Data Visualization Techniques

---

# 🎯 Conclusion

This Tableau project demonstrates how interactive dashboards can be used to analyze Airbnb listing data and uncover valuable insights into pricing, occupancy, and neighborhood performance. By combining calculated metrics, geographic visualizations, and user-driven interactions, the dashboard enables efficient exploration of the dataset and supports informed decision-making.

The project showcases practical Tableau skills including hierarchy creation, calculated fields, LOD expressions, dashboard design, and interactive analytics, making it a comprehensive example of business intelligence and data visualization.

