# final-project-FD

Question: 
     “Food Desert” is a long-lasting issue in metropolitans and has attracted much attention because the poor local food environment might deteriorate health status of local people. Both the growth of large supermarkets in outskirts and the economic segregation led to limited access to healthy food in inner cities. And a diet with less nutrition provided by not large supermarkets but fast food restaurants could make health outcomes poor.

     Our goal is to get the correlation or causality between health outcomes and food access from the data in Chicago. The U.S. Department of Agriculture defines a food desert as an area with a poverty rate of at least 20 percent and where at least a third of the population lives more than a mile from a supermarket or large grocery store. There has been some amount of research on food deserts (Renee E. Walker et al, 2010 etc.), but we don’t know the exact number of people living in food deserts in Chicago. The new law (HB3157) approved last month requires Illinois to track food deserts, and the City of Chicago is pursuing solutions such as the collaboration with Whole Foods to solve the problem. Thus, it is a good timing to reconsider the importance of the policy.


Datasets:
     We mainly need two datasets, which have the data on locations of grocery stores and the data on the public health data including hospitalizations of chronic diseases. Both the data can be extracted from Chicago Data Portal at the format of CSV or JSON.
     
A. Grocery Stores 2011 (491 samples)
https://data.cityofchicago.org/Community-Economic-Development/Grocery-Stores-2011/4u6w-irs9

B. Public Health Statistics- Diabetes hospitalizations in Chicago, 2000 - 2011 (49 samples)
https://data.cityofchicago.org/Health-Human-Services/Public-Health-Statistics-Diabetes-hospitalizations/vekt-28b5

C. Public Health Statistics- Selected public health indicators by Chicago community area (77 samples)
https://data.cityofchicago.org/Health-Human-Services/Public-Health-Statistics-Selected-public-health-in/iqnk-2tcu

     Dataset A has the column of zip code and community name, so we can merge A with B or C easily. However, we want to know the density of grocery stores to check the accessibility of food. To calculate this, we need the data on housing units per zip code or community. They could be downloaded with the API of American Community Survey.

D. American Community Survey 5-Year Data (2009-2015) housing units (DP04-0001E)
https://api.census.gov/data/2015/acs/acs5/profile/variables.html

Possible extensions:
     Some kinds of diseases could be tested to assess the effect of food access and get the best regression model. In addition, we would map the data for food deserts and build the website if we could.

