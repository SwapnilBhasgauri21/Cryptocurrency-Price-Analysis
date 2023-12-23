# Cryptocurrency Price Analysis
The project involves retrieving real-time cryptocurrency data from the CoinMarketCap API, analyzing it, and visualizing trends over time. The programming language used is Python, and the main libraries employed include Requests, Pandas, Matplotlib, and Seaborn.

# API Data Retrieval:  
Utilizes the CoinMarketCap API to retrieve real-time cryptocurrency data.
Specifies API parameters, such as the number of cryptocurrencies to retrieve and the conversion currency (USD).
Handles potential connection errors and retrieves data in JSON format.
 
# Data Processing and Storage:  
Uses Pandas to process and normalize the JSON data into a DataFrame.
Appends a timestamp to the DataFrame for each data retrieval.
Defines a function (api_runner) to automate the API request process and update the DataFrame at regular intervals.
Runs the API request in a loop, updating the DataFrame every minute for a specified number of iterations.
 
# Data Analysis and Visualization:  
Analyzes the cryptocurrency data by calculating the mean percentage change for specific time intervals (1h, 24h, 7d, etc.).
Structures the data for visualization using Seaborn, creating a DataFrame with columns for percentage change, cryptocurrency name, and timestamp.
Utilizes Seaborn to create a categorical plot, showing how various cryptocurrencies perform over different time intervals.
 
# Individual Coin Price Trend:
Extracts and visualizes the price trend of a specific cryptocurrency (e.g., Bitcoin) over time.
Selects relevant columns (name, price, timestamp) from the DataFrame and filters data for the chosen cryptocurrency.
Uses Seaborn to create a line plot displaying the price trend of the selected cryptocurrency.
 
# Conclusion:
The project provides a comprehensive overview of cryptocurrency trends, allowing for real-time analysis and visualization of price changes over different time periods. The code is structured to facilitate ongoing data collection and analysis.
