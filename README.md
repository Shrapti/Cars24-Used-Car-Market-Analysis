Cars24: Used Car Market Analysis & Price Intelligence
A Python-Based Web Scraping and Used Car Price Analysis Project

Developed by: Shrapti Bedre
1. Project Overview
Cars24: Used Car Market Analysis & Price Intelligence is a Python-based
web scraping and data analysis project designed to explore used-car
listings and understand the factors associated with their listed prices.

The project collects available vehicle listing information from the
Cars24 used-cars page. Python libraries are used to inspect the website
response, parse its HTML content, identify relevant embedded listing
data, and extract vehicle attributes into a structured dataset.

The collected data is then organized using Pandas and examined through
data inspection and exploratory analysis. The project focuses on
attributes such as car brand, model, manufacturing year, fuel type,
transmission, kilometres driven, ownership, and listing price.

The current notebook extracts 10 car listings. This is an initial
sample for demonstrating the data collection and analysis workflow, not
a representative sample of the entire used-car market.
2. Project Objectives
- Collect used-car listing information from the Cars24 website.
- Understand the structure of website HTML and embedded page data.
- Extract relevant vehicle details using Python and regular
  expressions.
- Convert extracted information into a structured Pandas DataFrame.
- Export the collected records into a CSV dataset.
- Inspect dataset dimensions, data types, missing values, and
  duplicates.
- Check for invalid listing prices.
- Create derived variables such as car age and price in lakhs.
- Explore used-car prices across available vehicle attributes.
- Communicate observations through data analysis and visualizations.
3. Data Source
Source: Cars24 Used Cars
Website: https://www.cars24.com/buy-used-cars/\
Data Collection Method: Python-based web scraping and extraction
from embedded page content.

The project accesses the Cars24 used-cars page and inspects the returned
HTML and embedded scripts to locate available vehicle listing
information.

The extracted dataset includes:
- Car name
- Brand and model
- Manufacturing year
- Fuel type
- Transmission type
- Kilometres driven
- Ownership
- Listing price
Note: Website content and listing availability may change over time.
The current extraction logic depends on the page structure and embedded
data available when the notebook is executed.
4. Technologies and Libraries
  Technology                          Application
  Python                              Core programming language

  Requests                            Sending HTTP requests and
retrieving webpage content

  BeautifulSoup                       Parsing HTML content

  Regular Expressions (re)          Extracting listing attributes from
embedded page content

  Pandas                              Creating, cleaning, and analyzing
tabular data

  NumPy                               Numerical operations

  Matplotlib                          Data visualization

  Seaborn                             Statistical data visualization
Jupyter Notebook                    Development and experimentation
5. Project Implementation
Step 1: Website Access
Used the Python Requests library to send an HTTP request to the Cars24
used-cars page and retrieve the webpage response.
Step 2: HTML Parsing
Used BeautifulSoup to parse the returned HTML, inspect the page title,
and extract readable website content.
Step 3: Embedded Data Inspection
Inspected script tags within the webpage to locate embedded information
containing vehicle listing attributes.
Step 4: Data Extraction
Used regular expressions to extract fields such as car name, brand,
model, year, fuel type, transmission, odometer reading, ownership, and
listing price.
Step 5: Dataset Creation
Combined the extracted fields into a Pandas DataFrame and converted
numeric attributes into appropriate numeric data types.
Step 6: Data Export
Exported the structured dataset into a CSV file named
cars24_used_cars.csv.
Step 7: Data Inspection and Quality Checks
Examined the dataset shape, column data types, missing values, duplicate
records, and non-positive listing prices.
Step 8: Feature Preparation
Worked with derived fields including Car_Age and Price_Lakhs to
support price-related analysis.
Step 9: Exploratory Data Analysis
Used the collected vehicle attributes to investigate patterns and
compare listing prices within the available sample.
6. Dataset Overview
The current extracted dataset contains 10 records and 11 columns.
  Dataset Attribute                   Details
  Total records                       10

  Total columns                       11

  Missing values                      0 across the displayed dataset

  Duplicate records                   0

  Invalid non-positive prices         0 records returned by the notebook
