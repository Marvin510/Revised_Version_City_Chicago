# Marvin Miranda Olmedo
# Revised_Version_City_Of_Chicago

https://public.tableau.com/profile/marvin.olmedo#!/vizhome/FinalVersionIndProj/Dashboard1?publish=yes

# Structure for all 3 visualizations
- Data exploration & Assumption
- Hypothesis
- Conclusion
- Improvements
- Image of final product
- The making of visualization with previous thesis, hypothesis, conclusion and improvements



# Visualization #1

Data Exploration Assumption
-	Questioned why certain cameras had more violations
- Assumed the location of these cameras was not arbitrary

Hypothesis
- There are more cameras in impoverished areas
- Plot with poverty index bins supported this idea

Conclusion
- Poverty areas are not targeted 
- School locations are the main driver of camera amounts ("Chicago Public Schools - School Profile Information SY1617 | City of Chicago | Data Portal")
- Violations increase with a higher camera count

Improvements - Interaction based on:
- Poverty Indexes
- Joined Chicago’s school data set to evaluate correlation between camera location and violations
- These improvements helped in clarifying whether or not poverty indexes were correlated with camera locations, the new data set provided location and count of schools.

## FINAL - Visualization# 1

![FinalPic1](https://github.com/Marvin510/Revised_Version_City_Chicago/blob/master/Pics/1.png "Fianl1")



### The making of visualization# 1 with previous thesis, hypothesis, conclusion and improvements

There are more cameras in impoverished areas.(Original Assumption)

While doing the data exploration assignment, I questioned the bias of some cameras locations.

For example, Camera ID 149 had by far the most violations. I found this stood out and deserved a deeper analysis. 

![Pic1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic1.png "Skewdata")


At first, I couldn’t make any assertions about why some areas and cameras had a disproportionately higher amount of violations. Furthermore, I felt the City of Chicago website did not provide enough information to justify their claim that cameras were installed around 1/8 of a mile from schools and parks. ("Children's Safety Zone Program & Automated Speed Enforcement")

Because of this, I suspected there was a bias with the location of the cameras and believed this would lead me to an interesting finding.

I started by investigating zip codes and realized that the original dataset presented the following limitations:
-	Zip codes were wrong
- Community areas and wards did not provide obvious insights

I tackled the zip code issue by exploring other data sets and I came across the Socio Economics Issue Data set from the City of Chicago. ("Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal")

This data set provided a column called Hardship Index, which collects socioeconomic indicators of the residents of Chicago.

This Index assigns areas with more poverty a higher ranking and vice versa.

I suspected at this point that location of cameras could be driven by economic issues and thus decided to explore differences between impoverished and rich areas.

Visualization number 1 would attempt to find if there are more cameras in lower income zip codes across Chicago resulting in biased violation data.

I plotted a count of cameras to hardship index. The first graph did not show obvious bias.

![Pic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.png "Countofcameras")

I also tried to graph a linear graph to see if there was an increment of cameras as Hardship increased. In this image, there was improvement yet there was a lot of missing values.

![Pic2.2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic2.2.png "Lines")

I then created a calculated field that assigned any Hardship index above 50 to Poor else Rich, with the intention to find a correlation.

This image did show that there are more cameras in poorer areas, but I didn't think it was convincing enough.

I also took a detour in my thinking. Up to this point, I wanted to prove with my visualization to the Mayor of Chicago that I had found evidence that impoverished areas are more policed. I decided that is not the message I would try to convey with my visualization.

![Pic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic3.png "Calculatedfield")

Finally, I decided to bin the Hardship Index in size bins of 10 and this is where I found a straight answer to my question.


There are more cameras in poorer areas than in rich areas. Specifically if Hardship Index is above 70 and this is the message that I would covey.


![FinalPic#1](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPict%231.png "Visualization#1")

### Enhancements road map

- A future enhancement to this visualization would be to optain school locations to prove or disprove that cameras have been installed 1/8 of mile from schools as the City of Chicago Claims.
- Consider other socio economic factors that may be affecting the location of cameras
- Explore population differences among indexes.




# Visualization #2

Data Exploration Assumption
- Assumed that party with largest representation would have the ward with highest violation 
- Democrats control 48 out of 50 wards, thus I assumed they would have the ward with highest violations

Hypothesis
- Democrats would have the ward with highest violations across years and poverty indexes

Conclusion
- Although Democrats have the majority representation, they did not represent the ward with the highest violation
- Ward# 38 has the only Independent representative with significantly more violations across years and poverty indexes

Improvements - Interaction based on:
- Poverty Indexes
- Years
- Validated that ward# 38 did not have demographics differences and the only interesting difference was its political representative
- Interaction of poverty indexes and years support the idea that ward#38 is very unique. Through out years and across indexes it remained the highest.

# FINAL - Visualization# 2

![FinalPic#2](https://github.com/Marvin510/Revised_Version_City_Chicago/blob/master/Pics/2.png "FinalVisualization#2")



## The making of visualization# 2 with previous thesis, hypothesis, conclusion and improvements

- The city of Chicago is divided into 50 wards. Each ward has 1 representative. There is 1 ward that is not controlled by a Republican or Democrat. This ward is controlled by an Independent. 
- The ward with the only Independent Representative has the highest amount of violations.

While researching the zip code issue from the original data set I came to realize that I did not understand the meaning of the Wards. 

I turned to Wikipedia and found data on wards and how each has a political representative. ("Chicago City Council", 2019)

Quickly realized that the City of Chicago has a democratic majority. I thought it would be interesting to see if wards ran by other parties differed from democrats in number of violations.

At first, I plotted zip codes which required me to download another data set called Ward Offices. ("Ward Offices | City of Chicago | Data Portal")

I had to split column location to create longitude and latitudes.

I then created a map of violations by zip code and political party. I color coded the zip codes by number of violations. The darker the color the higher the violations.

From this image, I couldn’t  make any clear statements about violations and parties.


![Pic4](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic4.png "zip code")


I then proceeded to think of Wards rather than zip codes and created a visualization that showed violations by Wards.

Here is where I found my interesting finding; there are only 2 Wards not controlled by Democrats, one of them is an Independent and the other is a Republican. 

The Ward with the highest amount of violations is represented by an Independent.

I thought this was a very intersting finding that does not imply or claim anything but is something I was not expecting.

![FinalPic2](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%232.png "Visualization#2")

### Enhancements road map
 - I would like to explore demographics of this Ward
 - I would like to see if this Ward differs from others on socio economic factors
 

# Visualization #3

Data Exploration Assumption
- Assumed that certain days would have more violations
- Presumably Monday through Friday as cameras target school hours and locations

Hypothesis
- Weekdays will have the highest violations
- Friday had the most violations based on the sum of violations per day  

Conclusion
- Averaging weekends showed significantly more violations across years, wards, and poverty indexes
- Saturday and Sunday consistently reported more than any weekday

Improvements - Interaction based on:
- Poverty Indexes
- Years
- Political Party
- These improvements helped in clarying if weekends had varience of violations in other wards, poverty indexes or years.

# FINAL - Visualization# 3

![FinalPic#3](https://github.com/Marvin510/Revised_Version_City_Chicago/blob/master/Pics/3.png "FinalVisualization#3")

## The making of visualization# 3 with previous thesis, hypothesis, conclusion and improvements
### Keeping in mind that school is in session Monday through Friday, weekends should have less violations. Which is the opposite of what is truly happening.

In the data exploration process, I designed a visualization that showed Friday as the day with more violations. I received criticism and thus decided to build on that mistake. Perhaps, explore if this visualization could lead to an interesting finding.

![Friday](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic5.png "Friday")

From feedback received, I wanted to explore different ways to properly show this information.  I decided to explore changes through out the years instead of day. 

![Pic6](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Pic6.png "Years")

After analyzing weekdays and years, I decided to add weekends and realized that on average Friday is not the day with more violations.

This is an intersting finding considering the fact that school is only in session during weekdays.

![FinalPic3](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/FinalPic%233.png "Visualization#3")


### Enhancements road map
- Would like to create a forecast
- Would like to breakdown by wards
- Would like to compare by zip code and Socio economic Factors


# Data Wrangling


- I had to retrieve information from multiple sources.

- Combined all Data Sets into a spreadsheet.

- Mapped and joined the tables. 

![joinss](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Jointss.png "joinss")


- I had to physically draw the attributes I needed to analyze if joining the different data sets was feasible.

![joins](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Joins.png "joins")

- Created bins for Harship Index

![bins](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/bins.png "bins")

- Created IF statements to categorize rich or poor in the column called Harship Index.

![if](https://github.com/Marvin510/ChicagoSpeedViolations/blob/master/Images/Calculated%20field.png "ifstatements")

- Split columns to find Longitude and Latitude of Wards.

- Added Data Set "Chicago Public Schools - School Profile Information SY1617"

- Cleaned N/A values

# References

- Children's Safety Zone Program & Automated Speed Enforcement. (n.d.). Retrieved April 27, 2019, from https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html

- Census Data - Selected socioeconomic indicators in Chicago, 2008 – 2012 | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2

- Chicago City Council. (2019, April 26). Retrieved April 27, 2019, from https://en.wikipedia.org/wiki/Chicago_City_Council

- Ward Offices | City of Chicago | Data Portal. (n.d.). Retrieved April 27, 2019, from https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Ward-Offices/htai-wnw4

- Chicago Public Schools - School Profile Information SY1617 | City of Chicago | Data Portal. (n.d.). Retrieved May 5, 2019, from https://data.cityofchicago.org/Education/Chicago-Public-Schools-School-Profile-Information-/8i6r-et8s
