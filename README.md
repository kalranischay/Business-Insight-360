# Business Insights 360

## Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

I worked on this project by following the Codebasics Power BI Course.

[Live Reporting Link](https://app.powerbi.com/view?r=eyJrIjoiNTU0MDcwM2YtMDkzZS00MDRlLWExOGYtODg1ZGQ2M2YyOGU2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Technology stack

- SQL
- Power Bi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project Charter File

## Power BI Techniques Learned
- What are all the questions that should be asked before starting the project?
- Creating calculated columns.
- Creating measures using DAX language.
- Data modeling.
- Using bookmarks to switch between two visuals.
- Page navigation with buttons.
- Using the divide function to prevent zero division errors.
- Creating date tables using M language.
- Dynamic titles based on the applied filters.
- Using KPI indicators.
- Conditional formatting of values in visuals using icons or background color.
- Data validation techniques.
- Power BI services.
- Publishing reports to Power BI services.
- Setting up a personal gateway to enable the auto-refresh of data.
- Power BI App creation.
- Collaboration, workspace, access permissions in Power BI services.
- And more...

## Business Related Terms
- Gross price.
- Pre-invoice deductions.
- Post-invoice deductions.
- Net invoice sale.
- Gross margin.
- Net sales.
- Net profit.
- COGS - Cost of Goods Sold.
- YTD - Year to Date.
- YTG - Year to Go.
- Direct.
- Retailer.
- Distributors.
- Consumer.

## Company Background
AltiQ Hardware is a company that has experienced significant growth in recent years and has expanded its business globally. It sells computers and computer accessories through three channels:

- Retailers
- Direct
- Distributors

Recently, the company incurred an unforeseen loss by opening a store in America. Based on surveys, intuition, and some Excel analysis, the company's competitors have a significant advantage with their analytics teams, enabling data-driven decision-making. Therefore, AltiQ Hardware has no choice but to build its analytics team for better survival in the industry.

During the project kickoff session, it's essential to clarify the project's objectives and address any questions related to the project.

## Questions to Ask Before Starting with the Dashboard
- What is the objective of building this Power BI dashboard?
- In what terms will the success of this project be measured?
- What will be the project's deadline?
- Do stakeholders expect a preview before the actual release?
- What are all the hopes stakeholders have for this project?
- What are all the fears the stakeholders have regarding building this dashboard?
- Who will be using this dashboard and for what purpose?
- What are all the expectations stakeholders have upon the completion of this project?
- What can go wrong while building this project?
- What are all the resources/data needed to build this dashboard?
- Is there any input from stakeholders regarding the design and views of the dashboard?
- After the project kickoff meetings, the data engineering team has provided the data as requested by the data analytics team. Let’s explore them.

## Dataset Understanding
Understanding the available data is crucial before analysis. Before diving into analysis, it's important to have a good understanding of the available data.

Dimension table: It contains static data such as customer and product details.

Fact table: It contains transaction data.

- gdb041:
    - dim_customer
          - 27 distinct markets (e.g., India, USA, Spain).
          - 75 distinct customers throughout the market.
          - 2 types of platforms:
            - Brick & Mortar - Physical/offline store.
            - E-commerce - Online Store (Amazon, Flipkart).
          - Three channels:
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - 27 distinct markets (e.g., India, USA, Spain).
        - 7 sub-zones.
        - 4 regions:
            - APAC
            - EU
            - NAN
            - LATAM
    - dim_product
        - Divisions:
            - P & A:
                - Peripherals
                - Accessories
            - PC:
                - Notebook
                - Desktop
            - N & S:
                - Networking
                - Storage
        - 14 different categories, such as Internal HDD, keyboard.
        - Different variants available for the same product.
    - fact_forecast_monthly
        - Used to forecast customer needs in advance, aiding in:
            - Higher customer satisfaction.
            - Reduced storage costs in warehouses.
        - The table is denormalized by the data engineering team for analytical work.
        - All dates of the month are replaced by the start date of the month.
        - Contains column names and forecasted quantity needed by the customer.
    - fact_sales_monthly
        - Similar to the fact_forecast_monthly table, but with sold quantities instead of forecasted values.
- gdb056:
    - freight_cost
        - Details of travel and other costs for each market with fiscal year.
    - gross_price
        - Details of gross prices with product code.
    - manufacturing_cost
        - Details of manufacturing costs with product code by year.
    - Pre_invoice_deductions
        - Details of pre-invoice deductions percentage for each customer by year.
    - Post_invoice_deductions
        - Details of post-invoice deductions and other deductions.

## Importing Data to Power BI
- As the database is MySQL in this project, we need to import the datasets from the MySQL database to Power BI by providing the database access credentials.

## Data Model
- Data modeling plays a vital role and is considered the foundation of a report. All visuals will be built upon the data model. 
- Poor data modeling can affect the overall performance of the report.
- Following good practices of data modeling is essential. In this project, we have followed the Snowflake data modeling method.

<img width="816" alt="image" src="https://github.com/kalranischay/Business-Insight-360/assets/42869655/591f2317-abe5-417f-af73-417158b3f810">

### Dashboard Design

Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

## Home View
![Home](https://github.com/kalranischay/Business-Insight-360/assets/42869655/b1d16c74-79cd-4071-b188-0be8c2a74a9a)

In the Home view, you'll find buttons to access all other views, the user will land on specific view page by clicking the button. 

- Information tab
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Support

## Finance View
![Finance View](https://github.com/kalranischay/Business-Insight-360/assets/42869655/01d2fad9-d811-4f9e-bf14-ed442b846fd2)

## Sales View
![Sales View](https://github.com/kalranischay/Business-Insight-360/assets/42869655/06888163-f40c-4655-9d6f-a697d312cfdc)

## Marketing View
![Marketing View](https://github.com/kalranischay/Business-Insight-360/assets/42869655/1e82de39-2490-46fe-984d-d8239906b934)

## Supply chain View
![Supply Chain View](https://github.com/kalranischay/Business-Insight-360/assets/42869655/c9222a93-9955-45cf-9e83-181680730b25)

## Executive View
![Executive View](https://github.com/kalranischay/Business-Insight-360/assets/42869655/6f35a41a-c37d-406c-81ea-6da68dfed149)

## Project Outcome

The report can be present insights and help finding answers to situation based questions and further help in the decision making process to stakeholders.
