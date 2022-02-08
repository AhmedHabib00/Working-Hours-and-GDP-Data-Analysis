## Dataset

The data consists of information about differenct financial aspects including GDP - Average annual wages - Average annual working hours - Unemployment rates across different countries over the years, that we need to explore to find the relationship between working hours and these other aspects and if our common belief that working more leads to better economy or not.  

I've chosen to work with a custom dataset that I collected it has the data on: 
1 - Unemployment : https://data.oecd.org/unemp/unemployment-rate.htm
2 - Wage : https://data.oecd.org/earnwage/average-wages.htm
3 - Working Hours : https://stats.oecd.org/index.aspx?DataSetCode=ANHRS
4- GDP : https://data.worldbank.org/indicator/NY.GDP.MKTP.CD


I gathered the data and then did some cleaning for it to be ready for exploring it. 
I loaded the datasets one by one removing missing values and then merging them to form the final dataframe which contains all the data, I also dropped some of the columns to make the data more usable and easier to read as they were irrelevant to our explorations and then after merging dataframes, renaming columns, dropping duplicates, dropping missing values, I had the final dataframe ready for exploration.
So, I first performed univariate visualization to explore the different aspects of the data visualizing the distribution of each of the parameters using histograms or countplots from seaborn, finding very interesting outliers in the distribution of both the GDP and the unemployment rate. Then I started to look at relationships between the data in my dataset with bivariate visualization and analysis getting the correlation between the different variables and found that working hours had a strong effect on different aspects, and then I went to the multivariate analysis where I started to see how these parameters are distributed across the countries and over the years to see if the previous findings and different parameters were always like that or if there was an anomaly. Then I got to the conclusions shown in the last slides of the slideshow attached here as html file.

I got feedback from two of my friends, one who's working in the field of data analysis and told me to edit somethings and I did and from another one who doesn't know anything about data analysis to see if he gets the flow of the story of the data and he did.


Resources I used: 

- Pandas Docs 
- Stackoverflow
- Stackxchange

## Summary of Findings

In exploration I found that working hours for an employee has a positive correlation with unemployment rates as the more an employee works the rate of unemployment increases and we also found that as working hours increase the average wages decrease which shows that the increase of working hours really hurts both the employed and unemployed. Despite having a positive correlation with the GDP but also unemployment had a negative correlation with the GDP so we can't directly say that by increasing hours worked the GDP increases cause it negatively affects the unemployment rate too. We also encountered very strange points in the distribution of GDP and average wages as at the highest average wages the GDP was either very high or very low which shows that at poorer countries some get very high wages despite the GDP of the country.

## Key Insights for Presentation

For my presentation, I focus on the working hours and its effects showing first the distribution of the GDP showing the outlier in it as a hook to start exploring if the working hours had an effect or not, so i then go to the scatterplot between the working hours and the GDP which shows that there's a positive correlation between them suggesting the common belief, but then I go to the point of how increased working hours negatively affect the average wages with a very strong negative correlation. And then I go back to the outlier in the GDP showing the distribution of the GDP across countries and then showing the distribution of unemployment and working hours acroos these countries to prove that not only does the working hours have a negative effect on employeed (negative correlation with wages) but it also does a huge impact on unemployment rates which negatively affect GDP and economy as a whole.
