# Unit-3: Data Wrangling (Experiment 14)

## Author Information
* **Name:** RUDRANSH SHARMA
* **PRN:** 25070123096

## AIM
To study data binning and data formatting techniques in Pandas including categorization, type conversion, sorting, and analysis of datasets.

## THEORY
The following functions and concepts from the Pandas library are utilized for effective data categorization and formatting:

* **`pd.DataFrame()`**: Creates a structured table (DataFrame) from dictionary or data.
* **`print()`**: Displays output on the console.
* **`pd.cut()`**: Divides continuous data into discrete bins or categories.
* **`bins`**: Defines the range intervals for categorization.
* **`labels`**: Assigns names to each bin category (e.g., 'Low', 'Medium', 'High').
* **`df['new_column'] = pd.cut()`**: Creates a new categorical column based on binning logic.
* **`df.dtypes`**: Shows the datatype of each column in the DataFrame.
* **`astype()`**: Converts data from one datatype to another (e.g., integer to float).
* **`df['col'].astype(float)`**: Converts specific column values into float datatype.
* **`df['col'].str.upper()`**: Converts all string values in a column to uppercase for uniformity.
* **`round()`**: Rounds numeric values to a specified number of decimal places.
* **`df.sort_values()`**: Sorts the DataFrame based on a specified column.
* **`ascending=False`**: Sorts data in descending (high to low) order.
* **`ascending=True`**: Sorts data in ascending (low to high) order (default setting).
* **`df['col'].unique()`**: Returns all unique values present in a specific column.
* **`value_counts()`**: Counts the frequency/occurrence of each category in a column.
* **Multiple binning**: Applying `pd.cut()` on different columns to categorize various features simultaneously.
* **Categorical Data Analysis**: Techniques that help in grouping continuous data into meaningful ranges for better interpretation.

## ALGORITHM
The logical process for data binning and formatting is as follows:

1.  **Data Preparation**: Define a dataset containing continuous numerical variables and unformatted string data.
2.  **Binning Implementation**: 
    * Define interval boundaries (bins) and corresponding category names (labels).
    * Apply `pd.cut()` to transform continuous numbers into discrete segments.
3.  **Data Type Calibration**: Identify current datatypes using `.dtypes` and cast columns to appropriate types (e.g., float)
