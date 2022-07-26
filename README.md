# Olympics-Visualisation:
Exploratory Data Analytics and Visualisation

# Why?
Across the world, many of us are sitting eager as we begin to watch the trials for the much anticipated 2025 Summer Olympics. Although this event is always seen as a historic, we find this Olympics to be especially momentous as it brings new hope for collective unity and optimistic spirits proceeding the great challenges and uncertainty of the past year and a half. No matter where you end up watching from or the flag you’re waving, together we will witness again true displays of hard work and passion from athletes around the globe, reminding us all the values of good character and teamwork. At the same time, it’s a competition and the bedrock of competition is Data Analysis and its subsequent Visualisation. We, here in this project are using this rich history of Olympics and the data that comes accompanied with it to create a Dashboard so that we can share the joy of Data Analysis to everyone through intuitive visualisations so that even if someone is a layman in terms of this field can get across the analysis we want to showcase. We must select a Dataset first and do Data Abstraction to find out the data types and the nature of the dataset as all the future tasks is dependent on this step, then based on the dataset we need to declare the Data abstractions thinking upon what the Users might want and need because the Visualisation is for no other than them. Also, this is a demonstration of how easy it is to make a Utilitarian dashboard by simply using R for Analysis and Flexdashboard library of R to visualise the analysis.

# Problem Statement:
As Tokyo Olympic Games just drew to an end,we review here 120 years history of Modern Olympic Game. Modern Olympic Games are leading international sport events featuring summer and winter sports competitions. The creation was inspired by the ancient Olympic Games, held in Olympia, Greece from the 8th century BC to 4th century AD. The first modern Games was held in Athens in 1896, and ever since Olympics has been happening almost without a stop, except during Wars. But, there hasn’t been much investigations into visualising this data, but due to the huge landscape of data, which are memories that Olympics have created throughout the history; it will be a disservice to the great athletes and their history if we don’t reignite the history; in this project as a form of a Dashboard where we can investigate the history again. Thus, this gives us a great foundation for a Demonstration project through which we want to develop and demonstrate the various visualisation that can be used and how different inferences can be drawn from that.

# Hardware Requirements:
Hardware Requirements:
Any modern System will do.
Software Requirements:
R.
R Studio.
These libraries:
library(flexdashboard)
library(tidyverse)
library(plotly)
library(treemapify)
library(gganimate)
library(gifski)
library(png)
Any modern browser to see the html file consisting of the dashboard.

# DATA ABSTRACTION:
Attributes:
ID - Unique number 
Name - Athlete's name - NOT USED
Sex - M or F
Age - Integer
Height - In centimeters - NOT USED
Weight - In kilograms - NOT USED
Team - Team name
NOC - 3-letter code
Games - Year and season
Year - Integer
Season - Summer or Winter
City - Host city - NOT USED
Sport - Sport
Event - Event
Medal - Gold, Silver, Bronze, or NA
The dataset is in form of a Table with Attributes and Items.
Quantitative - ID,Age,Height,Weight,Year
Qualitative - Name,Team,NOC,Season,City,Event,Medal
Discrete - ID,Age,Height,Year
Continuous - Weight
Nominal - ID,Name,Sex,Team,NOC,City,Sport,Event, Season,Medal,Games
Ordinal -Medal
Interval - Year,Games(Mixed)
Ratio -Age,Height,Weight
There’s no Cyclic or Diverging datapoint. Every attribute is sequential.
This is a historical dataset on the modern Olympic Games, including all the Games from Athens 1896 to Rio 2016. The author scraped this data from www.sports-reference.com in May 2018. 

The Winter and Summer Games were held in the same year up until 1992. After that, they staggered them such that Winter Games occur on a four year cycle starting with 1994, then Summer in 1996, then Winter in 1998, and so on. A common mistake people make when analyzing this data is to assume that the Summer and Winter Games have always been staggered.
The dataset contains 271116 rows and 15 columns. Each row corresponds to an individual athlete competing in an individual Olympic event (athlete-events)
Link: https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results

# Task abstractions Identified:
The Variation Female Participants In Comparison To Male Participants-Line graph
Relationship Between Height Vs Weight Vs Age of Participants -Scatterplot
Top 10 Nations To Win Gold, Silver and Bronze Medals-Donut Chart
Word-Cloud Visualizing Sports In Which India Has Won Medals
Top 3 Male/Female  Athlete's By The Number Of Medals using Sunburst Chart
Different Cities Hosted The Olympic Games Over The Years using World Map
Sports That Have Most Number Of Events using Treemap
Finally make Inferences based on these charts
Indicate the number of Athletes based on countries on a Word Cloud-Present and find patterns
The Relation Between Various Features And Labels In The Olympics Dataset- Production, Derive Patterns
The Overall Spread Of The Age Of Athletes on- Boxplot
The Overall Trend Of The Summer Olympics Participation-Line graph
