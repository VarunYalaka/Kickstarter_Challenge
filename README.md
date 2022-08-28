# Kickstarting with Excel

## Overview of Project
This project is to analyze a kickstarter campaign dataset for Louise to help her campaign success. 

### Purpose
Louise wants to begin a crowdfunding campaign for her play “Fever”. However, she has crowdfunding data, wants to understand how to increase the success rate of the campaign. We will analyze how launch dates and funding goals impact the campaign success for “Theater” in the Parent category. 

## Analysis and Challenges
The kickstarter campaign contains more than 4000 rows of data with different categories and subcategories. Which includes useful information like “Goal”, “Pledged” and “Outcomes” based on country and backers_count. 

![Kickstartersheet_data](https://user-images.githubusercontent.com/44387918/187019255-51f92eb8-52de-480a-bc57-6890ae97962e.png) 

However, “Deadline” and “Launched_at” columns contain poorly formatted dates such as 1437620400. Which is a Unix timestamp, further converting them to human readable format like  “MM/DD/YY” in separate columns using excel formula.   
*Example:  =(((xx/60)/60)/24)+DATE(1970,1,1))* 

![Date](https://user-images.githubusercontent.com/44387918/187019498-d4cb47b4-b229-42f4-8fab-fcc26315e02d.png) 
 
Similarly, divided “Category and Subcategory” data to two different columns for better filtering.  

### Analysis of Outcomes Based on Launch Date
Analyzed the success rate of a theater play campaign based on launch date and observed below trend lines in the chart. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/44387918/187019850-8066b9d7-1573-4607-87e8-129d2e8893ea.png) 
 
The success line incrementation starts from April to August and peaks in May. Therefore, the most successful time is “April to May “. 
Based on the above chat, the least successful time for campaigning is December.

### Analysis of Outcomes Based on Goals
Analyzed the success rate of a theater play campaign based on the fundraising goal and observed below trend lines. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/44387918/187020528-cf930e3d-f4a7-4017-85b2-d1a98e8f7225.png) 
 
Higher success rate of a theater play campaign is with lower goals i.e, less than $10000. 
The failure rate shows from $15000 to $30000 goal and greater than $40000. 
Observed increase in success rate between $35000 to $40000 goal, which is unclear and needs to dive deep into the data to understand. 

### Challenges and Difficulties Encountered
* Usage of statistical functions referencing from one to different forms. 
* Exclude unnecessary data on the pivot tables. 
* Changing Unix timestamps to human readable format. 

### Results
1. Based on the analysis, we suggest:  
   - Louise start her campaign between April to May.  
   - Try to avoid starting a campaign between November to January. 
 
2. Louise estimates a budget of over $10,000, which may lead mostly to failure. We suggest to reduce the goal amount to increase the success rate. 

### Limitations
All play themes are not similar, successful ones are more subjective and the right time in the right place. Need to do some   analysis using the blurb.

### Other possible areas or graphs: 
* Further analyze the success ratio based on the duration of the campaign. 
* Explore the funding percentage based on the launch date (i.e Percentage funded vs launch date table). 
