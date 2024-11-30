# NBA-MVP-Predictor
Predict the MVP of upcoming NBA season based on historical data


Here's a concise summary of my project:

1. **Data Collection & Web Scraping**: scraped data on NBA players, MVP votes, and team statistics from various sources, using web scraping techniques with `requests`, `BeautifulSoup`, and `Selenium` to handle dynamic content and rate-limiting issues.

2. **Data Cleaning & Preprocessing**: 
   - Removed irrelevant columns (e.g., "Unnamed: 0" and "Rk") from the players' dataset.
   - Filled missing values in key columns with zeros to ensure the data was complete.
   - Standardized team names and mapped player nicknames.
   - Merged datasets containing player statistics, MVP votes, and team data to create a comprehensive dataset.
   - Applied feature engineering, creating derived features like performance ratios (e.g., `PTS_R`, `AST_R`).

3. **Exploratory Data Analysis (EDA)**: 
   - Conducted basic EDA by inspecting key statistics and identifying trends.
   - Visualized player performance, highest scoring players, and MVP trends over the years.

4. **Modeling**: 
   - Initially used Ridge Regression to predict MVP rankings based on player statistics.
   - Improved model performance by switching to Random Forest Regressor, achieving a higher Mean Average Precision (MAP) of 80% (vs. 71% with Ridge).
   - Performed hyperparameter tuning and handled categorical variables like player position and team using encoding techniques.

5. **Evaluation**:
   - Evaluated model performance using MAP, comparing predicted MVP rankings with actual MVP vote results.
   - Applied backtesting over multiple years to assess model consistency and robustness across different seasons.

6. **Results**: 
   - The Random Forest model outperformed Ridge Regression, with improved MAP and more accurate ranking predictions.
   - Successfully predicted MVP rankings with higher precision, showcasing the flexibility and power of Random Forest over simpler models like Ridge Regression.

This project involved web scraping, data preprocessing, feature engineering, model building, and evaluation to predict MVP rankings, demonstrating my ability to handle real-world data and use machine learning techniques for predictive analytics.
