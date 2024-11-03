# Pricing and Discount Analysis of Top Men's Leather Jacket Brands
## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Data Collection and Preprocessing](#data-collection-and-preprocessing)
- [Analysis and Visualizations](#analysis-and-visualizations)
- [Key Findings](#key-findings)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [Conclusion and Future Work](#conclusion-and-future-work)
- 
## Project Overview

This project analyzes pricing and discount trends across different brands on  Myntra & Ajio. The goal is to uncover patterns in brand pricing, discount ranges, and product availability, providing insights into brand strategies and customer options.

## Objectives

-Identify price distribution of Men's Jacket
- Identify the average price and discount patterns by brand.
- Visualize the product count per brand and their discount distributions.
- Analyze pricing ranges and their correlation with brand discount percentages.
- 
- ## Dataset Description
- 
The dataset was sourced from [website source:Ajio, Myntra] through web scraping techniques. Key columns include:
- `Brand`: The name of the brand.
- `Name`: Product name.
- `Price`: Original price of the product.
- `Discount`: Discount applied on the product.
- ## Data Collection and Preprocessing

### Data Collection

Data was collected from AJIO's website using Selenium, a Python library for automating web interactions. The script visits each product page, scrapes key details, and saves the results in a CSV file. Here’s a detailed explanation of the data collection process:

#### Tools Used
- **Selenium**: A web automation tool that enables navigating websites, clicking buttons, and extracting data.
- Why selenium, over BeautifulSoup here:
- Selenium allows interaction with web pages that require JavaScript to load elements dynamically, making it suitable for e-commerce scraping.
- It can:
    Wait for elements to load (WebDriverWait).
    Click buttons to navigate (click()).
    Handle browser automation effectively.

- **Pandas**: A data manipulation library used here for saving data to CSV.

#### Purpose
The goal was to collect product information from the men's jackets and coats section on AJIO’s website. We gathered details like:
- **Brand**: The brand name of the product.
- **Name**: The specific name or title of the product.
- **Price**: The listed price of the product.
- **Discount**: The discount applied to the product, if any.

 ### Data Preprocessing
Cleaning: The dataset was cleaned by removing any missing values and standardizing column formats. Specifically, the "Discount" column was converted from a text format (e.g., "28% off") to a numeric format to allow for easier calculations and analysis.
