# Making an effective data visualization
**Titanic Passenger data**

**Wesley Scoggin January 2018**

### Summary:
The Titanic dataset includes a sample of 891 passenger details. While this may not be an entire accounting of each passenger aboard when the Titanic sank in 1912, it should provide an interesting look at factors that may have contributed to a passenger's chance of survival in the tragedy.

### Design:
To guide a viewer through factors contributing to survival chances of a passenger, this chart starts at the simplest breakdown of survivors and the deceased in total depicting overall chances were grim. All of the charts in each the initial design are 100% stacked bar charts exploring the ratio of survivors to deceased. A comparison of the breakdown follows the initial state of the chart by splitting passengers into groups by class, then a third chart showing ratios by gender. Finally the last animation transforms the data into A hierarchical group of passenger class and gender. The user can follow the decreasing chances of survival from first class to third, while observing female passengers faired better in each class as compared to the male counterparts.

After the startup animation is complete, users are presented with controls that allow them to explore each of the categorical breakdowns at their leisure with the use of buttons on the left side of the visualization.

### Feedback:
Users were asked to think about the following questions and respond with feedback:

· What do you notice in the visualization?

· What questions do you have about the data?

· What relationships do you notice?

· What do you think is the main takeaway from this visualization?

· Is there something you don’t understand in the graphic?

**Martha:**

This is really cool, I like the visualizations. I can make assumptions about the data just because I saw the movie.

**1.** I noticed that the visualizations all load in order when it is opened and then stays on the last graph. And they had pop-up labels

**2.** I think I would have liked to also know how many people where in each class and gender. It could be that more women survived % wise but I don’t know out of how many women compared to how many men.

**3.** Colors and class categories are consistent making it easier to process.

**4.** Main takeaway is that more women survived % wise in each class and overall

**5.** Why is class 3 first before class 1 & 2? Is it the same as first class, coach, etc.?

**Other feedback:**
a. The last visualization the class and gender it doesn’t specify which column is the gender.

b. The true/false can be misleading. It doesn’t tell you what is true.. that they died or they survived.

c. I am assuming that this is part of larger report but it doesn’t actually say that it is about the Titanic ship that sank in 1912.

d. I think it would tell a different story if it was a stacked bars that way it is  % of the whole so you wouldn’t need as many visualizations and you wouldn’t need to know how many people there were in each category.

**Marc:**
I noticed the initial load of the page cycled through all the categories (All, Class, Gender, Class and Gender), then ending with the category buttons on the left...an automatic drill down effect.

Do you have passenger lists to go with this data?  What is the source?

Females of all classes had a disproportionately higher survival rate than males in all classes; all female classes had above 50%.  Even the highest male survival rate, 1st class males, was less than 40% while the lowest class females had a survival rate of 50%.  It is interesting that the male 2nd and 3rd classes had similar survival rates, while the 1st and 2nd class females had similar survival rates.  

One had a much better chance of surviving the RMS Titanic sinking if one was a 1st or 2nd class female.  "Woman and children first"...

Green is the percentage of people that survived? and males on left and females on right? (Found it on the "tooltip"/"mouseover" popup)  
What was the total number of people?

**Benny**

**1** Initial reaction: The slides moved too quickly from 1 to 4. Had to refresh it a few times for me to review the first 3 slides. Didn’t figure out how to view each slide until I selected
“Select Category” last slide…I blame it on ”user error”. Overall visualization is simple and clear to understand.

**2** None, except for “Are these factual data?”

**3**
  · More female survivors.

  · More survivors for Class 1.

  · Over 90% females survived for Class 1 and 2

  · Hard to believe that over 60% of the passengers died due to lack of Safety and Survival Protocols.

**4** Better to be a female and stay in Class 1 in “Cruise Ships” to increase “Survival Rate”!

**5** No, overall visualization is simple and clear to understand.


### Changes to Final Visualization:
Some of the users that contributed feedback seemed to indicate their wish to see counts as well as 100% stacked bar charts so they could grasp the scale in the difference between each of the categorical breakdowns between gender and class. To accomplish this, additional controls were added at the end of the animation to facilitate changing the y axis type from a percent based axis to a measure axis. Calculated columns were made clearer for survival or deceased status. Rather than "Survived T/F:" indicating True or False, the popup now displays 'Status: Survived' or 'Status: Deceased'. A class string column was concatenating 'Class' with the class integer included in the dataset, it has been changed to read '1st Class', '2nd Class', or '3rd Class'.

Additionally, they expressed that meanings of each bar chart were a bit enigmatic. Although they did find the information they were looking for when they found popups by hovering over the bars, an additional source of information was added to this chart in the form of a legend and labels on male and female passengers when the chart is displaying the grouped categorical axis of passenger class and gender together.

### Resources
Example of bar chart labels for dual categorical x axis:

http://dimplejs.org/advanced_examples_viewer.html?id=advanced_bar_labels

Udacity Data Analyst Nano Degree: Data Visualization materials.
