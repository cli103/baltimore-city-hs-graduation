# Baltimore City High School Graduation Rates Relating to Socioeconomic and Racial Factors

## Background
The [national high school graduation rate in 2016](https://www.edweek.org/teaching-learning/data-u-s-graduation-rates-by-state-and-student-demographics/2017/12#:~:text=The%20national%20high%20school%20graduation,earned%20diplomas%20in%20four%20years) is 84.1%, while the high school graduation rate in Baltimore public high school is only 78%. The low Baltimore high school graduation rate is an important issue, as it not only affects these individuals, but also the entire community according to [Public School Review](https://www.publicschoolreview.com/blog/what-is-the-impact-of-high-school-graduation-rates) and [Jobs for the Future](https://jobs4thefuture.medium.com/a-partnership-to-improve-the-lives-of-adults-without-a-high-school-diploma-10c743e5d23a#:~:text=Statistics%20suggest%20that%20a%20lack,as%20those%20who%20have%20graduated). For instance, high school dropouts are more likely to use government assistance and experience periodic unemployment. Only less than 30% of the jobs in the job market are available for high school dropouts, and the unemployment rate for them is 7.7%, which is 2.4% higher than the people with high school diploma. They also have higher recidivism rate and lower income (70% less) than people who completed high school. On the other hand, ["the loss of economic opportunities, fiscal costs from unrealized tax revenues, and additional public costs"](https://jobs4thefuture.medium.com/a-partnership-to-improve-the-lives-of-adults-without-a-high-school-diploma-10c743e5d23a#:~:text=Statistics%20suggest%20that%20a%20lack,as%20those%20who%20have%20graduated) from one person without high school diploma is estimated to be 258,240 USD loss for the community, and the combined income and tax losses from a group of high school dropouts is approximately 192 billion or 1.6% GDP loss for the country. Therefore, high school completion is an essential issue that Baltimore city governemt should not overlook. To further explore this ussue, we used Microsoft Excel to conduct data analysis on the education industry in Baltimore City and considered factors relating to socioeconomic status and race. We used open data from Baltimore City to generate a multiple regression analysis, simple linear regression analysis, correlation analysis and cluster analysis model to determine how the education in Baltimore city is impacted by socioeconomic and racial factors.

## Business Question
How is high school graduation rate impacted by race and median household income?

## Baltimore City Open Data:
[High School Completion Rate](https://data.baltimorecity.gov/datasets/bniajfi::high-school-completion-rate?geometry=-76.840%2C39.192%2C-76.401%2C39.378&selectedAttribute=compl14)

[Median Household Income](https://data.baltimorecity.gov/datasets/bniajfi::median-household-income)

[Percent of Students that are African American (non-Hispanic)](https://data.baltimorecity.gov/datasets/bniajfi::percent-of-students-that-are-african-american-non-hispanic?geometry=-77.051%2C39.192%2C-76.190%2C39.378&layer=0)

[Percent of Students that are White (non-Hispanic)](https://data.baltimorecity.gov/datasets/bniajfi::percent-of-students-that-are-white-non-hispanic?geometry=-77.051%2C39.192%2C-76.190%2C39.378)

Access the file [here]()

## Data Analysis
Click [here](https://github.com/cli103/baltimore-city-hs-graduation/blob/main/step-by-step-instructions) for a step-by-step instructions for the analysis. 

### Multiple Regression Analysis
<img width="604" alt="Screen Shot 2021-03-27 at 11 31 16 pm" src="https://user-images.githubusercontent.com/78471393/112720758-8832fd80-8f54-11eb-83cf-680154f2b683.png">

Above are the results of the multiple regression analysis we conducted. Median household income and the percentage of African American students in the school population were found to be significant predictors of high school graduation rates as the p-values were less than 0.05. The percentage of White students in the school population was not found to be a significant predictor as the p-value was greater than 0.05, however, remained low at 0.1263 indicating that the factors are still related. Moreover, as our analysis only considered data from 2016, it is possible a relationship exists in data from other years.

Our r-squared value was 0.60 indicating that our model accounted for around 60% of the variation in high school graduation rates. Our F-statistic was also well below 0.05.

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


## Conclusion


We found that our data analysis was related to some of the findings regarding education equity across the US and in Baltimore city. The Education Opportunity Project at Stanford University found that [increasing racial segregation has lead to achievement gaps](https://edopportunity.org/discoveries/segregation-leads-to-inequality/) and that [racial socioeconomic inequality predicts racial academic inequality](https://edopportunity.org/discoveries/racial-inequality-predicts-academic-inequality/). These results relate to our data analysis as we found that the percentage of African American students was a predictor for high school graduation and there was a strong negative correlation between African American students and median household income. While the percentage of White students was not a predictor, it was strongly positively correlated with median household income. Our results could indicate that possible racial effects could arise, particularly as Baltimore schools have high populations of African American students. 

Below is a graph taken from the [Education Opportunity Project at Stanford University website](https://edopportunity.org/discoveries/segregation-leads-to-inequality/) regarding increasing racial segregation in the US over the last 10 years.

<img width="316" alt="Screen Shot 2021-03-27 at 11 32 22 pm" src="https://user-images.githubusercontent.com/78471393/112720787-aef13400-8f54-11eb-8dfb-2a200a3cf44e.png">

We also found an article by [Johns Hopkins Applied Public Research](https://www.arcgis.com/apps/Cascade/index.html?appid=3ddf7ded140d4dc38bedc27d6c0e44f7) which found that School conditions affect access to education in Baltimore City. The graph below is a breakdown of reasons for lost time due to school infrastructure in Baltimore city. The key reasons are heating and cooling failures meaning that students often miss school because it is too hot during the summer and too cold during the winter. This perhaps provides some explanation as to why Baltimore city high school graduation rates are lower than the national average. 

<img width="350" alt="Screen Shot 2021-03-27 at 11 32 45 pm" src="https://user-images.githubusercontent.com/78471393/112720805-bd3f5000-8f54-11eb-8577-66515d8d1e70.png">

Baltimore City has begun addressing school conditions in public school by ["doubling its preventive maintenance spending on critical building systems, improving staffing in its engineering department, and implementing a district-wide monitoring system to allow for real-time tracking of temperature."](https://www.arcgis.com/apps/Cascade/index.html?appid=3ddf7ded140d4dc38bedc27d6c0e44f7) Additionally, to combat heating and cooling issues when there are insufficient funds to install central HVAC systems, Baltimore City Public Schools are installing vertical units in classrooms to provide heating and cooling for students and staff.

