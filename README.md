<h1>YouTube Trending Videos Analysis</h1>

• This project is based on exploring and cleaning YouTube trending video statistics from different countries. The data contains video information in CSV format and category details in JSON format. All tasks were done using Google Colab.



**Tools & Libraries Used**

• Google Colab – for coding and running the notebook online

• Python – programming language used for data analysis

• Pandas – for reading, processing, and analyzing data

• json – for parsing JSON files

• os – for file handling and directory access

• zipfile – for extracting the zipped dataset

• NumPy – used for numerical operations and outlier detection



**Dataset Details**

The dataset includes:

• Trending video data for multiple countries (e.g., US, IN, GB, KR, JP, etc.) in .csv format.

• YouTube category ID mapping for each country in .json format.




**Workflow Summary**

1. Data Upload & Extraction

• Uploaded the .zip file using Google Colab.

• Extracted all files into a folder using Python's zipfile module.


2. Exploration

• Listed and reviewed all the files present in the extracted folder.


3. JSON Parsing

• Flattened the JSON files to extract relevant fields like:

• id

• title

• channelId

• assignable



4. Data Cleaning

• Checked basic info: shape, missing values, data types.

• Removed any duplicate rows.

• Renamed column names to lowercase and replaced spaces with underscores.

• Cleaned textual data (e.g., trimmed whitespaces, converted to lowercase).


5. Outlier Removal

• Used Interquartile Range (IQR) method on numeric columns to remove any outliers.




**Final Output**

• A clean, ready-to-analyze DataFrame with consistent structure.

• Useful for further data analysis, visualizations, or building dashboards
