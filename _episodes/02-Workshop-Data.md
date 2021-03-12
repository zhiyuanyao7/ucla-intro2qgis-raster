---
title: "Reserach topic and workshop data"
teaching: 40
exercises: 0
questions:
- "What is workshop's topic?"
- "What is the National Land Cover data?"
- "What is TIGER/Line Shapefile?"
objectives:
- "Understand topic of the workshop."
- "Learn where to download shapefiles from census bureau."
- "Learn how to download national land cover data."

keypoints:
- "This workshop will analyze National Land Cover Data (NLCD) using the raster analysis tools in QGIS to investigate the coverage of green space in census tracts in Los Angeles County and identify which census tract has the highest percentage of green space."
- "Topologically Integrated Geographic Encoding and Referencing, or TIGER, or TIGER/Line is a format used by the United States Census Bureau to describe land attributes such as roads, buildings, rivers, and lakes, as well as areas such as census tracts ."
- "NLCD 2016 is an ongoing land cover modeling production effort with NLCD scientists providing expertise in research and development, modeling, scripting, scene selection, cloud-masking, land cover mapping, and imperviousness mapping production. . "
---

## Research topic

Green space helps stabilize both micro- and macro-climates and provides outdoor space for dweller to participate physical activity, engage with nature, and socialize with people. The coverage of green space affects the living experience of dwellers. Estimating the coverage of green space at different census tracts helps the urban planners or policy makers identify areas that have low access to green space and thus provides a reference for actions to improve the green space coverage. 

According to EPA, Land cover that is considered green space includes all land that is vegetated; it excludes barren land, water, and impervious surfaces. This workshop will analyze National Land Cover Data (NLCD) using the raster analysis tools in QGIS to investigate the coverage of green space in census tracts in Los Angeles County and identify which census tract has the highest percentage of green space.

## Data

There are two main types of conceptualizations for digital geospatial data: the vector data model and the raster data model.

### TIGER/Line Shapefile

[Topologically Integrated Geographic Encoding and Referencing](https://en.wikipedia.org/wiki/Topologically_Integrated_Geographic_Encoding_and_Referencing), or TIGER, or TIGER/Line is a format used by the United States Census Bureau to describe land attributes such as roads, buildings, rivers, and lakes, as well as areas such as census tracts. 

### National Land Cover Database (NLCD)
[NLCD 2016](https://www.mrlc.gov/national-land-cover-database-nlcd-2016) is an ongoing land cover modeling production effort with NLCD scientists providing expertise in research and development, modeling, scripting, scene selection, cloud-masking, land cover mapping, and imperviousness mapping production. NCLD 2016 classified the land cover into 20 types (Table 2. NLCD legend), and the land cover dataset have a resolution of 30m by 30m. 

![National land cover legend](../fig/fig4-national-land-cover-legend-1.png)
![National land cover legend 2016](../fig/fig4-national-land-cover-legend-2.png)

National land cover legend (2016)
{: .text-center}

Environmental Protection Agency (EPA) defines the green space as all vegetated land, including agriculture, lawns, forests, wetlands, and gardens. Barren land and impervious surfaces such as concrete and asphalt are excluded. We exclude the 11 Open Water, 12 Perennial Ice/Snow, 23 Developed Medium Density, 24 Developed High Density, and 31 Barren Land and treat the rest of land cover as green space. In the later part, we will apply Raster calculator to filter out the green space. 

{: .text-center}

{% include links.md %}
