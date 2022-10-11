# Visualization Blog 1: Controversial Topics
**Part 1: A Good Visualization**

<img src="https://github.com/pazbaum/data_viz_390/blob/main/vb1_pew_mask_viz.png" width = 40% height = 40%>

This visualiztion from the Pew Research Center is a clear representation of Americans' opinions as of May 2022 on whether or not masks should be required in indoor, public areas. It 

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
<img src = 'https://github.com/pazbaum/data_viz_390/blob/main/vd1_recreation.png' width = 60% height = 60%>
