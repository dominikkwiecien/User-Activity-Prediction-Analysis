
# User Activity Analysis with Linear Regression

## Overview
This project demonstrates the use of linear regression for predicting user activity metrics, specifically Daily Active Users (DAU) and Weekly Active Users (WAU), using Google Sheets. It also includes various charts that visualize user activity data.

## Project Structure

- **WAU Sheet**: 
  - Contains data on Weekly Active Users (WAU), Average Daily Active Users (DAU), and the ratio DAU/WAU.
  - Includes predicted values for 20 future weeks using the `FORECAST` function.

- **Active Users Sheet**: 
  - Contains data on individual users, including user ID, game name, language, whether the user has an older device model, and age.
  - Includes summary statistics such as average age, standard deviation, median, and quartiles.

## Analysis Steps

### Part 1: Estimating DAU and WAU
1. **Extending Data Range**: Added 20 additional weeks to the WAU sheet.
2. **Prediction**: Used `ROUND` and `FORECAST` functions to predict WAU and DAU for the new weeks.
3. **Calculating DAU/WAU**: Computed the DAU/WAU ratio for the predicted weeks.

### Part 2: Building Charts
1. **Bar Chart**: Displays the number of users per language (from the "Active Users" sheet).
2. **Pie Chart**: Shows the distribution of users based on whether they have an older device model.
3. **Combo Chart**: Combines a bar chart for WAU and a line chart for DAU/WAU over time.
4. **Polynomial Trendline Chart**: Visualizes WAU over time with a polynomial trendline of degree 3.

## How to Use
- Download and open the `Zadanie 4.xlsx` file to explore the data and charts.
- Use the data and charts to understand user activity trends and the effectiveness of predictions.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
