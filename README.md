# Context

Our e-learning company offers courses on programming. 
Most of our courses are on web and mobile development, but we also cover many other domains, like data science, game development, etc. 
We want to promote our product and we'd like to invest some money in advertisement.

Our goal in this project is to find out the two best markets to advertise our product in.
Our product is a monthly subsription for learning of $59/ month.

To reach our goal, we could organize surveys for a couple of different markets to find out which would the best choices for advertising. 
This is very costly, however, and it's a good call to explore cheaper options first.

We can try to search existing data that might be relevant for our purpose. 
One good candidate is the data from freeCodeCamp's 2017 New Coder Survey. 
freeCodeCamp is a free e-learning platform that offers courses on web development. 
Because they run a popular Medium publication (over 400,000 followers), 
their survey attracted new coders with varying interests (not only web development), 
which is ideal for the purpose of our analysis.

The dataset is in `2017-fCC-New-Coders-Survey-Data.csv`.

# Objective

Each country in the dataset is considered a market.
Through our research, we will determine the two best countries to run marketing campaigns of the e-learning company and services.

# Process

The following steps describe our analysis:

- First, we check to see if the population wanted to learn the services the company provided by exploring the `JobRoleInterest` column.
- After removing all null rows in the `JobRoleInterest` column, we find that 86% of the population is interested in either Mobile Developer, Web Developer or both.
- Next, we create a frequency table to observe the locations of the individuals in the population by country in the `CountryLive` column.
- We create a new column, `money_per_month`, by dividing `MoneyForLearning` by `MonthProgramming` to check if the average coder is willing to spend for the subscription of the e-learning company.
- We clean up outliers for a better analysis.

# Results

After fitlering `JobRoleInterest` to about 7,000 coders, we find that the majority of the interested coders live in the USA.
After cleaning the extreme outliers, we find that the USA also has the best potential customers as they are willing to spend averagely $122/ month on learning.
Thereby, USA is the best market to run our market campaign in.

However, for our second best market, there is a debate between Canada and India. Coders in Canada averagely spend $93/ month vs coders in India spend $66/ month which are both above the price point for our product.
But, India has twice as more potential customers than Canada.

In the end, we decided on Canada being the second best pick as it would be easier to market in considering its general location to the USA and delivering similar marketing strategies for these two countries.