check
Export format                       CSV
Dataset Columns
  Column           Description
  Car_Name       Full name of the listed car
Brand          Vehicle manufacturer
Model          Vehicle model
Year           Manufacturing year
Fuel_Type      Fuel type
Transmission   Transmission category
KM_Driven      Kilometres driven
Ownership      Ownership count shown in the listing
Price          Listing price in Indian rupees
Car_Age        Derived age of the car
Price_Lakhs    Listing price converted into lakhs
7. Initial Observations
Based on the 10 records displayed in the current notebook:
- The extracted listings include brands such as Hyundai, KIA, Honda,
  Maruti, Tata, Mahindra, and Renault.
- Hyundai appears three times in the collected sample.
- All 10 displayed listings have Petrol as the fuel type.
- The collected sample contains both Manual and Automatic transmission
  listings.
- The Mahindra XUV700 has the highest listed price in this sample.
- The Renault Kwid has the lowest listed price in this sample.
These observations describe only the collected records. A larger dataset
is required before drawing conclusions about broader used-car market
trends.
8. Project Structure
Cars24-Used-Car-Market-Analysis/
│
├── Car Market Analysis – Cars24.ipynb
│
├── cars24_used_cars.csv
│
└── README.md
9. Installation and Execution
Follow the steps below to run the project locally.

Prerequisites: - Python installed on your system. - Jupyter Notebook
or JupyterLab. - Internet connection to access the Cars24 webpage.
Step 1: Clone the Repository
git clone https://github.com/your-username/Cars24-Used-Car-Market-Analysis.git
Step 2: Navigate to the Project Directory
cd Cars24-Used-Car-Market-Analysis
Step 3: Install Dependencies
pip install pandas numpy matplotlib seaborn requests beautifulsoup4
Step 4: Launch Jupyter Notebook
jupyter notebook
Step 5: Execute the Notebook
Open Car Market Analysis – Cars24.ipynb and execute the cells
sequentially to perform website access, data extraction, dataset
creation, data inspection, and analysis.

The notebook exports the extracted data as:
cars24_used_cars.csv
10. Skills Demonstrated
This project demonstrates practical experience in:
- Python programming
- HTTP requests and webpage access
- Web scraping concepts
- HTML parsing using BeautifulSoup
- Regular Expressions for data extraction
- Data extraction from embedded page content
- DataFrame creation and manipulation using Pandas
- Numeric data type conversion
- CSV data export
- Data inspection and quality checks
- Feature creation and data preparation
- Exploratory Data Analysis (EDA)
- Data analysis documentation
11. Limitations and Future Improvements
Current Limitations
- The current dataset contains only 10 vehicle listings.
- The extracted sample may not represent all Cars24 listings,
  locations, or vehicle categories.
- Website HTML and embedded scripts may change, affecting the
  extraction logic.
- Listing prices and vehicle availability may change over time.
- The current sample is too small for broad market-level conclusions.
Future Improvements
- Expand the dataset by collecting more listings, where permitted.
- Capture listing location and collection date.
- Improve extraction validation and error handling.
- Add further statistical analysis of vehicle attributes and prices.
- Explore price patterns across brands, models, fuel types, and
  transmission categories.
- Develop an interactive dashboard using Power BI or Python
  visualization tools.
12. Conclusion
Cars24: Used Car Market Analysis & Price Intelligence demonstrates how
Python can be used to access website data, extract structured
information, and prepare a dataset for analysis.

The project provided practical experience in webpage inspection, HTML
parsing, regular-expression-based extraction, Pandas DataFrame creation,
CSV export, and data-quality checks. It also establishes a foundation
for further analysis of used-car listing prices as the dataset grows.
Author
Shrapti Bedre

Information Technology Graduate | Aspiring Data Analyst

Project: Cars24 -- Used Car Market Analysis & Price Intelligence

Technologies: Python | Requests | BeautifulSoup | Regular
Expressions | Pandas | NumPy | Matplotlib | Seaborn


