# Description of project - Research on computer games success

## Research Goals
The goal of this research is to identify patterns that determine the success of a game, which will allow us to invest in potentially popular products and plan advertising campaigns in the future.

## Data Sources
Historical data on game sales, user and expert ratings, genres, and platforms were obtained from open sources in CSV format.

Data Description:
- Name: Game title
- Platform: Gaming platform
- Year_of_Release
- Genre
- NA_sales: Sales in North America (copies sold, mln)
- EU_sales: Sales in Europe (copies sold, mln)
- JP_sales: Sales in Japan (copies sold, mln)
- Other_sales: Sales in other countries (copies sold, mln)
- Critic_Score: Critic rating (maximum 100)
- User_Score: User rating (maximum 10)
- Rating: Rating from the Entertainment Software Rating Board (ESRB). This association assigns age categories to computer games.
*Data for 2016 may be incomplete.

## Libraries
Pandas, Numpy, Matplotlib, Seaborn, Scipy

## Research Plan:
1. Data Overview and Exploration
2. Data Cleaning
   - Handling missing values
   - Data type conversion
   - Removing duplicates and anomalous values
   - Adding new columns
3. Exploratory Data Analysis:
   - Exploration of different data periods and their significance
   - Analyzing sales dependence on platforms
   - Selecting the relevant period for the 2017 forecast and choosing sales-leading platforms
   - Investigating the impact of reviews on sales
   - Exploration of the distribution of games by genre
4. Creating a User Profile for Each Region
5. Hypothesis Testing:
   - Are the average user ratings for Xbox One and PC platforms the same?
   - Are the average user ratings for Action and Sports genres different?
6. General Conclusion on the conducted work and the results obtained."
