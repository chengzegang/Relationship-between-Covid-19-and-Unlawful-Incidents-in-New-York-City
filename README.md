# the Relationship between Covid-19 and Unlawful Incidents in New York City
## Abstract
The Covid-19 pandemic has been a devastating global incident lasted for more than a year with more than 100 million confirmed cases and almost 3 million deaths worldwide. The impact of COVID-19 on us is non-negligible, not only to those who were infected, but also to anyone living under the atmosphere of this contagious virus. In order to stop COVID-19 from spreading, people are required to practice 6-feet social distancing ,keep away from any crowded events and stay at home.
However, these actions also altered the way we live. People are “locked” inside, living with budgets, lack of resources, and might raise hate against each other. Therefore, in order to understand how negatively COVID-19 has affected us, we are going to investigate whether there is a relationship between the number of COVID-19 cases and the number of different types of unlawful incidents among different districts in New York City. Also, we are going to see how other factors such as quarantine policies, lockdown and economic status play a role among them. Especially, how COVID-19 affected hate crimes against Asians, and how the economy affected housing situations and evictions.

## Introduction
### Overall NYPD Complaints
People living in households in the US that have an income level below the Federal poverty threshold have more than double the rates of violent victimization compared to individuals in high-income households. Therefore, we can hypothesis that districts with high crime rate are usually places with large poverty community. In other words, we can not only insvestigate whether Covid-19 leads to any change in number of incidents, but also whether places with high crime rate leads to more Covid-19 cases due to their financial status.
### Evictions
There are certain types of unlawful incidents that might have much closer relation with Covid-19, Such as Evictions. TODO:...
### Hate Crimes against Asians
Also, Hate Crimes agaisnt Asians is another example. TODO:
## Methods
### Data Cleaning
For categorical data, we group them by columns to see if there are outliers or erroneous input. In some cases, for ambiguous values, we replace them with the value ‘Others’ on condition that it does not affect our analysis. For continuous data, we define a reasonable range and check if there are any rows that fall out of the range and remove them.

When reading csv files into tables for future use, we also trimmed down some of the columns that are not useful for our analysis, and also simplified some column names for our convenience and better readability.

Some of the challenges we faced are the integration of data and choosing the data to use based on their connection. For example, for covid data alone, we have a folder of various kinds of data, from case counts by date to case counts by borough, or by zip code. Depending on different use cases, we need to clean different data sets. What we did was assigning each member a specific aspect to integrate and clean data. Which reduces workload and improves efficiency.

When understanding and cleaning the data, another challenge we faced is how to interpret the data. Take the data from the NYC OCA Housing Court Records as an example; we wanted to find out among all the Housing Court Records which ones can be classified as evictions filing in New York City. However, this data set contains many legal terms to which all team members didn't understand. We then researched New York City's housing law and tenant's rights, and finally, we were able to interpret, clean, and integrate the complex data set.

### Relative Crime Index and Weighted Difference on Relative Crime Index
There are 404851 recorded complaints in 2020 and 450976 in 2019, however, according to NYPD, there are about 95000 incidents for both two years, which means that our data is not comprehensive. Thus, we cannot directly compare numbers in these two dataset. In other words, we can assume that each dataset has the same distribution as the overall complaints and we introduce a new stats called Weighted Relative Crime Index (Weighted RCI) to continue our analysis. This methods is pretty straight forward: RCI for each district is the ratio between its number of complaints and the mean of that year.

For the analysis of overall unlawful incidents, we are going to compare the RCI of each districts between 2019 and 2020. However, for districts with fewer complaints, RCI will increase or decrease a lot even if there is only a small amount of chance on total number of complaints, and for those places with lots of complaints, a small change on RCI actually means lots of complaints. Therefore, we then introduced Weighted Difference on RCI, which is the product of Diffrence on RCI on two years and the mean of number of incidents of 2019 and 2020.

## Results
### Relationship between Covid-19 and Overall Unlawful Incidents
First of all we can take a look of overall complaints in NYC to have a basic understanding:

## Discussion


## Datasets
