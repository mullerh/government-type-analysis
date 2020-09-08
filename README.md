# Overview

## What problem is being solved?

Determining the effect that different government types have on their average GDP per capita. While also trying to control the variable of unemployment to focus on the impact of government types rather than percentage unemployed.

## Information source

Dataset including: country names, unemployment rate, gdp per capita, government types, and population. From a [github source](https://github.com/ghenshaw/datasets/blob/master/country_per_cap_gdp_unemployment_gov_type_pop.csv) which was downloaded.

## Why is it interesting to <u>me</u>?

I have always been interested in statistics since I was young, especially country data. I find it fascinating to find small trends in a huge mess of numbers. On top of that, it’s always interesting for to look at government types with an objective lens, since when I look forward towards how I will push for the world to be shaped, it only makes sense to fully consider each option without the processing of one’s own bias.

# Design Choices

## How I used systematic program design?

I tackled the problem not as one large problem, but as many seperate and slightly connected problems with the help of **helper fuctions**. I also planned the entire process out by having the signatures of most functions before any of their bodies were built, so that I don't waste time with what I don't need, and to make sure all my logic of which data types to use would be correct.

## What design choices did I have to make? And Why did I make those choices?

To only include the bar chart and not having a scatterplot showing where the line of best fit is, used in some equations, came from. I chose to leave it out as although it can be interesting to see where the line came from, it could make it confusing to know which chart was the most important and containing the results.

Also, I switch to using a line of best fit to determine expected results and away from comparing countries based on where they ranked in terms of unemployment. I made this switch after I realized that this could lead to some countries, and government types, being artificially boosted in how they perform just based on a lucky ranking placement. 

# Problem Solving

## How did I solve the problem?

I found the expected GDP per capita a country should have based on its unemployment rate. I did this by finding the equation for the line of best fit (had all the countries been placed on a scatter plot, the x values would be unemployment rate, and the y values would be the gdp per capita). Thus by inputting the x (the unemployment of a country) into the y=mx+b equation the result would yield the expected gdp per capita. Then the actual result of the country's gdp per capita could be compared to determine if it is overperforming or underperforming. After the percentage of each government type's countries that were overperforming was found, those percentages could be exported as a bar graph.

# Most Challenging

The most difficult part of the project was finding the equation of the line of best fit for the data, and then using that equation to interpret the data. This is because this line was essentially being calculated from a graph that was not intended to be visually produced, so the graph and the line's implementation had to be kept on a 'theoretical' level, without the confidence of seeing it for myself.

# Future Work

Using the same systematic design skills I used for this project, I could similarly do studies on other types of country data, and see the effects of one type of country data on the other. This design process works nicely with the attempt to remove unconscious bias and unwanted variables, as the process makes you focus on the outcome of the small picture, rather than on what you want the final outcome to be. For example controlling another variable would just be adding more helper functions rather than redesigning the whole thing. Also, I could continue with the same topic and further remove variables that aren't directly part of government types and GDP per capita, such as how abundant natural resources are; or I could research a completely new correlation.
