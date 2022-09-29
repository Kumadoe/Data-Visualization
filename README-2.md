# (Ford GoBike System Data Exploration)
## by (Sheriff Francis Doe Kumadoe)


## Dataset

 This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The dataset contains 183412 observations and 16 attributes. After wrangling, Most of the remaining variables were categorical(nominal) in nature with a few being objects and strings. The only ordinal data type is member birth year. 
I wrangled the dataset by first converting variables to their required datatypes like to datetime or categorical using .astype(), i extracted new desired columns from already existing columns. In dealing with missing values for the categorical variables, i used the .fillna() to fill in the mode of that particular variable. Finally i dropped some columns that i wouldnt need in the exploration process.
The dataset can be found by clicking the link: https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1660457351989930&usg=AOvVaw1C7cGwDWmHAt8beo0ODp-z


## Summary of Findings

In the exploration, I found that there were more male users compared to female and other 
users. Also there were more subscribers than the customers. More users were eligible
for the Bike share for all trips than those whho weren't. For the time and day that 
most trips started and ended, i found that majority of the trips begun on weekdays 
and the least on weekends with Thurdays being the day of the week when most trips started and 
ended. Also majority of the trips begun during mornings and evenings followed by afternoons
with the least trips taking place at dawns. I also found that subscribers were more than 
customers across all three member geder types which may be due to the majority of users
being subscribers. To know the exact times of which days most trips begun, i found that
the mornings of fridays, thursdays, and tuesdays as well as thursday evenings had the highest 
count of users. It was interesting to finnd out that the categories with majority users
like males and subscribers turned out to have lower mean distance covered compared with
their respective minority groups like Other and customers. It wasnt surprising to find 
out that the Other gender types who were customers had the highest mean distance 
covered and male subscribers had the least mean distance covered in seconds.
Similarly, the Dawn of sundays which happens to be the time with the least number
of users happen to have the highest mean distance traveled. Also Not only does the 
Other gender type have the highest overall mean distance covered but it also has the 
highest distance covered in all the respective start days. This is followed by females 
and finally males. It is only in one case where the mean distance travelled by males 
exceeded that of females and that was on saturdays.




## Key Insights for Presentation

For the presentation, I'm interested in the gender that patronized the Bike Share system the most
and if it depends on whether they were subscribers or customers. When the most trips were taken in terms of time 
and the day. How long the average trip takes(duration_sec) for each time and day. 

I will first plot a bar graph showing the counts of each gender type. Will follow with another bar graph 
showing the relationship between member gender and user type. This should show how the user types 
behave across all the member genders. 
I will finally find the counts of the start day and start time. After i will wrap up by finding how they 
relate with the duration_sec which is the distance covered in seconds.
