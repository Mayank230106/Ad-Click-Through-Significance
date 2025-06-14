# Ad Click-Through Significance Analysis
This project investigates whether any color outperforms "blue" as a link color in terms of click-through rates, using statistical testing and multiple comparison corrections.

## Overview
The analysis compares the average click rates of 31 different link colors to determine if any color yields significantly more clicks than blue. The workflow includes:

1. Calculating mean click rates for each color
2. Identifying colors with higher mean click rates than blue
3. Performing hypothesis tests to compare each color to blue
4. Correcting for multiple comparisons using the Bonferroni method
5. Interpreting results and providing actionable insights

## Key Results
1. Five colors had higher average click rates than blue: Sapphire, Navy, Teal, Ultramarine, and Aquamarine.
2. Of these, Ultramarine had a notably low p-value (0.0034) and a mean click rate of 34.2, compared to blue's mean of 28.35.
3. However, after applying the Bonferroni correction for 29 comparisons (adjusted significance level: 0.0017), Ultramarine's p-value was not statistically significant.
4. If only the top five colors had been tested, the adjusted significance level would have been 0.01, making Ultramarine's result statistically significant in that scenario.

## Summary
1. More data isn't always better: Running unnecessary tests increases the risk of false positives. It's crucial to plan analyses thoughtfully and filter out unlikely candidates before testing.
2. Multiple comparisons matter: Without correcting for multiple tests (e.g., using Bonferroni), you risk "p-value hacking" and drawing incorrect conclusions.
3. Actionable insight: Despite the limitations, Ultramarine may be a promising alternative to blue and warrants further targeted testing.
4. Working with flawed data: Even imperfect experiments can yield useful insights if analyzed carefully.

## How to Run the Analysis
### This project is implemented as a Jupyter Notebook (Ad_Significance.ipynb). To reproduce the results:

1. Open the notebook in Jupyter or Google Colab.
2. Ensure you have the necessary data loaded into the expected DataFrame structure.
3. Execute the cells in order to perform the analysis and view the outputs.

## Dependencies
1. Python 3
2. pandas
3. numpy
4. scipy
5. matlplotlib

Note: These dependencies are already present in Google Colab

## File Structure
1. Ad_Significance.ipynb: Main notebook containing code, analysis, and commentary.
2. colored_ad_click_table.csv: The csv file on which we conduct our analysis.
3. README.md: Explore the project in this file.