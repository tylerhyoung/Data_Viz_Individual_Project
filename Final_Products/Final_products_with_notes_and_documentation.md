# Redesign Version

**Please find the three redesigned visualizations on this public tableau story:**
<https://public.tableau.com/profile/tyler.young#!/vizhome/Tyler_Young_Revised_Redesign_Final/FinalRedesignGunViolenceStory>

## Critique and 'making of' thoughts

First in the presentation of the final data products, I tried to tie all three together under one link in a logical fashion using tableau's story functionality. I thought about what would make a cohesive and compelling argurment, something the vox article may have attempted to do but ended up being fragmented or repetitive with little flow. So to start I gave my story a title to encapsulate the message from beginning to end of my three visualizations. In my story I wanted to convey with the first product that America has more guns and more firearm deaths which is a trend seen among developed nations. Then the second chart is actually two bar charts to highlight that the US is unique in firearm murder rate but not overall crime rate. I thought a potential rebuttle to my claim might be that America has more gun related violence just because we have a higher total crime rate. So in my second visualization I tried to preemptively counter that rebuttle and maintain the claim that America is unique in its gun violence. Finally I wrap up the story with a visualization that hopefully shows that gun control laws could potentially be one solution to combatting the higher rates of gun related deaths. In doing this I hoped to at least spur an actionable thought that some gun control, particuarly focused on child safety laws, could improve the situation. 

### Specifics for each data product: 
#### Data Product 1: "More Guns = More Gun Homicides"

Originally I graphed all the countries on three separate charts based on whether they were high, medium, or low ranking on the Human Development Index. But looking back at that data product, I realized I lost track of my primary focus, which was to highlight the United States gun problem. Also I removed the color on the data points and only kept a light red for the trend line, but if it was rendered in another color, or black and white, the message would still come across. I also made a decision to filter the data by the top 30 countries because I was running into some issues with all the labels rendering in such a tight cluster. In doing this I hoped to balance both showing enough data points to see a trend but not so many that only 10 country labels showed up. I also added two captions, one at the top which should be read first to establish where a reader is in the story and give high level description of what the graph is showing and the other caption at the bottom citing the data and my qualifiers for the reader who wants to go more in depth.

#### Data Product 2: "Firearm Murders by Country" & "Total Crime by Country"

Again I added the high level summary at the top to describe where the story goes next, and a caption at the bottom citing the sources and qualifiers. I realize in all my first versions there are no citiations or qualifying captions which would destroy any credibility and faith in the charts being true to some data. In the article's original chart, I did not like the stacked bar chart because it was easy to see the U.S. was similar in total crime, but very hard to see that they are an outlier in firearm murders. So I decided to split the data into two graphs and sort decending for both. I substituted greyscale for color  because color really wasn't adding much and this way I could guarantee that no matter what medium it is rendered on, the charts would highlight the one country that I am telling a story about, which is the United States. I also filtered the countries down so the list wasn't as long, making it easier to read on a smaller device, but more importantly I chose the same countries from the top HDI rank list used in the previous data product to keep some continuity throughout. This was something that the Vox article didn't do because the got the charts from multiple sources. 

#### Data Product 3: "The Benefits of Gun Control"

Once again I added the captions both at the top and bottom, giving a high level description to wrap up the story and cite the data sources, neither of which were in the first version. Additionally I removed color from the graph because the color was saying the same thing as the x-axis and I already wanted to try and show the amount of child safety laws a state had by the size of their dot. I think having multiple legends in the first version, one for color and another for size, made the graph seem more complicated that it needed to be and reduced its clarity. I also reduced the number of categories for size down from 7 to 4 with the goal of making it easier to understand and read.

# Deceptive Version

**Please find the three deceptive visualizations on this public tableau story:**
<https://public.tableau.com/profile/tyler.young#!/vizhome/Tyler_Young_Deceptive_Revised_Version/DeceptiveStory?publish=yes>

Similar to the submission of the redesigned data products, I used Tableau to make a "story" portraying the opposite side that guns in America are not a problem and used tactics to make deceptive visualizations that do not tell the whole truth.

### Specifics for each data product: 
#### Data Product 1: "More guns, less firearm murders."

In this revision, I added a caption both at the top to give a high level description to fit the chart within the context of the story I was trying to tell, and another caption was added to the bottom to cite the data source and qualify the data we are looking at. The deception here comes with the trend line that is skewed by several outliers in the data and it actually appears to say that increasing gun ownership reduces the firearm murder rate. 

#### Data Product 2: "U.S. Firearm Manufacturing and Homicide Rates"

