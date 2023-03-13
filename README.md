# Want to know how to be a billionaire?

Come with us (Isabella & Sri) as we go through the Forbes 2022 dataset of the top billionaires and companies in the world! 


## About our project

Through several exploratory analyses, we delve into 

## how_to_become_a_billionaire_tidying

  Our step by step process of organizing and manipulating the forbes 2022 datasets to fit our analytical needs. 

  In the companies dataset, given all of our values were in the format: $100 B, we first used the separate function on the profit, sales, assets, and market_value columns to separate out the B/M from each cell. After setting these letters into new columns, with the help of Hannah and other R teachers, we utilized the gsub function to remove the $ from each cell. Once this was complete, we ran into yet another issue: the values were a mix of millions and billions. So deciding to turn all of values into numeric, we then used case_when to divide by values by 1000 whenever they had 'M' present. However, this did not work due to the presence of commas, so we again utilized gsub to remove any instances of commas. Once all of this was complete, we removed the columns that held unnecessary B and M values and renamed sales, profit, assets, and market_value to their name_bil. 

## Analysis_of_Category_field

  In this file, we manipulate the billionaires dataset to create columns that show what field the top billionaires accumulated their wealth from. 

  We did this by creating a new column called 'category' and utilizing the function case_when to assign company fields to each company. We did this by researching the top 15 companies by highest profit. Then we manually assigned each company to a respective field. This data allowed us to see which feilds had the most profitable companies.
  
  
## Exploratory_age_analysis

  This file explores how old should you be to be more profitable and maximise your chances of being a billionaire. 

  

## Analysis_of_country

## Shinyapp_NPM