# Kickstarter Analysis
This analysis was performed by analyzing on provided dataset to undercover trends.
A Louise's play _Fever_ came close to its fundraising goal in a short amount of time, now she wants to know how different campaigns fared in relation to their launch dates and their funding goals. So, using the provided dataset, this time we will analyze how the outcome will be based on the launch dates and the funding goals.

# Analysis and Challenges
There are two parts of the analyses, and below are how I encountered the problems.
## Theater Outcomes by Launch Date
Step 1: Created a pivot table based on the given Kickstarter dataset.

![Screen Shot 2022-06-26 at 4 45 11 PM](https://user-images.githubusercontent.com/107448172/175838526-7bbd9533-ea71-46e4-9c4b-8f4257766373.png)

Step 2: Filtered the dataset into Parent Category, Years, with three different outcomes: successful, failed and canceled.

![Screen Shot 2022-06-26 at 4 46 55 PM](https://user-images.githubusercontent.com/107448172/175838576-a9dc6236-de88-4299-9cb4-ca3b4f91abd9.png)

Step 3: Created a line chart on the pivot table to visualize the relationship between outcomes and launch month. 

![Screen Shot 2022-06-26 at 4 45 57 PM](https://user-images.githubusercontent.com/107448172/175838557-29cfa064-cdcc-4e88-9d1b-bd770db8c75d.png)

## Outcomes based on Goals
Step 1: Gathered data from the Kickstarter dataset by using =COUNTIFS() based on certain dataset including 'Goal', 'Outcomes', and 'Plays'. 

![Screen Shot 2022-06-26 at 4 52 53 PM](https://user-images.githubusercontent.com/107448172/175838781-36fd4a5f-af8e-4e95-a89b-bf57dde9c917.png)

Step 2: Made sure the data was counted has to be correct according to different number of goals.

![Screen Shot 2022-06-26 at 4 55 18 PM](https://user-images.githubusercontent.com/107448172/175838882-281f79e3-c3e4-460a-a532-f715f75bc1e4.png)

Step 3: Calculated the percentage of successful projects and failed projects based on total counts of all projects. 

![Screen Shot 2022-06-26 at 5 00 03 PM](https://user-images.githubusercontent.com/107448172/175839084-c7893875-3614-4fcd-83e2-6127b1a71b2e.png)

Step 4: Created a line chart to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-basis.
![Screen Shot 2022-06-26 at 5 48 52 PM](https://user-images.githubusercontent.com/107448172/175841287-af164408-17e6-4b29-b0ff-8f4058c00dd6.png)

### Difficulties along the way
At first when I used =COUNTIFS() function, I wasn't getting the right number using the auto-generate option. I had to go back and manually entered the function and triple-checked the functions to get it right. There were different outcomes if the function wasn't clarified correctly. For example, the count number will be different if the funtion contains '=' or without '='.
Then, the line chart I created wasn't reflected the number that I had. But then I re-created the chart by selecting a different type of chart and then problem solved. 

![Screen Shot 2022-06-24 at 4 52 00 PM (1)](https://user-images.githubusercontent.com/107448172/175842949-95790525-6231-4cb3-97a3-798743370a45.png)

# Outcomes
Two conclusions are made about Theater Outcomes by Launch date:
- The number of successful projects is almost double the number of failed projects.
- The most successful time of the year are from March to May, and the from May to September, the number started to falling. 

One conclusion is made about the Outcomes based on Goals:
The percentage of successful line and the percentage of failed line are perfectly flipped on the chart, and the lower the goal, the higher the number of successful projects.

Limitations of dataset:
This dataset is too small to make a conclusion between the relationship between the outcomes based on the launch date. Personally, I can only tell the result according to the numbers, but I can't explain why. For example, why during March to May the number is higher but not after that, what happened that made the number changes. 

Same thing with the Outcomes based on Goals analysis, I believe this data is collected around the world. So, I can't concluded that the result in the analysis is related since different countries will resulted in different numbers and patterns. 
         
Recommendations:
With the Theater outcome based on launch date analysis, I recommend additional pivot table can be create with countries filter on. Or, we can only focus on US, or UK for our analysis only. 

With the Outcomes based on goals, I would recommend adding in goal pledged dataset, so we can see the gap between pledged goal and actual goal, and the affect it has on number of successful projects, failed projects and canceled projects. 


       

