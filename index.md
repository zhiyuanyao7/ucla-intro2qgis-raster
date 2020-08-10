---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
---

{% include gh_variables.html %}
## Welcome to the QGIS workshop
QGIS Quantum Geographic Information Systems (QGIS) is a user-friendly open source Geographic Information System (GIS) licensed under the GNU General Public License. This workshop exhibits a small portion of the many spatial analysis techniques QGIS offers to familiarize you with some of the basics, and to illustrate the fundamentals of GIS. In this workshop for beginners, we will locate apartments that are within 20 min distance by public transit, analyze the price of the apartments and count nearby grocery within a fixed buffer distance.

## Pre Workshop Survey
To get a better backgroud of the participantes and prepare for the workshop, we would like to get some information from you. 

[Pre Workshop Survery](https://docs.google.com/forms/d/1w1wk3f1JLv0quOZwZc1vwXUtTS_-vw83VQlRz6948wQ/edit?usp=sharing)

## Additional resources
Please consult the [Data Science Center](https://www.library.ucla.edu/location/data-science-center), contact us via email (datascience@library.ucla.edu) regarding Geographic Information Sciences (GIS), Geospatial analysis, Data publishing & Sharing, Data & Coding, Statistical analysis, and Carpentries and instruction request and inquiries. 

[Data Science Center](https://www.library.ucla.edu/location/data-science-center) is a division in UCLA library that aims to foster a research community by developing data literacy and foundational coding skills through consulting and education. DSC supports researchers throughout the full data life cycle of activities: planning research projects and data management plans; data acquisition, storage, cleaning, and usage; geospatial analysis; publication; curation; and preservation.

> ## Getting Started
>
> This workshop is hands-on, so participants are encouraged to use 
> their own computers to ensure the proper setup of tools for an efficient 
> workflow. To most effectively use these materials, please make sure to download 
> the data and install everything before working through this lesson.This workshop assumes no prior experience with the tools covered in the workshop. 
> To get started, please download and install [QGIS Version 3.14](https://qgis.org/en/site/). 
{: .prereq}


> ## QGIS project: Housing hunting plan
>
> In this project, you will help a student find a suitable apartment according to several criteria.
>
> | Content | Description |
> | ---- | ------|
> | **Research question** |Where should one student live when he/she wants to find a place where is close to grocery store, the price is lower than $1300/month and within 20 min distance to UCLA by public transit?|
> |**Study area** | Los Angeles County|
> | **Introduction & Objectives** | This workshop applies some basic spatial analysis tools to find out the suitable apartments for students. The objectives of the workshops are being familiar with QGIS layout, being able to use basic spatial analysis tools (e.g. buffer), changing layers properties, and making maps.| 
> |**Methodology**|1. Import csv file with X and Y Coordinates as a layer<br> 2. Add vector layers <br> 3. Project the layer into a proper projection<br> 4. Create buffers<br>5. Join attribute tables<br>6. Changes layers properties <br> 7. Create a print layout and make maps|
> |**Expected results**| Maps are saved for review. For this:<br>1. Learn to save map projects, and create, export, and save map print layouts.<br> 2. Add item contents (i.e. maps, text box, legend, north arrow, and scale bars) to compose a print layout, and modify item properties.|
> |**Analysis & Discussion**|To find the suitable apartment for the students, we need to consider other factors, such as having a car or not, the definition of grocery stores, the network distance instead of Euclidean distance when creating buffers.|
> |**Conclusion**|Thank you for attending the workshop. After reviewing the map, where do you think the best place for a student and why?|
{: .checklist} 

> ## Data
>
> The data used for the workshop are neighborhood boundaries for Los Angeles county, Grocery stores in Los Angeles County, and apartments locations within 20 min distance by public transit and price is less than $1700/month. 
>
> | Dataset | Format | Date | Resource | Description |
> | ---- | ------| ------ |  ---- |  ----|
> | Grocery store [Download](./data/GroceryStore_sp.zip) | Shapefile | 2020-05 | [Los Angeles Open Data](https://data.lacity.org/A-Prosperous-City/Grocery-Stores/g986-7yf9) | The locations of grocery stores in Los Angeles County.|
> | Neighborhood boundaries [Download](./data/Neighborhood_sp.zip) |  Shapefile | 2020-06 | [Los Angeles Open Data Geohub](http://geohub.lacity.org/datasets/la-times-neighborhood-boundaries?geometry=-118.621%2C34.033%2C-118.294%2C34.083) |The administrative boundaries of neighiborhood in Los Angeles County.|
> | Apartment locations [Download](./data/Apartments.csv) | csv | 2020-06 |[Apartments.com](Apartments.com)| The apartments are within 20 mins distance from UCLA by public transit, and the rents are less than $1700/month.The data were webscrapped from [Apartments](Apartments.com) on Jun. 15th, 2020 | 
{: .callout} 

## Post Workshop Survey
Thank you for attending the workshop. You feedback is crucial to improve the workshop and help us provide a better service to a broader community. Thank you for you input! 

[Post Workshop Survey](https://docs.google.com/forms/d/1dvC54QX5KJinK5jkqm-zMhS1p-HF_QVBMjFwZfasY1w/edit?usp=sharing)


{% include links.md %}
