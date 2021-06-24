# Kickstarting with Excel

## Overview of Project & Purpose
Perform analysis on Kickstarter Campaigns for Louise; Analyze data and uncover trends to help her with her future success

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Using the function: Year(), the corresponding years of the Date Created Conversion Columns were extracted and placed in a separate new column. 

![Year Function](https://user-images.githubusercontent.com/84931545/123334379-02056380-d511-11eb-9d9d-5b608a5d5dfb.PNG)

The entire Kickstarter worksheet was then selected to be encoded on a new PivotTable. Years and Outcomes were placed in Rows and Columns of the PivotTable. Additional filters including Years and Parent Category were added with the Parent category filtered to 'theater' category. Outcomes Columns were sorted in descending order in order to show successful outcomes first.

![PivotTable Filters](https://user-images.githubusercontent.com/84931545/123334436-1d706e80-d511-11eb-82c9-afff458c971c.PNG)

A line chart with markers was created with Months in the x-axis and the number of outcomes in the y-axis based on the PivotTable.

![Theater_Outcomes _vs_Launch](https://user-images.githubusercontent.com/84931545/123334475-2cefb780-d511-11eb-8faf-bfb70d48835f.png)

### Analysis of Outcomes Based on Goals
8 columns and 12 rows were created on a worksheet with their corresponding titles and goal-amount ranges 

COUNTIFS() functions were used to filter the desired outcome, goal-amount ranges, and "plays" subcategory from the Kickstarter worksheet and populate the corresponding Number Successful, Number Failed, and Number Canceled columns.

Total Projects is calculated using the SUM() function to add the number of successful, failed, and canceled projects for each row.

![Sum](https://user-images.githubusercontent.com/84931545/123334556-4690ff00-d511-11eb-8d3b-a8db65ddd699.PNG)

The ROUND() function was used to populate the Percentage Successful, Percentage Failed, and Percentage Canceled columns. The number for the corresponding outcome was divided by the number of total projects and then times by 100 to get the percentage. The percentage value was rounded to the nearest integer.

![Percentage](https://user-images.githubusercontent.com/84931545/123334585-4db80d00-d511-11eb-94a1-f5910d61b921.PNG)

A line chart with markers was plotted with goal-amount ranges in the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/84931545/123334603-53155780-d511-11eb-94a0-f291aa6ef053.png)

### Challenges and Difficulties Encountered
For the Analysis of Outcomes Based on Goals, double-check whether the criteria range and criteria are inputted correctly. 

For the Analysis of Outcomes Based on Launch Date, adding the Date Created Conversion to the Rows will create unwanted Years and Quarters on the PivotTable. Remove them as needed.

![adding Date Created Conversion](https://user-images.githubusercontent.com/84931545/123334820-a4254b80-d511-11eb-9963-962876b624f0.PNG)


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Summer months (May, June, July) have more successful outcomes than Winter Month (November, December, January) for theater.

The numbers of failed outcomes are quite stable around 40 with no significant increase or decrease for theater throughout the year.

- What can you conclude about the Outcomes based on Goals?

There are no Canceled Projects for Plays.

The most successful goal-amount ranges is less than 1000.

- What are some limitations of this dataset?

The increments of goal ranges might be too big to uncover other hiden trends.

There are outliers in the dataset.

- What are some other possible tables and/or graphs that we could create?

Outcomes based on pledged

Outcomes based on Country

Outcomes based on Closing date








