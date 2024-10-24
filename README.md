## EPL Player Data Web Scraping and Cleaning (2024-2025)

![Alt text](https://images.app.goo.gl/hw2aJQsm38rTtWxX8)

## Project Description
This project extracts and cleans football player data from the 2024-2025 Premier League season using Python. It scrapes player details such as names, teams, dates of birth, heights, and positions from the [worldfootball.net](https://www.worldfootball.net/) website. The data is then cleaned with pandas and exported as a CSV file for further use in analysis or applications.

## Table of Contents
1. [Project Description](#project-description)
2. [Technologies Used](#technologies-used)
3. [Data Source](#data-source)
4. [Data Cleaning Process](#data-cleaning-process)
5. [Project Workflow](#project-workflow)

## Technologies Used
- Python 3
- BeautifulSoup (for web scraping)
- requests (for sending HTTP requests)
- pandas (for data manipulation)

## Data Source
The player data was sourced from the [worldfootball.net](https://www.worldfootball.net/) website, specifically the player list for the 2024-2025 Premier League season.

## Data Cleaning Process
The raw data scraped from the website is cleaned using pandas. The main cleaning steps include:

1. **Handling Missing Values**: Players with missing height data were identified, and missing values were replaced with the median height.
2. **Standardizing Height**: Heights were stripped of the " cm" suffix and converted into numeric values.
3. **Date Formatting**: The dates of birth were converted into a datetime format to allow for easier date-related analysis.
4. **Exporting Data**: The cleaned dataset was saved as a CSV file named epl_players_data.csv.

## Project Workflow
1. **Scraping the Data**: The project loops through 13 pages of player data on the website, sending HTTP requests to retrieve each page’s content.
2. **Parsing HTML**: Using BeautifulSoup, relevant data such as player names, teams, dates of birth, heights, and positions are extracted from the website's table.
3. **Storing the Data**: The extracted data is stored in a Python list, which is then converted into a pandas DataFrame for analysis and cleaning.
4. **Data Cleaning**: Missing values are handled, heights are standardized, and the data is formatted for export.
5. **Exporting**: The cleaned data is exported to epl_players_data.csv.
   
