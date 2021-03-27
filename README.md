# Baltimore City High School Graduation Rates Relating to Socioeconomic and Racial Factors

## Background
The [national high school graduation rate in 2016](https://www.edweek.org/teaching-learning/data-u-s-graduation-rates-by-state-and-student-demographics/2017/12#:~:text=The%20national%20high%20school%20graduation,earned%20diplomas%20in%20four%20years) is 84.1%, while the high school graduation rate in Baltimore public high school is only 78%. The low Baltimore high school graduation rate is an important issue, as it not only affects these individuals, but also the entire community according to [Public School Review](https://www.publicschoolreview.com/blog/what-is-the-impact-of-high-school-graduation-rates) and [Jobs for the Future](https://jobs4thefuture.medium.com/a-partnership-to-improve-the-lives-of-adults-without-a-high-school-diploma-10c743e5d23a#:~:text=Statistics%20suggest%20that%20a%20lack,as%20those%20who%20have%20graduated). For instance, high school dropouts are more likely to use government assistance and experience periodic unemployment. Only less than 30% of the jobs in the job market are available for high school dropouts, and the unemployment rate for them is 7.7%, which is 2.4% higher than the people with high school diploma. They also have higher recidivism rate and lower income (70% less) than people who completed high school. On the other hand, ["the loss of economic opportunities, fiscal costs from unrealized tax revenues, and additional public costs"](https://jobs4thefuture.medium.com/a-partnership-to-improve-the-lives-of-adults-without-a-high-school-diploma-10c743e5d23a#:~:text=Statistics%20suggest%20that%20a%20lack,as%20those%20who%20have%20graduated) from one person without high school diploma is estimated to be 258,240 USD loss for the community, and the combined income and tax losses from a group of high school dropouts is approximately 192 billion or 1.6% GDP loss for the country. Therefore, high school completion is an essential issue that Baltimore city governemt should not overlook. To further explore this issue, we used Microsoft Excel to conduct data analysis on the education industry in Baltimore City and considered factors relating to socioeconomic status and race. We used open data from Baltimore City to generate a multiple regression analysis, simple linear regression analysis, correlation analysis and cluster analysis model to determine how the education in Baltimore city is impacted by socioeconomic and racial factors.

## Business Question
How is high school graduation rate impacted by race and median household income in 2016?

## Baltimore City Open Data:
1. [High School Completion Rate](https://data.baltimorecity.gov/datasets/bniajfi::high-school-completion-rate?geometry=-76.840%2C39.192%2C-76.401%2C39.378&selectedAttribute=compl14): This [dataset](https://github.com/cli103/baltimore-city-hs-graduation/files/6216253/High_School_Completion_Rate.xlsx) contains information of the percentage of students in 55 communities who satisfy graduation requirements for Maryland High School Diploma or the requirements for a Maryland Certificate of Program Completion from 2010 to 2017.
2. [Median Household Income](https://data.baltimorecity.gov/datasets/bniajfi::median-household-income): This [dataset](https://github.com/cli103/baltimore-city-hs-graduation/files/6216258/Median_Household_Income.xlsx) contains median household incomes of 55 communities from 2010 to 2019.
3. [Percent of Students that are African American (non-Hispanic)](https://data.baltimorecity.gov/datasets/bniajfi::percent-of-students-that-are-african-american-non-hispanic?geometry=-77.051%2C39.192%2C-76.190%2C39.378&layer=0): This [dataset](https://github.com/cli103/baltimore-city-hs-graduation/files/6216269/Percent_of_Students_that_are_African_American_.non-Hispanic.xlsx) contains the percentage of Black/African American students that attend Baltimore City Public School from 2010 to 2017. 
4. [Percent of Students that are White (non-Hispanic)](https://data.baltimorecity.gov/datasets/bniajfi::percent-of-students-that-are-white-non-hispanic?geometry=-77.051%2C39.192%2C-76.190%2C39.378): This [dataset](https://github.com/cli103/baltimore-city-hs-graduation/files/6216275/Percent_of_Students_that_are_White__non-Hispanic_.xlsx) contains the percentage of White students that attend Baltimore City Public School from 2010 to 2017. 

## Data Analysis
Click [here](https://github.com/cli103/baltimore-city-hs-graduation/blob/main/step-by-step-instructions) for a step-by-step instructions for the analysis and [here](https://github.com/cli103/baltimore-city-hs-graduation/blob/main/midterm-project-data-analysis-2016.xlsx) for the Excel analysis files.

### Multiple Regression Analysis
<img width="769" alt="Screen Shot 2021-03-28 at 10 07 01 am" src="https://user-images.githubusercontent.com/78471393/112737275-5dc15e80-8fad-11eb-9a53-d9f61287b661.png">

Above are the results of the multiple regression analysis we conducted. Median household income and the percentage of African American students in the school population were found to be significant predictors of high school graduation rates as the p-values were less than 0.05. The percentage of White students in the school population was not found to be a significant predictor as the p-value was greater than 0.05, however, remained low at 0.1263 indicating that the factors are still related. Moreover, as our analysis only considered data from 2016, it is possible a relationship exists in data from other years.

Our r-squared value was 0.36 indicating that our model only accounted for around 36% of the variation in high school graduation rates. However, our F-statistic was well below 0.05.

### Simple Linear Regression Analysis
For the purposes of visualing the significant predictors of high school graduation, we also generated some simple linear regression graphs. The graphs below demonstrate the relationship between the high school graduation rate and median household income and the high school graduation rate and the percentage of African American students.

![Picture 1](https://user-images.githubusercontent.com/78471393/112720866-fecffb00-8f54-11eb-8018-3c3e259303a9.png)

The graph above indicates that a one unit increase in median household income results in a 0.0001 unit increase in high school graduation rate.

![Picture 2](https://user-images.githubusercontent.com/78471393/112720869-01caeb80-8f55-11eb-991e-0fdfd2039c2d.png)

The graph above indicates that a one unit increase in the percentage of African American students in the student population results in a 0.0363 unit decrease in high school graduation rate.

### Correlation Analysis
<img width="563" alt="Screen Shot 2021-03-27 at 11 31 37 pm" src="https://user-images.githubusercontent.com/78471393/112720761-954fec80-8f54-11eb-83dd-5d70c266d740.png">

Our correlation analysis found that high school graduation rates were positively correlated with median household income and the percentage of White students, and negatively correlated with the percentage of African American students.

We also found that median household income was strongly positively correlated with the percentage of White students, and strongly negatively correlated with the percentage of African American students.

### Cluster Analysis
We also performed cluster analysis with three anchor nodes, which were found to be Glen-Fallstaff, Northwood, and Greater Roland Park/Poplar Hill.

<img width="946" alt="Screen Shot 2021-03-27 at 1 20 25 PM" src="https://user-images.githubusercontent.com/70459912/112728793-53488b80-8eff-11eb-8d3a-cbf7286829ff.png">
<img width="1326" alt="Screen Shot 2021-03-27 at 2 01 18 PM" src="https://user-images.githubusercontent.com/70459912/112729904-e932e500-8f04-11eb-8be3-fe6c48543018.png">

This plot displays the average z scores of high school completion rate, median household income,  percetage of White students, and percentage of African American students for all three clusters. For cluster 1, the average high school completion rate, median income, and percentage of White students are all below the mean, while the percentage of African American students is slightly above the mean. For cluster 2, its high school completion rate and percentage of African Americans are higher than the mean, the  median household income is about the same as the mean, and the percentage of White students is lower than the mean. For cluster 3, the high school completion rate, median income, and the percentage of White students are lower than the mean while the percentage of African American students are lower than the mean. 

<img width="1331" alt="Screen Shot 2021-03-27 at 1 47 26 PM" src="https://user-images.githubusercontent.com/70459912/112729536-f949c500-8f02-11eb-92fc-e2e64ca8b660.png">

This table summarizes the number of communities, average high school completion rate, median household income (USD), White students (%), and African American students (%) for the three clusters. Cluster 1 has the lowest average high school completion rate and median household income, while its percentage of White students and percentage of African American students fall in the middle. There are a total of 32 communities (58%) in cluster 1. On the other hand, cluster 2 (27% of the communities) has the highest percentage of White student and the lowest percentage of African American students. Its high school completion rate and median income are the second highest. Lastly, there are 8 communites (14.5%) in cluster 3. It has the highest high school graduation rate, median income, and percentage of White student. Its percentage of African American student is the lowest. 

From cluster analysis, we can see that the communities with higher median income tend to have higher high school completion rate, and that the effects of race on high school graduation rate is not as prominant, which is consistent with the regression analysis and correlation analysis. This result suggests that economic factor plays a significant role in education in Baltimore city in 2016.

### Error Analysis
There are a few limitations of our data. For example, we only looked at the data in 2016, so the results might not always reflect the trends in other years. Also, the median household income data in this analysis is for everyone living in the communities, not just for the households whose children go to public school. It might be a problem since the high school completion rate used in the analysis were collected from studens studying in public school. Lastly, students might not go to schools in the area they live, which could potentially skew the data.

## Conclusion
We found that our data analysis was related to some of the findings regarding education equity across the US and in Baltimore city. The Education Opportunity Project at Stanford University found that [increasing racial segregation has lead to achievement gaps](https://edopportunity.org/discoveries/segregation-leads-to-inequality/) and that [racial socioeconomic inequality predicts racial academic inequality](https://edopportunity.org/discoveries/racial-inequality-predicts-academic-inequality/). These results relate to our data analysis as we found that the percentage of African American students was a predictor for high school graduation and there was a strong negative correlation between African American students and median household income. While the percentage of White students was not a predictor, it was strongly positively correlated with median household income. Our results could indicate that possible racial effects could arise, particularly as Baltimore schools have high populations of African American students. 

Below is a graph taken from the [Education Opportunity Project at Stanford University website](https://edopportunity.org/discoveries/segregation-leads-to-inequality/) regarding increasing racial segregation in the US over the last 10 years.

<img width="316" alt="Screen Shot 2021-03-27 at 11 32 22 pm" src="https://user-images.githubusercontent.com/78471393/112720787-aef13400-8f54-11eb-8dfb-2a200a3cf44e.png">

We also found an article by [Johns Hopkins Applied Public Research](https://www.arcgis.com/apps/Cascade/index.html?appid=3ddf7ded140d4dc38bedc27d6c0e44f7) which found that School conditions affect access to education in Baltimore City. The graph below is a breakdown of reasons for lost time due to school infrastructure in Baltimore city. The key reasons are heating and cooling failures meaning that students often miss school because it is too hot during the summer and too cold during the winter. This perhaps provides some explanation as to why Baltimore city high school graduation rates are lower than the national average. 

<img width="350" alt="Screen Shot 2021-03-27 at 11 32 45 pm" src="https://user-images.githubusercontent.com/78471393/112720805-bd3f5000-8f54-11eb-8577-66515d8d1e70.png">

Baltimore City has begun addressing school conditions in public school by ["doubling its preventive maintenance spending on critical building systems, improving staffing in its engineering department, and implementing a district-wide monitoring system to allow for real-time tracking of temperature."](https://www.arcgis.com/apps/Cascade/index.html?appid=3ddf7ded140d4dc38bedc27d6c0e44f7) Additionally, to combat heating and cooling issues when there are insufficient funds to install central HVAC systems, Baltimore City Public Schools are installing vertical units in classrooms to provide heating and cooling for students and staff.

Our analysis can serve as an initial step for the Baltimore city government to implement policies that aim to increase high school graduation rate. Baltimore city government should first focus on investing in infrastructures in the high schools in the communities listed in cluster 1. They should especially improve the cooling and heating system in the classroom as they were the primary interruptions to students' learning. In addition, Baltimore city government should decrease racial segregations in school by encouraging mixed student populations to decrease achievement gaps and promote education equity. For future research, we can perform similar analysis on data of the other years to get a more hoslitic view of how the education in Baltimore city is impacted by economic and racial factors. On the other hand, we could investigate other variables such as the teachers’ experiences, school spending per students and see how these factors affect education in Baltimore city to come up with other solutions to increase high school graduation rate in Baltimore city. 

