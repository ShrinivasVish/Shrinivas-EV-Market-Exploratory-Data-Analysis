# Comprehensive Pandas Assignment: Electric Vehicle Market Analysis

As a data analyst for an automotive research firm, you're tasked with analyzing the electric vehicle (EV) market using Python and Pandas. Your analysis will cover various aspects of EVs, including brands, models, range, pricing, sales, and manufacturing details.

## Datasets

You will work with the following datasets:

1. **`ev_main.csv`**: Contains main EV data (Brand, Model, Range, Price, Sales)
2. **`ev_efficiency.csv`**: Contains efficiency data for EV models
3. **`ev_manufacturing.csv`**: Contains manufacturing locations for each brand

## Tasks

### 1. Introduction to Pandas and Series Operations

1. Create a Pandas Series containing EV brands: Tesla, Nissan, Chevrolet, BMW, Ford.
2. Perform basic operations like indexing and string methods on this series.
3. Calculate and display the mean length of the brand names.

### 2. Working with DataFrames

1. Load the **`ev_main.csv`** into a DataFrame.
2. Display DataFrame information. What insights can you gather?
3. Access and display the DataFrame's axes.
4. Demonstrate accessing specific values of the data.
5. Apply a filter to show EVs with a range over 250 miles.
6. Calculate the average price of EVs.

### 3. Handling Duplicates and NA Values

1. Check for and remove any duplicate entries based on the 'Model' column.
2. Identify NA values in the DataFrame. How many are there and in which columns?
3. Handle NA values in the 'Sales' column by filling them with the median sales value.
4. For any remaining NA values, devise and implement an appropriate strategy to handle them.

### 4. Advanced DataFrame Operations

1. Load **`ev_efficiency.csv`** and **`ev_manufacturing.csv`** into separate DataFrames.

2. Merge:

   - Merge the main EV DataFrame with the efficiency DataFrame based on the 'Model' column.
   - Perform a left join to merge the resulting DataFrame with the manufacturing DataFrame based on the 'Brand' column.

3. Concatenation:

   - Split the main DataFrame into two based on a condition (e.g., Price > 50000).
   - Concatenate these DataFrames back together. Verify the result matches the original.

4. Apply:

   - Create a new column 'Efficiency_Score' that categorizes each vehicle as 'High' or 'Low' efficiency based on a threshold.
   - Apply a custom function to calculate a 'Value_Score' as (Range \* Efficiency) / Price.

5. Reshape:
   - Create a pivot table showing average price by Brand and Efficiency_Score.
   - Melt the DataFrame to create a "long" format for Range, Price, and Sales.

### 5. Working with Vectors

1. Extract 'Range' and 'Price' columns as NumPy arrays.
2. Calculate the correlation coefficient between range and price.
3. Perform element-wise operations on these vectors (e.g., calculating price per mile of range).

### 6. Exploratory Data Analysis (EDA) with Pandas

1. Generate descriptive statistics using **`describe()`**. Interpret the results.
2. Create visualizations:
   - Scatter plot of Range vs Price
   - Bar plot of average Efficiency by Brand
   - Box plot of Price distribution by Brand
   - Pie chart of market share based on Sales

### 7. Advanced Analysis

1. Group the data by Brand and Manufacturing_Location, then calculate mean Range, Price, and Efficiency.
2. Use `pd.cut()` to bin the 'Price' into categories (Budget, Mid-range, Luxury). Analyze the distribution of these categories across Brands.
3. Identify the top 5 models based on the 'Value_Score' you created earlier.
4. Calculate the percentage of High vs Low efficiency vehicles for each Brand.
5. Perform a time-based analysis if your dataset includes a date column. If not, create a hypothetical 'Launch_Date' column and analyze trends over time.

## Submission Guidelines

1. Provide your well-commented Python code for all tasks.
2. Include all outputs, plots, and visualizations generated.
3. Write a comprehensive report (750-1000 words) summarizing your methodology, key findings, and insights about the EV market based on your analysis.
4. Discuss any challenges you faced during the analysis and how you overcame them.
5. Suggest potential further analyses that could provide additional insights into the EV market.

Remember to use Pandas functions and methods wherever applicable, and strive for efficient, readable code. Good luck with your analysis!
