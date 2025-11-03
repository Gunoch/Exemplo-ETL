Brazilian Universities Data ETL
This notebook demonstrates a simple ETL (Extract, Transform, Load) process to fetch data about Brazilian universities from a public API, process it, and store it in an SQLite database.

Process:
Extract: Data is fetched from the Universities Hipolabs API.
Transform: The data is transformed into a pandas DataFrame, filtered to include only universities in the state of Goiás, and specific columns are selected and formatted.
Load: The transformed data is loaded into an SQLite database named my_lite_store.db into a table called goias_uni.
Files:
This notebook (.ipynb file): Contains the code for the ETL process.
my_lite_store.db: The SQLite database file containing the processed university data.
universities.csv: A CSV file containing the transformed data before loading into the database.
How to Run:
Open the notebook in Google Colab or a local Jupyter environment.
Run the cells sequentially to execute the ETL process.
The resulting SQLite database file (my_lite_store.db) and CSV file (universities.csv) will be created in the same directory as the notebook.
