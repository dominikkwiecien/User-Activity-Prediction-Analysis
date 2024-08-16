
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

Chart 1: Number of Users by Language

This horizontal bar chart displays the number of users by the language they speak.
<img width="787" alt="image" src="https://github.com/user-attachments/assets/9fefdc6f-2cc1-46e0-bf50-05cae6eaea21">

- uk: The largest group of users speaks Ukrainian, making up the majority of the user base.
- ru: The second-largest group of users speaks Russian.
- en: The smallest group of users speaks English.

This chart provides a clear visualization of the dominant languages among the application's users.


Chart 2: Distribution of Users by Device Type

This pie chart illustrates the distribution of users based on whether they have an older device model.
<img width="788" alt="image" src="https://github.com/user-attachments/assets/481de188-000b-4853-bc1b-6d2d0f2fe4ea">

- 88.0% of users (blue segment) do not have an older device model (FALSE).
- 12.0% of users (red segment) have an older device model (TRUE).

This chart provides insight into the proportion of users who are using older technology compared to those with newer devices.

Chart 3: WAU and DAU/WAU Over Time

This combo chart shows the Weekly Active Users (WAU) over time as blue bars and the DAU/WAU ratio as a red line.

<img width="779" alt="image" src="https://github.com/user-attachments/assets/4e88e256-9318-44e5-8d0f-d47baa0a3d77">

- WAU (Blue Bars): The number of Weekly Active Users has generally increased over time, with noticeable growth beginning in mid-2022.
- DAU/WAU Ratio (Red Line): The ratio of Daily Active Users to Weekly Active Users has fluctuated over time, indicating varying levels of daily engagement compared to weekly activity.

This chart provides a comprehensive view of user engagement trends over the analyzed period.


Chart 4: WAU Over Time with a Polynomial Trend Line (Degree 3)

This chart displays the Weekly Active Users (WAU) over time as blue bars, along with a polynomial trend line of degree 3 in red.

<img width="777" alt="image" src="https://github.com/user-attachments/assets/7ebedefa-2c66-4718-99b4-664738b1a39b">

- WAU (Blue Bars): The chart shows the weekly active users increasing over time, with a peak around mid to late 2022, followed by a slight decline.
- Polynomial Trend Line (Red Line): The trend line fits the data with a high degree of accuracy (R² = 0.965), capturing the general upward trend and the subsequent leveling off and decline in WAU.

This chart provides a smoothed perspective on how WAU has changed over time, highlighting the key trends in user activity.



## How to Use
- Download and open the `User-Activity-Prediction-Analysis.xlsx` file to explore the data and charts.
- Use the data and charts to understand user activity trends and the effectiveness of predictions.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
