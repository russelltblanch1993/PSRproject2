# Renovate with Confidence
## A Guide for Homeowners on Home Renovation Projects that Increase Home Value

**Authors**: Paul Schulken, Sean Conlon, Russell Blanchard

## Overview

This project is intended for homeowners looking to increase the value of their homes through various renovations. Using housing data provided from King County, Washington we have conducted an analysis on different factors that could potentially enhance the value of homes.

## Business Problem

We understand that homeowners may be looking for ways to increase the value of their homes. Our goal is to identify any particular features that correlate with the home value so that homeowners can make efficient decisions. We also want to ensure that any potential renovations to the home are worth the investment.

Our analysis revealed that the grade of the home (which, per the King County government website, is a measure of the construction quality of improvements) has the highest correlation with sales price. On average, the price increases by $188,600 for every increase in grade. When we looked further into the data, we found that number of bathrooms had the highest correlation on grade, and an increase of 1 bathroom led to an average price increase of $105,000.

## Data

The data was taken from the King County government website and offered us information on property transactions throughout the area. Since we wanted our analysis to focus on data pertinent to current homeowners, we were able to narrow the dataset down to just those features that are within the homeowner’s control. The dataset used didn't incorporate all factors that could contribute to home grade, such as type of flooring or quality of kitchen appliances. There are also other factors like permitting costs and whether or not a renovation would pass an inspection.

## Data Modeling

As mentioned earlier, the number of bathrooms had the highest correlation on grade, which in turn had the highest correlation with price. To double check our models, we plotted the number of bathrooms against the average grade, then plotted the grade against average sale price. Although the average grade seems to decrease beyond 6 bathrooms, about 97% of the homes had between 1 and 3.5 bathrooms. As for average sale price, there is a strong positive relationship between grade and average price. Houses graded between 6 and 9 comprised almost 96% of the data.

![Mean House Grade by Number of Bathrooms](./models/Mean_House_Grade_by_Number_of_Bathrooms.jpeg)

![Mean Sale Price by House Grade](./models/Mean_Sale_Price_by_House_Grade.jpeg)

Earlier in our analysis we found grade to have the highest correlation with price so we wanted to see the effect of grade with price as our target. We found that grade alone accounts for about 28% of the variance in sales price. After adding all features under the homeowner’s control to the model, we were able to determine the $188,600 increase in price with one increase of grade. Our model also showed us the impact rankings of the features and confirmed that grade was the highest.

## Results and Recommendations

We discovered that the grade of a home correlates strongly with its price. Specifically, homes with higher grades tend to have more desirable features, such as garages, patios, and a greater number of bedrooms and bathrooms. Therefore, to increase the grade of a home, it's necessary to perform renovations that add these desirable features. Based on our research, the mean price of homes with 2.5 or more bathrooms is higher than the average price of homes with 2 or fewer bathrooms. This shows the number of bathrooms is an important factor in a home’s value.

![Sale Price by Number of Bathrooms](./models/Sale_Price_by_Number_of_Bathrooms.jpeg)

Throughout our data, we found that different sizes of renovations will add different values. Homeowners who have invested more in their home renovation have been able to achieve a higher sale price for their home.

Based on our research, we recommend that homeowners consider upgrading specific features of their homes, whether it is for their own enjoyment or to attract more potential buyers. Specifically, adding or upgrading a bathroom was shown to have a high impact on both grade and price.

## Next Steps

Future research will help you find the highest return on investment in your local housing market. Seek advice from a professional home appraiser or real estate agent to get a better understanding of the potential impact of renovations on your home’s value. Lastly, plan renovations carefully to ensure they align with the overall goals of the home, such as increasing your enjoyment of the property or making your home market-ready.

## For More Information

Please review our full analysis in [our Jupyter Notebook](./Phase_2_Project_Notebook.ipynb) or our [presentation](./presentation.pdf).

## Repository Structure

```
├── exploratory_files                   <- Jupyter notebooks for data exploration and testing
├── models                              <- Both sourced externally and generated from code
├── data                                <- Data files used in analysis
├── .gitignore                          <- Code to avoid uploading specified files
├── Phase_2_Project_Notebook.ipynb      <- Narrative documentation of analysis in Jupyter notebook
├── README.md                           <- The top-level README for reviewers of this project
├── presentation.pdf                    <- PDF version of project presentation
```