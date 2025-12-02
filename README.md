# 📊 Kozhikode 2020 Local Body Election – Web Scraping, Demographic Enrichment & Political Analysis

This project focuses on extracting, enriching, and analyzing the 2020 Kozhikode Local Body Election member list from the official Kerala Government Local Self Government Department portal (lsgkerala.gov.in).
The goal of the project is to automate the data collection process, clean and structure the scraped information, enrich it with demographic attributes such as religion, and perform meaningful political and community-level analysis.

This end-to-end project demonstrates core skills in web scraping, data cleaning, feature engineering, EDA, and political/demographic data analytics.

## 🧠 Project Motivation

Local body elections in Kerala reflect strong patterns of:

- Community-based political alignment

- Party dominance across local wards

- Age and demographic trends in candidate selection

However, publicly available datasets are often unstructured and lack important attributes like age or religion.
This project solves that by:

- Automating data scraping

- Creating clean structured datasets

- Adding new features

- Performing insightful political analysis

## 🚀 Project Workflow (End-to-End)
1️⃣ Web Scraping from lsgkerala.gov.in

The 2020 Local Body Elections for various districts, including Kozhikode, are hosted on the LSGD website.
Using Requests and BeautifulSoup, the project scrapes:

- Names of elected members

- Ward number / seat

- Political party

- Additional details like age (if available)

Tools used:

- requests

- BeautifulSoup

- pandas

The scraper navigates through HTML tables, extracts rows, removes unnecessary tags, and converts them into a structured Pandas DataFrame.

## 2️⃣ Data Cleaning & Standardization

After extraction, the scraped data contains inconsistencies such as:

- Inconsistent age formats

- Mixed text inside names

- Party labels not standardized

- Missing values

Cleaning steps include:

- Removing unnecessary characters

- Converting age to numeric

- Standardizing party names (LDF, UDF, BJP, Independent)

- Extracting ward names cleanly

- Removing duplicates and null rows

Libraries used:

- pandas

- numpy

## 3️⃣ Feature Engineering – Religion Prediction Using Names

The website does not provide religion/community information.

To solve this, you designed a rule-based name inference engine:

Approach:

- Define common first-name patterns for:

  - Muslims → Abdul, Muhammed, Fathima, Umar, etc.

  - Hindus → Krishnan, Nair, Kumar, Devi, etc.

  - Christians → Mathew, George, Joseph, Mariya, etc.

- Match each name using keyword-based and suffix-based rules.

- Assign religion as:

  - Hindu

  - Muslim

  - Christian

  - Other

This step adds demographic depth to the dataset, enabling powerful community-level analysis.

## 4️⃣ Exploratory Data Analysis (EDA)
- Party-Wise Analysis

  - Count of elected members by party

  - Visualization using bar charts

  - Identification of dominant parties in Kozhikode

- Community (Religion) Analysis

  - Distribution of Hindu/Muslim/Christian members

  - Inferring political affinity patterns at the community level

- Age Distribution Analysis

  - Age ranges (min, max, average)

  - Representation of younger vs older candidates

Tools used:

- matplotlib

- seaborn

- pandas

📈 Key Insights
1. Political Dominance

  - LDF emerged as the strongest coalition in Kozhikode based on seat count.

  - UDF and BJP had limited representation in many wards.

2. Community Representation

  - The Muslim community had the highest representation among elected members.

  - Hindu and Christian members followed in proportion consistent with Kozhikode’s demographics.

3. Age Trends

  - Most elected members belonged to the 35–55 years age group, showing voter preference for mid-aged leaders.

4. Community–Party Patterns

  - Certain parties showed clear demographic alignment in specific wards.

  - Independent wins occurred mainly in rural or less competitive wards.

## 🧩 Skills Demonstrated

- Web Scraping: Automated data extraction from government election portals using Python, Requests, and BeautifulSoup.

- Data Cleaning & Wrangling: Standardized raw HTML data, handled missing values, normalized text, and cleaned age/party fields using Pandas.

- Feature Engineering: Built a custom rule-based name-matching logic to infer religion/community categories.

- Exploratory Data Analysis (EDA): Analyzed party dominance, community representation, and demographic patterns using Matplotlib and Seaborn.

- Problem Solving: Converted unstructured web data into a structured, analysis-ready dataset with insightful interpretations.

- Data Visualization: Created clear charts to communicate political and demographic trends effectively.

## 🏁 Conclusion

This project successfully transformed unstructured election results from lsgkerala.gov.in into a clean, enriched, and analyzable dataset. By integrating web scraping, data cleaning, demographic inference, and visual analytics, the project reveals meaningful insights into party dominance, community representation, and age trends in the 2020 Kozhikode local body elections.
It highlights how data can be used to understand grassroots political behavior and demonstrates strong end-to-end data analytics and engineering capabilities — from extraction to insight.

# -Local-Body-Election-Member-Scraping-and-Analysis-Kozhikode-2020-
