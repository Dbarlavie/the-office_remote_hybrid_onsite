# The Office
## Remote/Hybrid/On-Site Work

Four years ago, almost to the day we were hit with a worldwide pandemic that sent all of us to lockdown,  some of us ,for the first time, to work from home. 
Remote workers are percieved more productive because they have no commute, fewer distractions, more time for family, exercise, and overall better work-life balance. 
But are there also benefits to working from the business premesis? The office? 

The dataset I analysed included a questionnaire answered by 65thousand employees who work on some scale between fully remote to fully on site. Among basic details such as gender,age, education and income, they also rated what are the benefits of WFH(working from home) and WBP(working on business premises), and what is their top 3 most important benefits. 
On the basis of the participants traits and wishes and work status, I wanted to try to predict in what kind of format they would work- Remote, Hybrid or OnSite. 

## Data sources
WFH Research - https://wfhresearch.com/gswadata/

## Presentation & Public Tabeau links
https://docs.google.com/presentation/d/1iNBrTxb6NQ3Kyft0XaXrtrNrVSJpljVZ_IOBQQH5FPw/edit?usp=sharing
Employer vs. Employee - https://public.tableau.com/views/employersvs_employees/Sheet1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
Hybrid workers from which Industry - https://public.tableau.com/views/Industry_17104262072890/2023HybridworkersfromwhichIndustry?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
Making the Most of Less Commute - https://public.tableau.com/views/WFHcommutefamily/Sheet1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
WFH WBP Gender - https://public.tableau.com/views/finalprojectWFH/WFHWBPGender_1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link

## Getting Started
In 'WFH data exploration and cleaning' Jupyter NB you can find the 'WFHdata_February24.csv' with it's 611 columns and 236,164 rows. Various columns were explored using the 'Variable dictionary March24.pdf'. Once the relevant columns were chosen, cleaned and improved, dataset were exported for modeling('rem.xlsx') and visualisations('dfBoss.xlsx','dfcommute.xlsx','dfwp.xlsx','dfp.csv','wfhc.csv')

Corrolation and dependecies between participant traits and their WFH/WBP wishlist are analysed in 'WFH WBP.ipynb'. Different prediction classifiers are tested in 'rem data manipulation.ipynb'. TOnca scales and normalized, the first prediction model has the best accuracy results however the data is highly imbalanced. Therefor I proceded with testing various models on up and down samples from the data. 

To corroborate my analysis a web scrabe of Linkedin.com can be found in 'WFH web scraping - eu IT Services.ipynb'. 

## Conclusion
The first model showed that the most impactful traits on the workplace of employees is naturally what the boss allows, the education and income of the participants. Since these are expected influences, I further tested the model without those features 'rem data manipulation-noBoss_noEducation_noIncome_noMonth_noYear_noOther.ipynb'. In that prediction, I was surprised to learn that other than the Industry in which the employee work, lass commute and more family time were the top 3 traits which impacted the model prediction. 

Overall, before the pandemic less than 5% of employees world wide worked completely remotely. Today around 30% of employees work some form of hybrid/remote globally. This was confirmed in basic scraping of linkedin job posts found in 'WFH web scraping - eu IT Services.ipynb'. 

That’s a huge shift in personal priorities, business decisions, and an overall environmental impact. This data analysis project was a glimpse into why and how do the employees chose their working stylr. 