Again I added captions to give a high level description to start and then more details and qualifications down below such as the years and citation. I decided with the revision of this visualization to limit the years to only the more recent ones which would be more compelling for the argument that guns manufactured are not positively correlated with firearm murders. There are several layers of deception, first using guns manufactured might not be the best proxy to say how many individuals in the U.S. have guns because the chart doesn't show how many guns are exported or used for military purposes. Secondly, multiple y-axis are not on the same scale and I actually changed the starting point of the left side to emphasize more of a divergence between the lines towards the end.

#### Data Product 3: "Without Guns, Simple Suicide Methods Still Available"

This was a basic redesign of the original data in the article, which almost looks the same, but I think that is where the deception can really come into play. Taking the same data I just used the percentage of attempts that were fatal or not fatal for each suicide method. This hides the amount of occurences for each method and just tries to show that while guns may be the most fatal method, there are others which are simpler and nearly as effective. In the revision I also removed the red and green colors to replace with black and grey to avoid issues with color rendering or perception that could leave the entire circle looking filled with one color. I also put similar captions on top and below to connect it with the rest of the story and provide details about where the data comes from. 

# Documentation

Please refer to previous documenation for data file and data wrangling as this section for documentation on the revised versions will explain the work to create the visualizations not the sources of the data which are uploaded already to this github repository. 

## Redesign
### Data Product 1: "More Guns = More Gun Homicides"

Using the “2007_world_guns.csv” file I was able to create a scatter plot in Tableau with a trendline to show the relationship between the number of firearms per 100 people and the number of homicides per 100,000 people in the top 30 countries. To determine the top 30 counties, I used the United Nations “Human Development Index” data from 2007. The sheet contains “Firearms per 100” on the columns and “Homicides per 100,000 people” on the rows. Null values were also removed through filters. I changed the title and then created a dashboard to resize the chart and add a caption text box beneath it. Then I added it to a new story.

### Data Product 2: "Firearm Murders by Country" & "Total Crime by Country"
“2002_crime_rates_by_country.csv” was used for this data product redesign. “Country” was put on columns and “Total Crime Rate Per Million” on rows for the first graph. “Firearm Murder Rate Per Million” was put on rows with “Country” on the columns on a separate sheet to make the second graph. Both graphs were filtered by to select as many countries from the top 40 HDI rank list as available in the crime dataset. A bar graph was used for each and sorted high to low from left to right. Then greyscale was added, and United States was singled out in a different shade on each graph. Then the graphs were added to the same dashboard with a title and caption and then that dashboard was added to the next slide in the story.

### Data Product 3: "The Benefits of Gun Control"
“2016_gunlaws.csv” and “2016_violence_by_state.csv” were loaded into Tableau and merged on “state”. For the graph, I used “Lawtotal” on columns and “Deaths Per 100k” on rows. I graphed the trend line. I wanted to improve upon the Vox’s articles way of showing if a state had specific gun control laws in place aimed at improving children safety. So using the “Child” variable, which refers to the number of child safety gun control laws a state has, I created 4 bins and edited the aliases to show the categories properly from 0-2, 3-5, 6-9 and 9+. I then dragged the “child bin” onto size so that larger dots represent states that have more child safety gun control laws. I put it on a dashboard, changed the title, axis labels, gave it a caption and loaded that onto the find slide of the story.

## Deception
### Data Product 1: "More guns, less firearm murders." 
“2007_world_guns.csv” was loaded into Tableau.‘Firearms per 100’ was put on columns and ‘Homicides per 100’ on rows. I renamed the axis and set a title. I also filtered out null values and dragged "country" to label and set a filter on HDI rank from 1-100. Graphed the trendline and created a dashboard with a caption beneath citing the data and qualifying it. Finally I created a story and put this on slide 1 with a high level caption to start the story and a title for the story.

### Data Product 2: "U.S. Firearm Manufacturing and Homicide Rates"




### Data Product 3: "Without Guns, Simple Suicide Methods Still Available"
“Illinois Suicide Distribution 90-97.csv” was loaded into Tableau. Columns "Pct Fatal" renamed to "Fatal". I then created a calculated field for "Not Fatal" just 100-"Fatal". In sheet, I selected ‘Pie’ from Marks drop down field. Dragged Suicide Method to Columns and ‘Measure Values’ to Angle removing all measure values except ‘Fatal’ and ‘Not Fatal’. Then I dragged ‘Measure Values’ to Color and set to ‘Custom Diverging’ with 2 steps. Set colors to grey and black. Next I moved ‘Suicide Method’ to Filters and selected only ‘Firearms’, ‘Crash/jump’, and ‘Suffocation’.Then I dragged the 'Measure names' and 'Measure values' to labels. Finally I created a dashboard, changed the title, added a citation caption below and put it on the last slide in the story with a descriptive caption above.
