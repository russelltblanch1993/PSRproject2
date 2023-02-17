###

Good morning, everyone. My name is Russell and I am here to present to you our recommendations for homeowners looking to increase the value of their homes through various renovations. Using housing data provided from King County, Washington we have conducted an analysis on different factors that could potentially enhance the value of homes.

Our team consists of Paul Schulken, technical lead; Sean Conlon, presentation lead; and Russell Blanchard, GitHub lead.

First, we’ll discuss what we sought to achieve with our analysis and who it might benefit. Then, we’ll discuss the data used and what we did to find answers to the questions we started with. After that, we’ll interpret the results of our analysis and how they formed our recommendations. Finally, we’ll go over what could be done in the future to refine our results.

We understand that homeowners may be looking for ways to increase the value of their homes. Our goal is to identify any particular features that correlate with the home value so that homeowners can make efficient decisions. We also want to ensure that any potential renovations to the home are worth the investment.

Our analysis revealed that the grade of the home (which, per the King County government website, is a measure of the construction quality of improvements) has the highest correlation with sales price. When we looked further into the data, we found that number of bathrooms had the highest correlation on grade, followed by the square footage of a garage.


The data was taken from the King County Assessor Data Download website and offered us information on home sales throughout the area with numerous variables about the size, location, and features of the homes. Since we wanted our analysis to focus on data pertinent to current homeowners, we were able to narrow the dataset down to just those features that are within the homeowner’s control. We did notice some oddities in the dataset, such as a 4 bed 4.5 bath mansion that listed the sale price as $40,000, but this home and other outliers were removed before our analysis began.

As mentioned earlier, the number of bathrooms had the highest correlation on grade, which in turn had the highest correlation with price. To double check our models, we plotted the number of bathrooms against the average grade, then plotted the grade against average sale price. Although the average grade seems to decrease beyond 6 bathrooms, about 99% of the homes had between 1 and 4 bathrooms. As for average sale price, there is a strong positive relationship between grade and average price. Houses graded between 6 and 9 comprised almost 96% of the data.

Earlier in our analysis we found grade to have the highest correlation with price, so we created a baseline model with price as our target. This returned a mean error of just under $430,000, suggesting the model could have that much of a difference between the predicted price and actual price. Next, we added just grade to the model, which returned a high (but better than our baseline) mean error. We can also see that the grade of a home is responsible for about 28% of the variance in sale price. Lastly, we added all features under the homeowner’s control to the model, which improved both our mean error and R-squared value. The model with all features also revealed the impact rankings of the features, with grade being most impactful and the presence of a garage least.

To determine the most effective way to increase the grade of a home, we performed a similar analysis with grade as the target. The baseline mean error was 0.99, which was decreased to 0.80 when adding just bathrooms to the model. The number of bathrooms explains about 34% of the variance in house grade. After adding the remaining features to the model, we were able to decrease our mean error and increase our R-squared value. The impact rankings were slightly different, but number of bathrooms remained a critical feature in both sets of models.

We discovered that the grade of a home correlates strongly with its price. Specifically, homes with higher grades tend to have more desirable features, such as garages, patios, and a greater number of bedrooms and bathrooms. Therefore, to increase the grade of a home, it's necessary to perform renovations that add these desirable features.

Throughout our data, we found that different sizes of renovations will add different values. Homeowners who have invested more in their home renovation have been able to achieve a higher sale price for their home.

A Cost vs. Value report made by Remodeling magazine reveals in 2022, homeowners spent an average of $64,000 on renovations, 
which in turn increased their homes value by an average of 60%. Meaning if a homeowner spends the average amount of $64,000 on their renovations, they can add approximately $100,000 in value to their home.

Based on our research, we recommend that homeowners consider upgrading specific features of their homes, whether it is for their own enjoyment or to attract more potential buyers. Specifically, adding or upgrading a bathroom was shown to have a high impact on both grade and price.

What are the Next Steps! 
Future research will help you find the highest return on investment in your local housing market. 
Seek advice from a professional home appraiser or real estate agent to get a better understanding of the potential impact of renovations on your home’s value. 
Lastly, plan renovations carefully to ensure they align with the overall goals of the home, such as increasing your enjoyment of the property or making your home market-ready. 


We believe that our recommendations will provide valuable insight for homeowners looking to increase the value of their home. Thank you for your attention and we look forward to your feedback. We will now open up to any questions. 

###






