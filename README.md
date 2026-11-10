# H&M Retail Sales & Customer Behavior Analysis

An interactive **Power BI business intelligence project** exploring
H&M's retail performance, product portfolio, customer behavior, and
sales patterns. The project combines transaction, customer, and product
information to turn raw retail data into actionable business insights.

> **Project type:** Data Visualization / Business Intelligence\
> **Tool:** Microsoft Power BI\
> **Analysis period covered in this report:** January--September 2020\
> **Dataset:** H&M Personalized Fashion Recommendations (Kaggle)

------------------------------------------------------------------------

## Table of Contents

-   [Project Overview](#project-overview)
-   [Business Objectives](#business-objectives)
-   [Dataset](#dataset)
-   [Dashboard and Analysis](#dashboard-and-analysis)
-   [Key Findings](#key-findings)
-   [Tools and Techniques](#tools-and-techniques)
-   [How to Access the Dataset](#how-to-access-the-dataset)
-   [How to Use This Project](#how-to-use-this-project)
-   [Limitations](#limitations)
-   [Acknowledgements](#acknowledgements)

------------------------------------------------------------------------

## Project Overview

This project analyzes H&M's retail business through multiple dimensions,
including sales channels, product categories, customer demographics,
product attributes, pricing, and membership status.

The report describes an analysis based on more than **11 million
transaction records**. It combines high-level KPIs with interactive
visualizations to examine both overall business performance and detailed
customer and product segments.

The Power BI report is organized into two main analytical views:

-   **Dashboard Overview** -- a high-level view of sales performance,
    product contribution, and sales patterns.
-   **Dashboard Insights** -- a deeper exploration of customer segments,
    average order value, membership activity, and product design
    preferences.

## Business Objectives

The project aims to:

1.  Monitor overall business performance through revenue, transaction
    volume, and customer KPIs.
2.  Compare revenue trends between online and physical-store sales
    channels.
3.  Understand revenue contribution across product categories and
    product types.
4.  Explore customer age distribution and differences between age
    groups.
5.  Identify leading products and understand the role of product design
    attributes such as color and pattern.
6.  Examine the relationship between price, sales volume, and revenue
    over time.
7.  Evaluate average order value (AOV) and purchasing activity across
    membership statuses.
8.  Translate analytical findings into recommendations for inventory,
    marketing, pricing, and customer retention.

## Dataset

The project is based on the public **H&M Personalized Fashion
Recommendations** dataset hosted on Kaggle.

### Main data files

  --------------------------------------------------------------------------
  File                       Description             Main analytical use
  -------------------------- ----------------------- -----------------------
  `transactions_train.csv`   Historical purchase     Sales trends, revenue,
                             records, including      quantity, channel
                             transaction date,       comparison
                             customer ID, article    
                             ID, price, and sales    
                             channel                 

  `customers.csv`            Customer attributes     Customer segmentation,
                             such as age and club    age distribution,
                             membership status       membership analysis

 `articles.csv`              Product metadata,       Product performance,
                             including product type, category contribution,
                             category, color,        design analysis
                             pattern, and department                            

  --------------------------------------------------------------------------

The original Kaggle dataset contains a broader transaction history. This
project report focuses on the 2020 analysis scope described in the
report, including monthly views from January to September. The dataset
may therefore need to be filtered and transformed before reproducing the
reported results.

### Dataset download

**Kaggle competition page:**\
https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data

You may need to sign in to Kaggle and accept the competition rules
before downloading the files.

For this Power BI analysis, start with the three CSV files listed above.
The product image archive is not required for the analyses described in
this report.

> **Important:** The original dataset is large. Do not upload raw data
> files to this GitHub repository unless you have checked their size,
> licensing terms, and sharing permissions. Download the data directly
> from Kaggle instead.

## Dashboard and Analysis

### 1. Sales Trends and Channel Comparison

A line chart compares monthly revenue from the **Online** and **Store**
channels.

The analysis examines: - Differences in revenue contribution between the
two channels. - Monthly fluctuations and notable peaks. - The
complementary roles of online and in-store shopping.

### 2. Revenue Contribution by Product Category

A **Sunburst chart** presents revenue hierarchically: - Inner ring: main
product categories (`index_name`). - Outer ring: product types
(`product_type_name`). - Segment size: revenue contribution.

This view helps identify the categories and product types that
contribute most to sales.

### 3. Customer Age Distribution

A line-and-area visualization explores the distribution of customers by
age.

It is used to identify: - Major age concentrations and secondary
peaks. - Age ranges with relatively fewer customers. - Potential
customer segments for targeted marketing and product planning.

### 4. Product Ranking and Design Preferences

Two complementary analyses are included:

-   **Top 10 products:** a horizontal bar chart ranks leading products
    by the selected sales measure.
-   **Pattern and color analysis:** a Treemap compares product design
    attributes, including `graphical_appearance_name` and
    `colour_group_name`.

These views help reveal leading product types and commonly purchased
design characteristics.

### 5. Price, Demand, and Revenue Over Time

An animated **Bubble Scatter Plot** with a monthly Play Axis examines
the relationship between: - Average price. - Total quantity sold. -
Total revenue, represented by bubble size. - Product category,
represented by color.

The animation supports comparisons across the months in the analysis
period.

### 6. Membership Status and Average Order Value

A **Combo Chart** combines: - Columns for Average Order Value (AOV). - A
line for transaction volume.

The analysis compares three membership statuses: - `PRE-CREATE` -
`ACTIVE` - `LEFT CLUB`

Considering AOV together with transaction volume helps distinguish high
spending per transaction from frequent purchasing activity.

### 7. Dashboard Overview and Insights

The report consolidates the analyses into two dashboard views:

-   **Overview:** business KPIs, sales-channel trends, product-category
    contribution, product ranking, and price-demand relationships.
-   **Insights:** customer scale, active membership, AOV, age
    distribution, and product design preferences.

Interactive selections allow users to explore segments and compare their
contribution to overall performance.

## Key Findings

The following findings are reported in the project analysis:

-   **Ladieswear** is the largest revenue-contributing category,
    accounting for approximately **47.5%** of the reported total.
-   **Divided** contributes approximately **21.1%**, while
    **Lingeries/Tights** contributes approximately **15.7%**.
-   Within Ladieswear, **Dress** and **Trousers** are among the leading
    product types.
-   Basic and solid designs, particularly neutral colors such as black,
    white, and beige, are prominent in the design analysis.
-   The Store channel contributes more revenue than the Online channel
    in the period discussed in the report.
-   The customer age distribution has a major concentration in the early
    twenties and a secondary concentration around the early fifties.
-   The report highlights a high level of purchasing activity among
    customers with `ACTIVE` membership status, despite their lower
    average order value compared with the other membership groups.

These are descriptive findings from the report and should not be
interpreted as proof of causal relationships.

## Tools and Techniques

-   **Microsoft Power BI** -- dashboard development and interactive data
    visualization.
-   **Power Query** -- data preparation and transformation within Power
    BI.
-   **DAX** -- KPI and analytical measure development.
-   **Data modeling** -- combining transaction, customer, and product
    information.
-   **Visualization techniques** -- line charts, Sunburst, horizontal
    bar charts, Treemap, animated Bubble Scatter Plot, and Combo Charts.

## How to Access the Dataset

1.  Open the [Kaggle H&M competition data
    page](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data).
2.  Sign in to your Kaggle account.
3.  Accept the competition rules if prompted.
4.  Download `transactions_train.csv`, `customers.csv`, and
    `articles.csv`.
5.  Extract the files and connect them to Power BI.
6.  Apply the same date scope and data transformations used in the
    project before comparing results.

Because the original files are large, consider using a filtered or
aggregated copy for local development. Keep the raw dataset outside Git.

## How to Use This Project

1.  Clone or download this repository.
2.  Download the required CSV files from Kaggle using the link above.
3.  Open the Power BI project file if it is included in the repository.
4.  If Power BI reports missing data sources, update the file paths in
    **Transform data → Data source settings**.
5.  Refresh the data model.
6.  Explore the report pages and interact with the visuals and filters.

> The Power BI report file may be distributed separately if its size
> exceeds GitHub's standard file-size limit. Check the repository
> contents for the available project files.

## Limitations

-   The analysis is primarily descriptive and visual; observed
    associations do not establish causation.
-   The report focuses on the date range and data scope stated in the
    analysis. Results may differ if the full original Kaggle dataset is
    used without applying the same filters and transformations.
-   Some interpretations of customer behavior are hypotheses based on
    observed distributions and should be validated with additional data.
-   The original dataset is subject to Kaggle's competition rules and
    terms. Users should review those terms before redistribution or
    commercial use.

## Acknowledgements

-   Dataset: [H&M Personalized Fashion Recommendations --
    Kaggle](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data)
-   Organization: Faculty of Mathematics and Computer Science,
    University of Science, VNU-HCMC.
-   Course: Data Visualization.

------------------------------------------------------------------------

*This project was developed for academic purposes as a data
visualization and business intelligence study of H&M retail data.*
