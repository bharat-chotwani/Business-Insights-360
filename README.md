# Business Insights 360

## Project Overview

AtliQ Hardware, a fast-growing manufacturer and distributor of computers and peripherals, is adopting **Power BI** for advanced data analytics. Previously, the company relied on Excel for analysis, but this approach lacked the depth needed for strategic decision-making, leading to inefficiencies and financial losses—especially in the Latin American market.

To overcome these challenges, AtliQ Hardware launched the Business Insights 360 project, leveraging **1.8 million transaction records** from **Excel, CSV, and MySQL** to create a **Power BI dashboard** that provides:

- **Finance Analytics:** Profit & Loss statement to track financial performance.

- **Sales Insights:** Identify top/bottom customers and key sales metrics.

- **Marketing Analysis:** Evaluate product performance to refine strategies.

- **Supply Chain KPIs:** Assess efficiency using forecast accuracy, net error, and other key metrics.

- **Executive Dashboard:** A high-level summary for leadership decision-making.

- **Product Performance:** Highlight top/bottom 5 products based on GM% growth YoY and post-discount trends.

This project enables **data-driven decision-making** and helps AtliQ Hardware **stay competitive** in the market.

### [Business Insights Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiMWE4NzhjMDctMjk3Ni00MmFhLTlmM2QtYThiMTFmYjFiMmVlIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
### [Project Explanation](https://www.youtube.com/embed/IvlPC9Vq5sg?si)
### [Linkedin Post](https://www.linkedin.com/posts/bharatchotwani_business-insights-project-pdf-activity-7296173874465894400-zxXA?utm_source=share&utm_medium=member_desktop&rcm=ACoAADM4aokB6N7ZE70j2pv_sEK2dOUT-I2Lf6Q)

## Company Summary: AtliQ Hardware
AtliQ Hardware is a global company that manufactures and sells **computer hardware and accessories** like PCs, printers, USBs, and more. The company operates through three sales channels:

1. **Retailers** – Partners like **Croma, Best Buy, Amazon, and Flipkart** sell AtliQ products to consumers.
2. **Direct Sales** – AtliQ operates its own stores, including **AtliQ E-store** and **AtliQ Exclusive**.
3. **Distributors** – In some countries, government regulations require sales through distributors like **Neptune**.

### Why Analytics?
AtliQ Hardware recently faced unexpected losses in the U.S. market due to decisions based on surveys, intuition, and basic Excel analysis. Meanwhile, competitors use **advanced analytics** to drive their business decisions. To remain competitive, AtliQ is now building a **dedicated analytics team** to improve decision-making across key departments:

- **Finance** – Track revenue, profits, and financial performance.
- **Sales** – Identify top customers and sales trends.
- **Marketing** – Measure product performance and optimize campaigns.
- **Supply Chain** – Improve efficiency with key operational metrics.
- **Executive Insights** – Provide leadership with data-driven decision-making tools.
- **Product** – Analyze top and bottom-performing products to optimize growth and pricing strategies.

With **data analytics in Power BI**, AtliQ Hardware aims to transform its business strategy and ensure long-term success.

### Questions to Ask Before Building the Dashboard

1. What is the main goal of this Power BI dashboard?.
2. How will we measure the success of this project?
3. Do stakeholders want to see a preview before the final release?
4. What are the stakeholders’ expectations and concerns about this project?
5. Who will use this dashboard, and how will they use it?
6. What potential challenges might arise during development?
7. What data sources and resources are needed to build the dashboard?
8. Do stakeholders have any specific design or layout preferences?
9. What is the project deadline?
10. What do stakeholders expect to achieve by the end of this project?

After the project kickoff meeting, the data engineering team has provided the requested data. Let’s explore it.

### Dataset Understanding:
Understanding the available data is crucial before starting the analysis. This dataset consists of **dimension tables** (static data like customer and product details) and **fact tables** (transactional data).

1. **Customer Data**
- **74 customers** across **27 countries/markets**
- **209 stores** operating on two platforms:
   a. **Brick & Mortar:** Physical stores (e.g., Croma, Best Buy),
   b. **E-commerce:** Online stores (e.g., Amazon, Flipkart)

2. **Market Data**
- **27 markets** grouped into **7 sub-zones** across **4 regions**:
   a. APAC (Asia-Pacific)
   b. EU (Europe)
   c. NA (North America)
   b. LATAM (Latin America)
  
3. **Product Data**
- **3 divisions:**
   a. Networking & Storage (N & S)
   b. Peripherals & Accessories (P & A)
   c. PCs (Notebooks & Desktops)
- **6 segments** and **14 product categories** (e.g., Internal HDD, Keyboards)

