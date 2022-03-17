# Bike-share-nevigate-speedy-success
The Cyclistic bike share analysis is a project based on a fictional company in Chicago. As an analyst, the goal of this project is to maximize the number of annual memberships which would lead to the growth of the company. In order to achieve this, the team wants to design a new marketing strategy to convert casual riders into annual members. The company launched in 2016 and has since then grown a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.

GOAL **Converting casual riders into annual members of the bike-share product.** In order to tackle this, these key steps would be followed:

a. Ask
b. Prepare
c. Process
d. Analyse
e. Share
f. Act

**ASK**

Business task: Growth of the company by increasing the number of members through converting casual riders to annual members. Exploring how casual users use Cyclistic bikes differently from annual members. Key Stakeholders: The Director of Marketing, The Manager, Marketing Analytics Team and the Executive Team.

**PREPARE**

The data being used is the Divvy datasets which has been made available by Motivate International Inc. under the license. Cyclisitc is a fictional company hence using this public data to explore the different types of riders and their behaviours. Riders’ personally identifiable information has been removed from the data due to data privacy policies. Viewing the data in spreadsheet for the first quick glance, it is seen that the datasets have 13 features namely; ride_id, rideable_type, started_at, ended_at, start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng and member_casual.


**PROCESS**

The data of previous 11 months has been used and using Power query editor in excel they all are merged onto one worksheet.
The data has been cleaned in power query, all the error were removed from started_at, ended_at, start_station_name, end_station_name. 
created a column called “ride_length.” Calculated the length of each ride by subtracting the
column “started_at” from the column “ended_at” (for example, =D2-C2) and format as HH:MM:SS using Format > Cells >
Time > 37:30:55. and then converted it in hours.
Created a column called “day_of_week,” and calculated the day of the week that each ride started using the “WEEKDAY”
command (for example, =WEEKDAY(C2,1)) in each file. Format as General or as a number with no decimals, noting that
0 = Monday and 6 = Sunday.


**ANALYZE**

 Ran a few calculations in one file to get a better sense of the data layout. Options:
● Calculated the mean of ride_length
● Calculated the max ride_length
● Calculated the mode of day_of_week
 Created a pivot table to quickly calculate and visualize the data. Options:
● Calculated the average ride_length for members and casual riders. Try rows = member_casual; Values = Average
of ride_length.
● Calculated the average ride_length for users by day_of_week. Try columns = day_of_week; Rows =
member_casual; Values = Average of ride_length.
● Calculated the number of rides for users by day_of_week by adding Count of trip_id to Values.

**SHARE**

What did data tell us **Total rides per month** 

![image](https://user-images.githubusercontent.com/28131288/158747456-4a2eef33-6df1-494f-bc73-950fe23356e6.png)

The rides per month show that casual riders were a lot more active during the summer months than the long-term. Conversly, the winter months show very little activity on the part of the casual users. The long-term users are more active in the winter and spring months.

**Rides as per Week**

![image](https://user-images.githubusercontent.com/28131288/158749927-59120913-dbe4-40d5-a74e-653a2851e602.png)

The rides per day of week show casual riders peak on the Saturday and Sunday while members peak Monday through Friday. This indicates members mainly use the bikes for their commutes and not leisure.

**Average ride time per week**

![image](https://user-images.githubusercontent.com/28131288/158751551-257785fd-f12e-4908-b898-937b5a9a619f.png)

The average ride time shows a stark difference between the casuals and members. Casuals overall spend more time using the service than their full time member counter-parts.

**Which bike is popular**

![image](https://user-images.githubusercontent.com/28131288/158751975-dbac5955-6577-4da3-9ca2-d96767451aae.png)

The breakdown of which type of bike is the most popular among either type of user. Showing among the two types of bikes classic and electric. both types of memberships prefer using the classic bike more so than the electric bike. The long-term memebrs are also seen to be of the two types favours the classic bike.

WHAT DOES DATA TELL US?

**key takeaways**


● Casual users tended to ride more so in the warmer months of Chicago, namely June- August. Their participation exceeded that of the long term members.

● To further that the Casual demographic spent on average a lot longer time per ride than their long-term counter-parts.

● The days of the week also further shows that causal riders prefer to use the service during the weekends as their usage peaked then. The long term members conversly utilised the service more-so throughout the typical work week i.e (Monday- friday)

● Long term riders tended to stick more so to classic bikes as opposed to the docked or electric bikes.

**RECOMMENDATIONS**

● Introducing plans thats may be more appealing to casuals for the summer months. This marketing should be done during the winter months in preperation.

● The casual users might be more interested in a memebrship option that allows for per-use balance card. Alternatively, the existing payment structure may be altered in order to make single-use more costly to the casual riders as well as lowering the long-term membership rate.

● Membership rates specifically for the warmer months as well as for those who only ride on the weekends would assist in targeting the casual riders more specifically




