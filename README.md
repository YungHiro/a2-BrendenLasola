# A2: U.S. COVID Trends

## Overview
In many ways, we have come to understand the gravity and trends in the COVID-19 pandemic through quantitative means. Regardless of media source, people are consuming more epidemiological information than ever, primarily through reported figures, charts, and maps. 

This assignment is your opportunity to work directly with the same data used by the New York Times. While the analysis is guided through a series of questions, it is your opportunity to use programming skills to ask more detailed questions about the pandemic.

You'll load the data directly from the [New York Times GitHub page](https://github.com/nytimes/covid-19-data/), and you should make sure to read through their documentation to understand the meaning of the datasets. 

Note, this is a long assignment, meant to be completed over the two weeks when we'll be learning data wrangling skills. I strongly suggest that you **start early**, and approach it with patience. We're asking real questions of real data, and there is inherent trickiness involved. 

## Analysis
You should start this assignment by opening up your `analysis.R` script. The script will guide you through an initial analysis of the data. Throughout the script, there are prompts labeled **Reflection**. Please write 1 - 2 sentences for each of these reflections below:

- What does each row in the data represent (hint: read the [documentation](https://github.com/nytimes/covid-19-data/)!)?
  
  National has 3 Rows while county and state have added features. Some rows are self-explanatory especially in the county and states column, things like "State" and "County" are self explanatory. This is the state in the US and the county in that specific state. They all share cases and deaths, these are  both confirmed and probable cases/deaths. One thing that is different from national to state/county is the addition of fips, Fips or fips code is a geographical identifier that makes it easier for people to use this data to create map files or population data.  
 
- What did you learn about the dataset when you calculated the state with the lowest cases (and what does that tell you about testing your assumptions in a dataset)?
  
  The "state" with the lowest cases is the Norther Mariana Islands which a US territory. Some of the results in this dataset might be affected by the fact that it includes US territories. If I truly wanted to know what state had the lowest number of cases I would have to get rid of US territories from the raw file. 

- Is the location with the highest number of cases the location with the most deaths? If not, why do you believe that may be the case?
  
  There are more cases in California but there are more deaths in NY. This might be attributed by the fact that California is just a larger state compared to NY, in terms of population and mass. It wouldn't be surprising that NY has the most deaths because a large amount of its population are located in one city. They might not have a lot of resources needed to support the amount of people that are getting sick from COVID, leading to more deaths. 
 
- What do the plots of cases and deaths tell us about the  pandemic happening in "waves"? How (and why, do you think) these plots look so different?

    I think the pandemic coming in waves can be allocated to a lot of different factors, one thing that affects the cases side of things is the lack of testing. When the pandemic started there were a lack of tests available, those waves at the start are heavily affected by the lack of tests. When new tests are available cases will rise because there are more people that are counted to have COVID-19. 

- Why are there so many observations (counties) in the variable `lowest_in_each_state` (i.e., wouldn't you expect the number to be ~50)?
  
  There are more than 50 because this data set also includes US Territories, for example in lowest_in_each_state it has "Tinian. Northern Mariana Islands". 

- What surprised you the most throughout your analysis?
  
  The most surprising observation for me was that NY had the most deaths. I had an idea that big cities would have large amounts of deaths but it is very surprising to me that NY got hit the most in terms of deaths compared to other places like California or Washington. Also, the fact that California had the most cases was also surprising for me, I thought that Texas had the most cases. 