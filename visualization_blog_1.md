# Visualization Blog 1: Controversial Topics

## Part 1: A Visualization I Like

<img src="https://github.com/pazbaum/data_viz_390/blob/main/vb1_pew_mask_viz.png" width = 50% height = 50%>

Source: https://www.pewresearch.org/fact-tank/2022/05/11/57-of-americans-say-masks-should-be-required-on-airplanes-and-public-transportation/

This visualiztion from the Pew Research Center is a clear representation of Americans' opinions as of May 2022 on whether or not masks should be required in indoor, public spaces. One reason why the visualization is transparent is because it provides the question asked to the respondents. Therefore, we know that the results are a true representation of respondents' opinions; their answers were not misconstrued. The visualization is also clear and honest because it provides the date that the survey was conducted. Opinions about Covid protocol, including mask requirements, have changed often and rapidly since the pandemic began, so the timing of a poll about Covid is vital context to the results of that poll. The visualization itself is useful because it separates results into two distinct categories ("masks should be required" and "masks should not be required") and breaks the results down based on demographic information that, according to researchers, impact people's perceptions of and reactions to Covid.

This code produces a similar graphic, as shown below:
```
demographics <- c('U.S. adults', 'Men', 'Women', 'Rep/lean Rep', 'Dem/lean Dem', 'Vaccinated', 'Not vaccinated',
                  'U.S. adults', 'Men', 'Women', 'Rep/lean Rep', 'Dem/lean Dem', 'Vaccinated', 'Not vaccinated')
condition<-c(rep(0,7), rep(1, 7))
value <- c(42, 49, 36, 71, 19, 33, 74,
           57, 51, 63, 29, 80, 66, 25)

df<- data.frame(demographics, condition, value)

df$condition <- as.factor(df$condition)

df %>% 
  ggplot(aes(x= demographics, y = value))+ 
  geom_col(aes(fill= as_factor(condition)), position = "dodge") + 
  geom_text(aes(label = round(value, 2), fill = as_factor(condition)), 
            position = position_dodge(0.9), vjust = -0.6) + 
  ylim (0, 100) + 
  scale_x_discrete(labels = c("Adults", "Men", "Women", 'Rep/lean Rep', 'Dem/lean Dem', 'Vaccinated', 'Not vaccinated'))+
  scale_fill_discrete(name = 'Belief in Requirement', 
                      labels = c('Should Not Be Required', "Should Be Required")) +
  labs(x = "Demographic Category", 
       y = "Percentage",
       title = 'Percentage of Americans who believe masks should be required on airports and public transportation')
```
<img src = 'https://github.com/pazbaum/data_viz_390/blob/main/vb1_recreation.png' width = 70% height = 70%>

## Part 2: A Visualization I Dislike

<img src="https://github.com/pazbaum/data_viz_390/blob/main/2020_electoral_map.png" width = 50% height = 50%>

Source: https://brilliantmaps.com/2020-county-election-map/

This is a visualization of the 2020 presidential election results. While election results may not seem like a contentious topic, the 2020 presidential results certainly were. The map displayed above portrays election results by county, which is accurate, but it gives the false impression that the Republican candidate won more votes than the Democratic candidate. This is because the map is colored by county election results instead of population election results. A more accurate way to display the 2020 presidential election results would be to create a map with states artificially larger or smaller based on their population. This way, the map would communicate that more people voted for the Democratic candidate than the Republican candidate, leading a Democratic victory.

## Part 3: My Own Visualization
