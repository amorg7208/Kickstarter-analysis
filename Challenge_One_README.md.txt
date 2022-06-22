# Kickstarting with Excel## Overview of Project
  Analyze data to determine outcomes based on monetary goals vs. launch dates for Theater and Play events.
### Purpose
The purpose of this project is to visualize data and draw conclusions as appropriate based on those findings. Specifically, we are looking at theater outcomes based on launch date and play outcomes based on funding goals. Comparing the data outcomes will allow our client to make more savvy decisions when it comes to starting a new Kickstarter campaign. ## Analysis and Challenges
There are two deliverables created in this analysis: Theater Outcomes Based on Launch Date and Outcomes Based on Goals.
To analyze the outcomes based on Launch Date, a new column was created in the spreadsheet titled, "Years" and used the Year() function to extract the date from the "Date Created Conversion" column. A pivot table was created based off of the launch date and different outcome variables: "Successful," "Failed," and "Canceled." The table was filtered via "Parent Category" and "Years" and the columns were filtered by outcomes. The "Parent Category" was set to show only "Theater" data. Finally the table was sorted in descending order. A line chart was created from the pivot table.

![Theater Outcomes Based on Launch Date](Data_Class/resources/Theater_Outcomes_Based_On_Launch-Date.png)

To analyze the outcomes based on funding goals a new sheet was created with a range of funding goals listed in ascending order by 5000. The =COUNTIFS function was then used to populate data into new columns: "Number Successful," "Number Failed," and "Number Canceled" by filtering the Kickstarter sheet column "outcome." Additional qualifiers were used including the new "goal" column ranges and "subcategory" column in the Kickstarter sheet filtered to "plays." The sum function was used to populate total projects for each funding range. Then percentages were calculated of successful, failed and cancelled projects for each row. A line chart was created showcasing the relationship between funding goal ranges and the percentage of the various outcomes. 
![Outcomes Based on Goal](Data_Class/resources/Outcomes_Based_On_Goal.png)
### Analysis of Outcomes Based on Launch Date
-May is the best time to launch a theater Kickstarter as it has the highest success rate. 
-November has the most failed campaigns. 
-It is likely that this trend is due to school finishing in the late spring and resuming in the fall. ### Analysis of Outcomes Based on Goals
Generally, the higher the funding goal amount, the more likely the campaign is to fail. 
Plays that aim to generate a funding goal of 5,000 or less have a higher success rate than any higher amounts. 
The amount of plays funded at this lower funding goal is greater than the amount of plays at higher funding goals. This would be the safer choice in launching a new campaign. 
The highest ranging goal amounts had a 87.5-100% fail rate.
There are significantly less amounts of plays at this higher goal range, making it riskier to launch a large scale event.  ### Challenges and Difficulties EncounteredI followed the directions laid out in Bootcamp Spot but when I didn’t understand how to do something I googled, used YouTube and the “hints” videos in Bootcamp Spot. I also reached out on Slack to some classmates, as well as, in my direct thread with the TA’s and instructor. (Though, I didn’t get any feedback there.) I was able to figure out what I was not doing correctly in my =COUNTIFS function. I was leaving out the “=” part of >=/<= which was leaving out data points. Initially I created the graph, and it did not look right. I knew I had made some sort of mistake because most of my data points were zero. After a lot of trial and error in trying to edit the graph directly I figured out what I was missing. I also had to figure out how to sort the data points correctly. I have also had a challenging time in formatting the ReadMe file for this write up. 
## Results- What are two conclusions you can draw about the Outcomes based on Launch Date?
May is the best time to launch a theater Kickstarter as it has the highest success rate. 
November has the most failed campaigns. 
It is likely that this trend is due to school finishing in the late spring and resuming in the fall. - What can you conclude about the Outcomes based on Goals?
Generally, the higher the funding goal amount, the more likely the campaign is to fail. It would be safer to create a small to modest campaign with a smaller funding goal as it is more likely to be successful. - What are some limitations of this dataset?
Changing the goal increments from 5000 to smaller size could change graph interpretation. This seems to be more of an overview of success/failed rather than specific, individual data points. There could also be biases of data since we do not know how this data was collected. - What are some other possible tables and/or graphs that we could create?
The data used in this analysis was global, we did not filter for specific location. We could create tables and graphs depicting only US data, or only country data for wherever the next campaign will be. 