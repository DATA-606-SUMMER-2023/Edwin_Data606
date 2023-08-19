 
<p><strong><isalign="center"><br>Edwin Brown
<br>Homelessness Population</br>
<br>UMBC Data Science Capstone 606</br>
<br>Summer 2023 </br></strong></p>
 
# Background 
****** Homelessness is a worldwide issue, and some commonalities can be found globally as an attribute to homelessness. According to the National Library of Medicine, homeless is defined as an individual who lacks a fixed, regular, and adequate nighttime primary residence, and lives in a publicly operated shelter to provide temporary living. (National Library of Medicine, June 2023).  At the beginning of this project, I wanted to understand how we could use machine learning to solve homelessness and what I have discovered is some foundational insight for some of the causes.   The data collected and aggregated is a collection for the year 2016 and not all the information has not been captured to   conclude the reason for homelessness but only has some insight that suggests a reasonable factor of influences.   
The data used to find some of the causes comes from three sources – HUD, FRED and Kaggle. FRED is short for Federal Reserve Economic Data, and some of data from FRED had median income for all of United States (U.S.)  as an economic factor. HUD stands for Housing Urban Development and some of the data capture was the climate information for the United States (U.S.) such as the average temperature in the summer and the average precipitation among the U.S. in 2016.  Additionally, HUD data , captured the overall population for all 50 states and U.S.  homeless population, unemployment labor rate and total number of Shelter. The total number of shelters is counted as emergency places of refuge. 
Nevertheless, going through this effort has its challenging moments. One of the challenges is understanding how to use measurable factors; for instance, one of my variables in the dataset was population of the U.S and homeless population. Well, counting the population was informative but it does not necessarily help to tell a compelling story when comparing the actual impact of homelessness and just counting the population could be misleading. For example, California has a larger homeless population than Hawaii and a larger overall population of people. At first glance, one would conclude that California has the worst cases of homelessness, but contrary to belief, Hawaii rate of homelessness is approximately 2 times higher than California. In order to aid in capturing an unfamiliar perspective, using ratio, percentage, proportion, and rate can help explain relationships and provide a prospective of actionable activity.    
 
# Description of Data Elements and   EDA 

- Upon discovery, asking the right questions and making assumptions could be invaluable. For instance, using unemployment rate and economic factors would be intuitive and make sense to help explain homelessness. However, using precipitation and temperature is not as instinctive to support factors of homelessness. Fortunately, and unfortunately, climate factors have some influence on the homeless population. For instance, the lower the precipitation and the higher the temperature, the higher the rate of homeless population.  
Most of the data involved are continuous values. Also, some of the features were used to aggregate data and others were used in the machine learning model. For obtaining, rate and proportion and percentage to aid in processing relationships amongst the features, some of the features were derived. For example, the rate of homelessness was derived from total population of the U.S and total population of homelessness per 10,0000 in population. Additionally, a ratio of shelter to homelessness was calculated and the data indicated there were not enough shelters per homeless people to provide shelter to aid in reducing the homeless rate. Additionally, the total shelter data was significant enough to add to the machine learning model which will be discussed later.    
During the phase of EDA, the data that was acquired were continuous values which indicated that certain models had to be used when implementing a machine learning model.  Most of the data had to be cleaned using python scripts. By making sure some of the data types were strings and floats and integers aided in making some of the aggregated data more useful and significant.   Also, out of the 19 features only 5 were significant according to the OLS regression model . The 5 features which was used to create the machine learning model to aid in predicting rate of homelessness were total shelter, average unemployement rate, median income dollar, precipitation, summer temperature  and rate of homelessnes was the dependent variable.  
- Out of the 5 features, there were little to no multicollinearity and the features that reference climate change were negative correlated   and the economic data such as labor unemployment, median income, sheltered were positive correlated. All the correlation to the rate of homelessness was weak given that were numerically less than 55% which does not necessarily indicate a strong relationship. However, each of the features when plotted on a graph, bar chart or mapped visually show some interesting patterns. For example, besides the economic level indication which influences homeless such as low median income per 10,000-person and high unemployment rate which would normally stand out and indicate some influence on homelessness, climate weather mentioned in the data also indicated some influences of impact on homelessness.  On average each state does not have enough shelters to serve the homeless population in each state; for example, Hawaii and Arizonia do not have enough shelter to serve its homeless population. All the features mentioned seem to indicate an impact on the influence of homelessness in each state. 
 
# Machine Learning (ML) model 
- While testing the data using ML, I needed to use models that would accommodate continuous variables. Thus, I chose to use items such as Ridge, SGD, Decision tree, Random Forest, Bayesian Ridge and Lasso. From the result of each model, the R-squared and mean square error was low which indicate I may need more data or there may be other combinations of features that could be used to increase the R-squared and reduce the mean square error.  The best mode used was SGD which measured at a higher rate of the R-squared of .44 and a low means squared error of 206 and a cross validation score of .20 which was better measure than the other models. This results does not conclude useful for deployment;however, it does create a baseline to continue researching model and method for creating a better model. 
    
 
 
 # Conclusion 
- At the beginning of the project, I ranked the homelessness case from the it worst based on population. From the findings there seem to be factors that influence the homeless population such as economic indicators such as median income, unemployment rate and access to shelters and climate weather such as percipitaition and higher temperatures. I suspect that other factors have an impact on the population, which were not indicated in the project such as education, crime levels and access to health care.  Also, having aggregated data to show rates, proportion, percentage, and ratio aids in providing insight that may go unnoticed if not pursued. The top five states with the highest rate of homelessness are Hawaii, New York, Arizonia, Oregon and California and the lowest rate of homelessness occurs in states such as Arkansas, Mississippi, Kansas, Virgina and West Virginia.  Each state has it on weakness and strength in relations to its economics strength and weakness, geographic location and climate and policies on the homeless which more than likely needs a deeper understanding of impact of the homeless population. 
 
# Future and Research 
 - For the forseeable future, more features will need to be tested  such as crime , education, race, and health  and drinking water accessible.  Also the results and collected features will need to be vetted by expertise  that serve the homelessness population in order to gauge ML model and finding. So a search for this experise will need to be a part of the research.  Additionally, using GNN and other machine learning model will be tested to obtain better result.  
 
# YouTube Link 
 [[https://studio.youtube.com/video/unrfTUUf4Nk/edit](https://www.youtube.com/watch?v=unrfTUUf4Nk)](https://www.youtube.com/watch?v=unrfTUUf4Nk) 
 
# ReadmeLink 
README.md 
 
# PowerPoint slide link 
EdwinBrown_Data_690_Capstone_presentation-4.pptx 
 
 
 
 
<p align="center"> # References </p>
 
https://bookdown.org/bfischer_su/data_3320_bookdown/homeless.html#data-preparation-1 
https://www.hudexchange.info/sites/onecpd/assets/File/Guide-for-Counting-Unsheltered-Homeless-Persons.pdf 
 
https://www.kaggle.com/code/adamschroeder/homelessness-in-the-united-states-of-america 
https://fred.stlouisfed.org/ 
https://www.hudexchange.info/ 

