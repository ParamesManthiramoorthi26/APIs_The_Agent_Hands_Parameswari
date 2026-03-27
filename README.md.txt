# APIs: The Agent's Hands - Subjective

**Student Name:** Parameswari Manthiramoorthi  
**Roll No:** IITP_AIMLTN_2602771  

## Project Overview

This Jupyter Notebook demonstrates how to **fetch, process, and analyze country data** using a public REST API. The data is retrieved from the [REST Countries API](https://restcountries.com/), and Python libraries like `requests`, `pandas`, `matplotlib`, and `seaborn` are used for analysis and visualization.  

The analysis focuses on:

1. Fetching and validating API responses.
2. Extracting and displaying key country data fields.
3. Summarizing and visualizing insights such as:
   - The region with the highest total population.
   - The largest countries by area.

---

## Notebook Tasks

### Task 1 — Fetch and Validate API Response
- Send a GET request to the REST Countries API using the `requests` library.
- Validate the response using a `try-except` block.
- Display the total number of countries retrieved.

**Result:** 250 countries retrieved successfully.

---

### Task 2 — Extract and Display Key Fields
- Convert JSON response to a Pandas DataFrame.
- Extract the `common` country name from the nested `name` field.
- Check for missing values in `region` and `area` columns.
- Display the first 10 rows of the dataset for a quick overview.

**Observation:** No missing values in the dataset.

---

### Task 3a — Region with Highest Population
- Group countries by `region` and sum their populations.
- Identify the region with the highest population using `.idxmax()`.

**Result:**  
- **Region:** Asia  
- **Total Population:** 4,724,731,966  

**Visualization:** Bar chart displaying total population by region shows that Asia has the highest population.


**Total Population by Region**  

![Population Chart](images/population_chart.png)
---

### Task 3b — Country with Largest Area
- Find the country with the largest area using `.idxmax()` on the `area` column.
- Display the country name and area.

**Result:**  
- **Country:** Russia  
- **Area:** 17,098,246 sq. km  

**Visualization:** Bar chart of top 10 largest countries by area highlights Russia as the largest, followed by Antarctica, Canada, China, and the United States.


**Top 10 Largest Countries by Area**  

![Area Chart](images/area_chart.png) 

---

## Libraries Used
- `requests` — For API requests  
- `pandas` — For data processing and manipulation  
- `matplotlib` & `seaborn` — For visualization  

---

## Conclusion
This notebook demonstrates how to leverage a public REST API for live data analysis. Key insights include:

- Asia is the most populated region.  
- Russia is the largest country by area.  


---

