## Sintec's Competitor Sales Analysis in Power BI
**Datacamp Case Study**
<br/>
<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/9fc4117a-66d9-4e9f-bcb4-90bbe03954a0" style="width:100px;"/> x
<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/bb546968-c01c-4344-a204-65a164f0e699" style="width:100px;height:100px;"/>

*Check out the PowerBI tools I used: [PowerBI-Tools-Used](/PowerBI-Tools-Used.md/)*

This document showcases a comprehensive competitor sales analysis project completed in Power BI. The analysis focused on Sintec's performance against competitors in the USA and internationally.

### Data Exploration and Transformation

The project began by exploring a dataset containing sales information for various manufacturers. This data was structured across several tables, including fact and dimension tables, ultimately forming a snowflake schema.

**Raw Data State**
<br/>
*Product Table*
<br/>
<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/5d1f7321-83b7-4fd9-ba83-018c3f49b4c6" style="width:500px;"/>
<br/> *& Sales Table*<br/>
<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/bde199ca-78eb-4005-abb0-05ed9906b51b" style="width:500px;"/>


**Data Cleaning and Transformation:**

* Data was imported into Power Query Editor.
* Unnecessary columns were removed.
* Null values were addressed in relevant columns.
* Data types were adjusted (e.g., Zip code from number to text).
* New calculated columns were created (e.g., separating currency and price, creating a unique key using Zip and Country).
* International sales data was appended to the main sales table.
* Data was filtered to include only years 2019-2021.

### Data Modeling and Relationships

Data modeling played a crucial role in establishing connections between tables.

* A calculated column, "ZipCountry," was created in both the Geography and Sales tables to enable a relationship.
* A "Date" table was created using the CALENDAR function to provide a date dimension.
* Relationships were established between Geography and Sales, between Date and Sales, and indirectly between manufacturer and sales.

<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/5fa42de4-6693-4a61-b0fe-90fe225c4cb6" style="width:600px;"/>
<h1> 👇
<br/>
<br/>
<img src="https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/8f56388e-8ab1-4ace-8879-5fc8651a383f" style="width:600px;"/>



### Discovering Sales Trends and Insights

**DAX Calculations and Measures:**

* Measures were created to calculate revenue share across regions, identify top-selling manufacturers, and visualize sales growth.

**Visualizations:**

* Stacked column charts displayed revenue by country with manufacturer legends.
* Line graphs depicted revenue over time (quarters per year).
* Slicers for manufacturer and date were implemented for interactive exploration.
* Category hierarchies were created within the product table for deeper analysis.
* A gauge visualized total revenue with year-over-year growth.

### Sharing Market Analysis
* Sintec held a 38.22% market share in the USA.
* Sintec achieved the highest growth rate (18.8%) in 2021 compared to the previous year.
* Artisans captured over 50% of the German market share, while Sintec held 21.25% globally.

#### PowerBI Dashboards

![Sintec 1](https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/93506b7b-95b0-442b-b9c5-978f6d756e72)
![Sintec 2](https://github.com/lukbos/PowerBI-Competitors-Sales-Analysis/assets/97811417/6ca682f3-a4fc-4eaa-8d45-ffbe10909d65)

