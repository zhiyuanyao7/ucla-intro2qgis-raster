---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
---

{% include gh_variables.html %}
## Welcome to the QGIS workshop
QGIS Quantum Geographic Information Systems (QGIS) is a user-friendly open source Geographic Information System (GIS) licensed under the GNU General Public License. This workshop exhibits a small portion of the many spatial analysis techniques QGIS offers to familiarize you with some of the basics, and to illustrate the fundamentals of GIS. In this workshop for beginners, we will applies some basic spatial analysis and raster analysis tools to calculate the percentage of green space for each census tract in Los Angeles County and make a map to show the result.

## Pre Workshop Survey
To get a better backgroud of the participantes and prepare for the workshop, we would like to get some information from you. 

[Pre Workshop Survery](https://docs.google.com/forms/d/e/1FAIpQLSfL6bXzCvTz8lCDZqxfenbnJu4-W0MHV1fp999sK0a88fIYhw/viewform)

## Additional resources
Please consult the [Data Science Center](https://www.library.ucla.edu/location/data-science-center), contact us via email (datascience@library.ucla.edu) regarding Geographic Information Sciences (GIS), Geospatial analysis, Data publishing & Sharing, Data & Coding, Statistical analysis, and Carpentries and instruction request and inquiries. 

[Data Science Center](https://www.library.ucla.edu/location/data-science-center) is a division in UCLA library that aims to foster a research community by developing data literacy and foundational coding skills through consulting and education. DSC supports researchers throughout the full data life cycle of activities: planning research projects and data management plans; data acquisition, storage, cleaning, and usage; geospatial analysis; publication; curation; and preservation.

> ## Getting Started
>
> This workshop is hands-on, so participants are encouraged to use 
> their own computers to ensure the proper setup of tools for an efficient 
> workflow. To most effectively use these materials, please make sure to download 
> the data and install everything before working through this lesson.This workshop assumes no prior experience with the tools covered in the workshop. 
> To get started, please download and install [QGIS Version 3.16](https://qgis.org/en/site/). 
{: .prereq}


> ## QGIS project: The green space coverage for tracts in Los Angeles County
>
> In this project, you will some basic spatial analysis and raster analysis tools to calculate the percentage of green space for each census tract in Los Angeles County and make a map to show the result.
>
> | Content | Description |
> | ---- | ------|
> | **Research question** |Which census tract has the highest percentage of green space|
> |**Study area** | Los Angeles County|
> | **Introduction & Objectives** | This workshop applies some basic spatial analysis tools to find out the suitable apartments for students. The objectives of the workshops are being familiar with QGIS layout, being able to use basic spatial analysis tools (e.g. buffer), changing layers properties, and making maps.| 
> |**Methodology**|1. Learn how to download data from census bureau<br> 2.  Clip rast <br> 3. Raster calcualtor<br> 4. Zonal statistics as table<br>5. Join table by attributes tables<br>6. Change symbology  <br> 7. Create a print layout and make maps|
> |**Expected results**| Maps are saved for review. For this:<br>1. Learn to save map projects, and create, export, and save map print layouts.<br> 2. Add item contents (i.e. maps, text box, legend, north arrow, and scale bars) to compose a print layout, and modify item properties.|
> |**Analysis & Discussion**|The definition of green space, the resolution of raster data, and the symbology to visualize the map all affect the result. |
> |**Conclusion**|Thank you for attending the workshop. After reviewing the map, which area has the highest percentage of green space??|
{: .checklist} 

> ## Data
>
> The data used for the workshop are Los Angeles County census tract, Los Angeles County boundary, and National land cover data (30m by 30m). 
>
> | Dataset | Format | Date | Resource | Description |
> | ---- | ------| ------ |  ---- |  ----|
> | Los Angeles County census tract [Download](./data/la_tract_nad.zip) | Shapefile | 2016 | [TIGER/Line Shapefile](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) | The census tract in Los Angeles County.|
> | Los Angeles County boundary [Download](./data/la_boundary_nad.zip) |  Shapefile | 2016| [TIGER/Line Shapefile](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) |The administrative boundary of Los Angeles County.|
> | National land cover data [Download](https://drive.google.com/file/d/1s6pVNL4YzshIL7r0rnMbLlzbw8RIE644/view?usp=sharing) | raster | 2016 |[National land cover data](https://www.mrlc.gov/data)| The National Land Cover Database (NLCD) provides nationwide data on land cover and land cover change at a 30m resolution with a 16-class legend based on a modified Anderson Level II classification system.| 
{: .callout} 

## Post Workshop Survey
Thank you for attending the workshop. You feedback is crucial to improve the workshop and help us provide a better service to a broader community. Thank you for you input! 

[Post Workshop Survey](https://docs.google.com/forms/d/e/1FAIpQLScYFXUJRP4AcS7InJTCZThXDqk1bfYwpz481Ik0_iQlYu8k1w/viewform)


{% include links.md %}