4. **Fact Tables (Transactional Data)**
- **Fact Sales Monthly:** Sales quantities for each product.
- **Fact Forecast Monthly:** Predicted customer demand to improve planning and reduce storage costs.

5. **Additional Data Sources (Excel Files)**
- **Market Share:** Total sales data, including competitors (**737 records**)
- **Operational Expense:** Advertising, promotions, and operational costs (**113 records**)
- **NS GM Target:** Sales targets set by management for the current fiscal year (**321 records**)

This structured dataset allows for **detailed business analysis** across sales, marketing, finance, and supply chain operations.

## Data Model

![Data model](https://github.com/bharat-chotwani/Business-Insights-360/blob/badaa6eb919f231b20ab8a62a28901e49ad240e0/Data_Model_.png)

### What is Data Modeling?
- The process of organizing and structuring data to define relationships between tables.
- Helps in creating accurate reports and performing complex calculations.
- Ensures smooth data integration for better business intelligence and decision-making.

### Why is Data Modeling Important?
- Acts as the foundation of the report—every visual is built on the data model.
- Poor modeling can negatively impact report performance and accuracy.
- Following best practices is essential for efficient data analysis.

### Data Modeling Approach in This Project
- Uses **Star and Snowflake Schema** techniques for structuring data.
- Maintains a **one-to-many relationship** between tables.
- Implements the **Snowflake modeling method** for better data organization.

By following ***best practices in data modeling***, this project ensures a **reliable and high-performance** Power BI report.

## Tech Stacks
- Power BI Desktop
- Power BI Service
- SQL
- DAX
- DAX studio (for optimizing the report)
- Project charter file

## Technical Skills and Learning
- Identifying **key questions** to ask before starting the project.
- Understanding **data sources**, required transformations, and business needs.
- Ensuring proper **data validation techniques** before analysis.
- Performing **ETL processes** to clean and transform raw data.
- Creating a **separate date table** using Power Query (M Language).
- Extracting **fiscal year, months, and quarters** from given data.
- Establishing **one-to-many relationships** between tables using **Star & Snowflake Schema**.
- Incorporating **additional datasets** into the existing data model without issues.
- Creating **calculated columns** and **measures** using DAX.
- Using the **DIVIDE function** to prevent zero-division errors.
- Implementing **dynamic titles** based on applied filters.
- Utilizing **KPI indicators** to track performance metrics.
- Using **Bookmarks** to switch between visuals dynamically.
- Implementing **Page navigation with buttons** for better user experience.
- Applying **conditional formatting** using icons and background colors.
- Publishing reports to **Power BI Service**.
- Setting up **Personal Gateway** for automated data refresh.
- Creating and managing **Power BI Apps**.
- Managing **collaboration, workspaces, and access permissions**.
- Ensuring **efficient data modeling** to avoid slow performance.
- Optimizing **report loading time, file size, and data refresh speed**.

## Business 360 Project Overview

The **Home view** provides access to all available view buttons, allowing users to seamlessly navigate to a specific view page with a single click.

1. Info
2. Finance View
3. Sales View
4. Marketing View
5. Supply chain View
6. Executive View
7. Products
8. Support

### Home View
A source page providing easy page navigation access to all views, with dedicated support pane and information manual.

![Home View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Home.png)

### 1. Finance View
Enhances financial planning and cost control, featuring a Financial P&L (Profit & Loss) Statement, Net Sales Trend and Breakdown by Products/Customers and more.

![Finance View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Finance_view.png)

### 2. Sales View
Focuses on boosting sales revenue and tracking customer performance, including Gross Margin % Variance across Customers/Products and more.

![Sales View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Sales_view.png)

### 3. Marketing View
Elevates brand visibility and evaluates marketing campaign ROI, with insights into Segment Performance, Net Profit % Variance across Regions and more.

![Marketing View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Marketing_view.png)

### 4. Supply Chain View
Optimizes inventory management and demand forecasting, featuring trends in Forecast Accuracy and Inventory Stock Risk by Customers/Products.

![Supply Chain View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/supply_chain_view.png)

### 5. Executive View
Provides a high-level overview of organizational performance for top AtliQ executives and senior management, showcasing business KPIs, Revenue Contributions by Division/Channel, Top Customers & Products, AtliQ's Market Share Trend and more.

![Executive View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Executive_view.png)

### 6. Product View
Stakeholder's request to know the top 5 and bottom 5 products based on GM% Growth YoY and the post discounts % trend in tool-tip for each customer.

![Product View](https://github.com/bharat-chotwani/Business-Insights-360/blob/2f02f89ba0ba0ffd213d71aa49d3e8399c5c3731/Product_view.png)
