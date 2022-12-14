# Short Form Blog 1: What drives college students to vote?

### Why study student voters?

Voting systems in America are designed for urban and suburban adults with a flexible job and permanent address. Unlike adults, college students have strict class and work schedules and days filled with sports practices and club meetings. They often live in a state different from where they grew up and rarely live at the same address for longer than a year or two. The odds of voting are stacked against them.

Why, then, do some students vote? Which students vote, and in what elections? How do students vote and who enables them to do so? These questions coupled with my work with NU Votes, an organization at Northwestern that enables students to register to vote and request absentee ballots, motivated me to look into student voter habits.

College students are allowed to register to vote in either their home state or the state in which they attend school but are granted no federal rights beyond that. Absentee voting, voter ID, and registration/ballot request deadline laws vary by state. Thirty-one states require absentee ballot requests to be printed out and mailed.[<sup>1</sup>](https://www.ncsl.org/research/elections-and-campaigns/vopp-table-6-states-with-web-based-and-online-absentee-ballot-applications.aspx) Fourteen states require voters’ mail-in ballots to be witnessed or notarized.[<sup>2</sup>](https://www.ncsl.org/research/elections-and-campaigns/vopp-table-14-how-states-verify-voted-absentee.aspx) In Illinois, in order to register to vote in person, residents must show a physical document that proves their address.

College students have limited access to printers and mailing supplies, their addresses are temporary so they receive little mail, and it is unlikely that most students know a notary. The scarcity of time and money among college students makes it difficult for them to complete the required steps to participate in our democracy at the most basic level.

Despite these obstacles, more young people are turning out to vote each election. In 2020, 55% of people ages 18 to 29 voted. This is an 11% increase from 2016 and a 15% increase from 2000.[<sup>3</sup>](https://www.statista.com/statistics/984745/youth-voter-turnout-presidential-elections-us/) Young people are the future; they are already leading social movements and participating in the political process in historic ways.[<sup>4</sup>](https://www.commonsensemedia.org/articles/6-youth-led-political-movements-to-inspire-you-to-vote) It is therefore vital that we study how and why this participation came to be as well as where it will go from here.

### Data Source: ANES

In order to investigate student voter trends, I used data from the American National Election Studies (ANES) 2016 and 2020 surveys. ANES has conducted public opinion and electoral behavior interviews before and after each presidential election since 1948.[<sup>5</sup>](https://electionstudies.org/about-us/history/)

In 2016, interviews were conducted both in-person and online, and in 2020 they were exclusively online. Respondents were randomly selected from residential addresses in the U.S. The sample was selected based on counties that were stratified by region, prevalence of poverty and members of minority groups, and population size. ANES conducted about 4,000 interviews before and after each election.[<sup>6</sup>](https://electionstudies.org/wp-content/uploads/2018/12/anes_timeseries_2016_userguidecodebook.pdf)<sup>,</sup>[<sup>7</sup>](https://electionstudies.org/wp-content/uploads/2022/02/anes_timeseries_2020_userguidecodebook_20220210.pdf)

ANES survey data is trustworthy because in its collection, researchers took into account the heterogeneity of the target population–the U.S. public. For example, respondents are stratified by variables including race, gender, and region. The data is also trustworthy because the sample size is thousands of people, which is a large portion of the target population.

The main limitation of the ANES data is that it was not collected with students in mind. As a result, there is a relatively small sample size of college students–121 students over the two surveys. Because of this, the analysis conducted cannot be generalized to the entire population of students in the U.S. Another resulting limitation is that the survey questions are not targeted toward students. For example, respondents were not asked whether they voted in the state from which they are from or the state in which they attend school, which is an important aspect of student voter habits. Despite these limitations, ANES is a good data source for this analysis because the data itself is reliable.

### Student Voter Habits

The dataset used in the following visualizations includes the data of respondents to the ANES surveys in 2016 and 2020 who indicated their work status as “student” and were between the ages of 18 and 22 at the time of the survey.

Voting laws vary greatly by state, but there are some regional consistencies. Northern states tend to have more lenient voting laws while Southern states tend to have stricter voting laws.[<sup>8</sup>](https://www.usnews.com/news/the-report/articles/2021-04-09/how-voting-laws-suppress-the-new-south) As shown in the plot below, a lower percentage of students voted in the South than in the Northeast, Midwest, and Western regions of the U.S. in the 2016 and 2020 elections. Specifically, 25% fewer students voted in the South compared to the Northeast and Midwest. More research is required in order to find out the reasons behind this discrepancy. While there are several potential factors, such as culture and candidate outreach to students, one likely variable is accessibility of voting.

One limitation of the plot below is that it does not specify if students are voting in their home or their school state or if they are voting in-person or absentee. It is therefore difficult to ascertain the impact of specific states’ voting laws on student voter habits and accessibility.

![A bar graph titled "% of Student Voters by Region" with four categories--"Midwest", "Northeast", "South", and "West"--on the x-axis and "% of Students Who Voted" on the y-axis. The plot shows that 78% of students in the Midwest voted, 79% in the Northeast, 53% in the South, and 69% in the West.](https://github.com/pazbaum/data_viz_390/blob/main/sb1_voters_by_region.png)

Voting remains inaccessible to many people throughout young adulthood, but it becomes more accessible as a person ages. Older people tend to have more money and access to transportation compared to younger people, which makes getting to the polls as well as travelling to pick up mailing supplies easier. This trend holds true even within small age ranges, like 18 to 22 year olds in college. For example, many universities allow upperclassmen to have cars on campus but not underclassmen.

This is reflected in the data, as demonstrated below. Voters are concentrated at an older age, 20, while non-voters are concentrated at a younger age, 19. Another indicator that civic participation increases with age is that the population of students who were registered but did not vote is older than the population that was not registered at all.

When broken down by election year, the data show that while in 2016, more older college students voted than younger college students, in 2020, voting was spread fairly evenly across students ages 18 to 21. This brings into question the differences between the 2016 and 2020 elections. The two main factors are the pandemic, which caused college students across the country to move home for a year, and Trump’s presidency. The pandemic likely improved accessibility to voting: states expanded their vote-by-mail systems; many students were with their middle aged parents, who were of a demographic likely to vote, at the time of the election; and many students were in the familiar political environment of their home state.

A limitation of these boxplots is that they show the number, not percentage, of students of each age. It is therefore slightly skewed toward students ages 19 to 21 since those are the most common ages of college students.

![Two boxplots side-by-side with "Age" on the x-axis and three categories on the y-axis: "Voted", "Registered but did not vote", and "Not registered". The boxplot on the left, titled "Student Voting Status by Age", shows that the mean age of students "Not registered" and "Registered but did not vote" is 19 and the mean age of students who voted is 20. The boxplot on the right, titled "Student Voting Status by Age and Year" breaks down each y-axis category into the 2016 and 2020 elections. In 2020, the interquartile range of ages of students who voted is larger than it was in 2016.](https://github.com/pazbaum/data_viz_390/blob/main/sb1_voted_age_boxplots.png)

With the plots below, we can take a closer look at exactly how many students voted in 2016 compared to 2020. Over 20% more college students voted in the latter election, and there was a larger increase in female student voter turnout than male student voter turnout. More research is needed in order to determine what caused the higher college student turnout in 2020 compared to 2016. It is possible, though, that a combination of college students being in their home states during the 2020 election and the public’s strong feelings toward Trump led to this increase in turnout.

The gender difference in turnout is important because it indicates that there may be different motivating factors for male and female students to vote. It is unclear why turnout increased more for female students than male students from 2016 to 2020, but one possibility is that female students had a stronger oppositional reaction to Trump’s presidency compared to their male counterparts.

![Two bar graphs side-by-side with "Year" on the x-axis with the categories "2016" and "2020" and "% of Students Who Voted" on the y-axis. The plot on the left, titled "Student Voters in the 2016 and 2020 Elections: Total" shows that in 2016, 56% of students voted and in 2020, 77% of students voted. The plot on the right, titled "Student Voters in the 2016 and 2020 Elections: By Gender" breaks the data of each year into two gender categories, "Male" and "Female". It shows that among female students, 59% voted in 2016 and 83% voted in 2020 and among male students, 55% voted in 2016 and 71% voted in 2020.](https://github.com/pazbaum/data_viz_390/blob/main/sb1_voted_by_year.png)

The high turnout from college students in 2020 led to victory for the Democrats. As shown below, 90% of student voters voted for Biden in 2020, an increase of 14% from the votes democratic nominee Hillary Clinton got from college students in 2016. This is one reason why I believe it is possible that Trump, who ran in both elections, was a motivating force behind the increase in student turnout.

Another possible explanation for the high percentage of democratic student voters is that Trump-supporting students were prevented from voting. Southern states tend to have both more conservative residents and stricter voting laws. As was seen in the first plot of this blog, a relatively low percentage of students voted in the South, which could be a result of laws in Southern states that make it difficult for students to vote. It is therefore possible that Trump-supporting students were underrepresented in the results of the 2020 election.

Beyond the small sample size of students this plot is based on, another limitation is that it does not account for third party voters. The few third party student voters in this sample were removed from the data used to create the plot for ease of calculations.

![A bar plot titled "Students Who Voted for the Democratic Presidential Candidate" with two categories--"2016: Hillary Clinton" and "2020: Joe Biden"--on the x-axis and "% of Students" on the y-axis. The plot shows that in 2016, 76% of students voted for the Democratic presidential candidate and in 2020, 90% of students voted for the Democratic presidential candidate.](https://github.com/pazbaum/data_viz_390/blob/main/sb1_dem_vote.png)

The data and visualizations above demonstrate that students in the Northeast and Midwest, older students, female students, and democratic students tend to vote at higher rates than their counterparts. If I could collect more data on the topic, I would conduct a regression analysis to determine which variables have the greatest impact on student voter registration and turnout rates.

Given the opportunity, I would also look into how students vote–absentee ballot or in-person, in their home state or their school state, and registered on their own or through an organization. Access to this data would enable voter advocacy groups to tailor their programming to students’ habits and desires.

### Bibliography

American National Election Studies. *ANES History.* https://electionstudies.org/about-us/history/ 

American National Election Studies. (2022). *ANES Time Series Cumulative Data File.* September 16, 2022 version. www.electionstudies.org

American National Election Studies. (2019, Sept. 4). *User’s Guide and Codebook for the ANES 2016 Time Series Study.* https://electionstudies.org/wp-content/uploads/2018/12/anes_timeseries_2016_userguidecodebook.pdf 

American National Election Studies. (2022, Feb. 10). *User’s Guide and Codebook for the ANES 2020 Time Series Study.* https://electionstudies.org/wp-content/uploads/2022/02/anes_timeseries_2020_userguidecodebook_20220210.pdf 

Arnold J (2021). _ggthemes: Extra
  Themes, Scales and Geoms for 'ggplot2'_.
  R package version 4.2.4,
  <https://CRAN.R-project.org/package=ggthemes>.

Hagen, F., & Milligan, S. (2021, April 9). *How Voting Laws Suppress the ‘New South’.* U.S. News and World Report. https://www.usnews.com/news/the-report/articles/2021-04-09/how-voting-laws-suppress-the-new-south 

Hvitfeldt E. (2021). paletteer:
  Comprehensive Collection of Color
  Palettes. version 1.3.0.
  https://github.com/EmilHvitfeldt/paletteer

National Conference of State Legislatures. (2022, July 12). *Table 6: States With Online Absentee Ballot Application Portals.* https://www.ncsl.org/research/elections-and-campaigns/vopp-table-6-states-with-web-based-and-online-absentee-ballot-applications.aspx 

National Conference of State Legislatures. (2022, March 15). *Table 14: How States Verify Voted Absentee/Mail Ballots.* https://www.ncsl.org/research/elections-and-campaigns/vopp-table-14-how-states-verify-voted-absentee.aspx 

Pedersen T (2022). _patchwork: The
  Composer of Plots_. R package version
  1.1.2,
  <https://CRAN.R-project.org/package=patchwork>.

Rossell Hayes, Alexander (2022).
  fauxnaif: Convert Values to NA.
  https://fauxnaif.rossellhayes.com

Statista Research Department. (2022, Sept. 30). *Youth voter turnout in presidential elections in the United States from 1972 to 2020.* https://www.statista.com/statistics/984745/youth-voter-turnout-presidential-elections-us/ 

Trageser, C. (2020, April 1). *6 Youth-Led Political Movements to Inspire You to Vote.* Common Sense Media. https://www.commonsensemedia.org/articles/6-youth-led-political-movements-to-inspire-you-to-vote 

Wickham H, Averick M, Bryan J, Chang W, McGowan LD, François R,
  Grolemund G, Hayes A, Henry L, Hester J, Kuhn M, Pedersen TL, Miller E,
  Bache SM, Müller K, Ooms J, Robinson D, Seidel DP, Spinu V, Takahashi K,
  Vaughan D, Wilke C, Woo K, Yutani H (2019). “Welcome to the tidyverse.”
  _Journal of Open Source Software_, *4*(43), 1686.
  doi:10.21105/joss.01686 <https://doi.org/10.21105/joss.01686>.

Wickham H, François R, Henry L, Müller K
  (2022). _dplyr: A Grammar of Data
  Manipulation_. R package version 1.0.10,
  <https://CRAN.R-project.org/package=dplyr>.

Wickham H, Miller E, Smith D (2022).
  _haven: Import and Export 'SPSS',
  'Stata' and 'SAS' Files_. R package
  version 2.5.1,
  <https://CRAN.R-project.org/package=haven>.

Wickham H, Seidel D (2022). _scales:
  Scale Functions for Visualization_. R
  package version 1.2.1,
  <https://CRAN.R-project.org/package=scales>.
