# Want to know how to be a billionaire?

Come with us (Isabella & Sri) as we go through the Forbes 2022 dataset of the top billionaires and companies in the world! 

## About our project

We completed this project by pair programming, working together on most parts. Through several exploratory analyses, we delve into:

## Tidying the Billionaire and Companies data

Our step by step process of organizing and manipulating the forbes 2022 datasets to fit our analytical needs. 

In the companies dataset, given all of our values were in the format '$100 B', we first used the separate function on the profit, sales, assets, and market_value columns to separate out the B/M from each cell. 

After setting these letters into new columns, with the help of Hannah and other R teachers, we utilized the gsub function to remove the $ from each cell. Once this was complete, we ran into yet another issue: the values were a mix of millions and billions. So deciding to turn all of values into numeric, we then used case_when to divide by values by 1000 whenever they had 'M' present. However, this did not work due to the presence of commas, so we again utilized gsub to remove any instances of commas. Once all of this was complete, we removed the columns that held unnecessary B and M values and renamed sales, profit, assets, and market_value to their name_bil. 

## Analysis of Category (field) to be in 

In this file, we manipulate the datasets to create columns that show what field the top billionaires accumulated their wealth from. 

We did this by creating a new column called 'category' and utilizing the function case_when to assign the respective fields (categories) to each company. We did this by filtering the top 20 companies by highest profit. Then we manually assigned each company to a respective field. This data allowed us to see which fields had the most profitable companies. 

We then compared this to the fields of the top 20 billionaries, arranged by final worth. Using both of these, we determined which field it was best to be in to have the highest profits in a company as well as the greatest chances of accumulating wealth.
  
## Age analysis

This file explores how old you should be and what year you should be born to be more profitable and maximize your chances of being a billionaire. Using prior data about the age category with the highest proportion of billionaires, we created an estimation of when you could be most profitable in this lifetime.

## Analysis of Country

This file does many different location analyses, such as top countries and top states, of billionaires and companies to show the optimum locations to be in to have the best wealth margins.

## Shinyapp_NPM

Our app explores the (profits)/(sales revenue) ratio, or rather the net profit margin of the top 100 companies. 
  
In addition to this displayed relationship, the App allows for you to select for the top 10 countries as well as change the size of the points on the graph.
