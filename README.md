# Bar Hopping Optimization Project

## Overview

This project focuses on optimizing a **bar-hopping schedule** for students visiting 10 pre-selected bars near the Ohio State University (OSU) Columbus campus. The objective was to minimize the **total cost of drinks** and **walking distance** while adhering to a reasonable college-friendly budget. The solution was implemented using **mixed linear programming** techniques and demonstrates strong data science, optimization, and problem-solving skills.

---

## Problem Statement

Given 10 popular bars around the OSU campus, the goal was to:
1. Create a **mixed linear program** to find the optimal bar-hopping schedule.
2. Minimize the **total cost per student** for drinks.
3. Minimize the **walking distance** between bars.

---

## Process Overview

The project followed these steps:

1. **Bar Selection**: Shortlisted 10 popular bars around campus based on reviews and popularity.
2. **Data Collection**: Gathered data on:
   - Average price per drink at each bar.
   - Average time spent at each bar.
   - Bar ratings (out of 5 stars).
   - Distances between bars (in miles).
   - Bar operating hours.
3. **Data Preparation**:
   - Generated a table summarizing drink prices, review ratings, time spent at each bar, and distances between bars.
   - Calculated the average price for three popular drinks at each bar.
4. **Constraints**:
   - Set a reasonable college-friendly budget for each student.
   - Modeled walking distance and bar operating hours as constraints.
5. **Optimization**:
   - Used mixed linear programming to:
     - Minimize the average price per drink.
     - Find the optimal route to minimize walking distance.

---

## Assumptions and Simplifications

To make the problem computationally feasible, the following assumptions were made:
- Little to no wait time outside bars.
- The outing starts after 10 PM on Friday nights.
- Only three of the most popular drinks were considered for calculating average drink prices.
- Distance calculations were based on straight-line distances (in miles).
- Only 10 pre-selected bars around campus were included in the analysis.

---

## Data Summary

### Example Data Points
- **Bar Details**: "At Bar 1, people spend an average of $3.67 per drink, stay for about 20 minutes, and rate it 4.4 out of 5 stars. The bar operates from 7 PM to 2 AM on Fridays."
- **Distance Matrix**: "The distance between Bar 1 and Bar 2 is 0.041 miles."

### Key Metrics
- Average price per drink for each bar.
- Walking distances between all pairs of bars.
- Operating hours for each bar.

---

## Results

### Optimal Bar-Hopping Schedule
The optimization algorithm recommended visiting the following bars:
1. Bar 1
2. Bar 3
3. Bar 6
4. Bar 7
5. Bar 9

The suggested drink purchases were:
- **2 drinks at Bar 1**
- **3 drinks at Bar 3**
- **2 drinks at Bar 9**

This resulted in a total minimum cost of approximately `$25`.

### Optimal Walking Route
To minimize walking distance, the following route was suggested:

3’s -> The Library Bar -> Midway -> Leo’s on the Alley -> Ethyl and Tank -> Back to 3’s

The total walking distance was minimized to **1.64 miles**, ensuring convenience for participants.

---

## Tools and Technologies Used

- **Python**: For data processing, modeling, and visualization.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For matrix operations (e.g., distance matrix).
- **PuLP/OR-Tools**: To solve the mixed linear programming problem.
- **Matplotlib/Seaborn**: For visualizing results like bar routes and cost breakdowns.

---

## Skills Demonstrated

This project highlights several key data science skills:

1. **Data Analysis**:
   - Extracted actionable insights from raw data on drink prices, bar ratings, and distances.

2. **Mathematical Modeling**:
   - Formulated a mixed linear programming problem with real-world constraints like budgets, operating hours, and distances.

3. **Optimization Algorithms**:
   - Solved complex optimization problems using Python libraries like PuLP/OR-Tools.

4. **Data Visualization**:
   - Created clear visualizations to communicate results effectively (e.g., bar routes, cost breakdowns).

5. **Problem-Solving**:
   - Translated a real-world problem into a structured mathematical framework and derived practical solutions.

---

## Future Improvements

While this project provides a solid foundation, there are opportunities for enhancement:

1. Incorporate real-time data (e.g., live wait times or drink specials).
2. Add support for larger datasets with more bars across different cities.
3. Use geospatial APIs (e.g., Google Maps API) for more accurate distance calculations.
4. Introduce user preferences (e.g., favorite drinks or ambiance) into the optimization model.

---

## Acknowledgments

This project was inspired by college life experiences and aims to blend practicality with fun through data science! Feel free to reach out with questions or suggestions! 😊
