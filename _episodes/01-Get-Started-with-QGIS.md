---
title: "Get started with QGIS"
teaching: 20
exercises: 0
questions: 
- "How do we add a vector data into QGIS?"
- "How do we map X and Y Coordinate into QGIS?"
- "How do we add a basemap and a plugin into QGIS?"
objectives:
- "Know how to add vector data into QGIS."
- "Know how to add delimited file into QGIS and map them."
- "Know how to add a basemap into QGIS."
- "Learn how to add a plug in into QGIS"
keypoints:
- "Vector data use X and Y coordinates to define the loctions of points, lines, and areas (polygons) that correspond to map features."
- "To map a delimited file, the file need to have geospatial information (e.g. X Y Coordinates)."
- "X Y Coordinates are longtitude and latutide in degrees. WGS 84 is the most often used geodetic datum to represent coordinates"
- "A variety of basemap can be added to QGIS through adding an XYZ Tile layer."
---

## Familiarize yourself with QGIS

**1.** The main area of QGIS is called the canvas. There are also panels and toolbars, a status bar and menu panels. 

**2.** Panels and toolbars may be moved around and docked at different locations (left-click and
hold to initiate this flexibility).  If you drop a panel on top of another, they will be nested into tabs. Panels you do not used can be removed. Toolbars can be moved around in much the same way, but you cannot nest toolbars into tabs. By right-clicking in the toolbar area, you may get a list of available panels and toolbars you can turn them on and off as you like.

**3.** Through the menu, you can access almost everything in QGIS; some functions have buttons, 
and keyboard shortcuts as well.

**4.** The status bar shows relevant information about the current tool or aspects of the map canvas, like coordinates and scale.

**5.** Toolbox is where you can search for all the tools provided in QGIS. If you can see the toolbox as the figure shows, you can open it in the menu (Processing->Toolbox).

![QGIS Layout](../fig/Figure7-QGIS-layout.png)

QGIS Layout
{: .text-center}

**6.** Use the map navigation toolbar to help navigate your map in the canvas. Here you can find tools to pan and zoom the map, zoom to selected features, and view the complete extent of the map or selected layer. You can also jump to a previous extent with dedicated buttons.  

![QGIS Toolbar](../fig/Figure8-QGIS-tool-bar.png)

QGIS Toolbar
{: .text-center}

## Add data to QGIS

To start, we need to download the data first. There are two shapefiles: Grocery stores [Download](./data/GroceryStore_sp.zip), and Neighborhood boundary [Download](./data/Neighborhood_sp.zip), and a csv file: Apartments [Download](./data/Apartments.csv). The Apartments are thoes which are within 20 min buffer to UCLA by public transit and whose price are less than $1700/month. 

### Add vector data 

**1.**  Left-click the "Layer" menu option, hover over "Add Layer," and left-click the "Add Vector Layer" option. 

![Add a vector layer](../fig/Figure9-Add-a-vector-layer.png)

Add a vector layer
{: .text-center}

**2.**  In Data Source Manager window, click the button and navigate to the folder where the data is. Once select GroceryStores_sp.shp, click Add. 

![Add Grocery store layer](../fig/Figure10-Add-GroceryStores_sp-layer.png)

Add Grocery store layer
{: .text-center}

**3.**  Follow the same procedure and Add Neighborhood_sp.shp.

![Add Neighborhood layer](../fig/Figure11-Add-Neighborhood_sp-layer.png)

Add Neighborhood layer
{: .text-center}

**4.**  After adding GroceryStores_sp.shp and Neighborhood_sp.shp, close the Data Source Manager window.

### Add delimited file

QGIS can convert X Y Coordinates into locations on a map. Open Apartments.csv and you can see X_Coor and Y_Coor columns. These are geospatial information for these apartments. We can map X_Coor and Y_Coor as a point layer in QGIS.

**1.**  In the menu bar, click Layer, then Add layer, and choose Add Delimited Text Layer.

![Add delimited file](../fig/Figure12-Add-delimited-text-layer.png)

Add delimited file
{: .text-center}

**2.**  In the Data Source Manager window
        (1) navigate to the Data folder
        (2) choose Apartment.csv. 
        (3) Make sure Geometry CRS is EPSG: 4326 - WGS84. 
        (4) Click Add. 
        Close the Data Source Managerwindow. Apartments should show in the Canvas. 

![Add Apartments layer](../fig/Figure13-Add-Apartments-layer.png)

Add Apartments layer
{: .text-center}

**3.**  The Canvas looks like the following. There are two points layers (Apartments, and GroceryStore_sp), and one polygon layer (Neighborhood_sp).

![Layout after adding layers](../fig/Figure14-Layout-after-adding-layers.png)

Layout after adding layers
{: .text-center}

## Add a basemap

QGIS provides access to a variety of online base maps. You can add these base maps by building [XYZ Tiles connections](https://www.spatialbias.com/2018/02/qgis-3.0-xyz-tile-layers/). Here we add Google Road/Streets as the base map for the project. 

**1.**  Find XYZ Tiles in Brower. Right click XYZ Tiles. 

![Add a new connection of XYZ Tile](../fig/Figure15-Add-a-new-connection-for-XYZ-Tiles.png)

Add a new connection of XYZ Tile
{: .text-center}

**2.**  In the XYZ Connection window, name the new XYZ Tile as Google Road/Streets, and copy  https://mt1.google.com/vt/lyrs=m&x={x}&y={y}&z={z} into URL. Click OK. 

![Add Google Streets as the basemap](../fig/Figure16-Add-Google-Streets-as-the-basemap.png)

Add Google Streets as the basemap
{: .text-center}

**3.**  Drag Google Road into the Canvas and move Google Road layer to the bottom in Layers Panel. 

![Drag Google Streets to the Canvas](../fig/Figure17-Drag-Google-Streets-to-the-Canvas.png)

Drag Google Streets to the Canvas
{: .text-center}

## Add a plugin 

As an open source software, QGIS have an active community constantly contributing to a variety of tools by developing QGIS plugins. We will use a MMQGIS plugin in this project. 

**1.**  To add a plugin, go to Menu, and click Plugins. Then click Manage and Install Plugins.

![Manage and install plugins](../fig/Figure26-Manage-and-install-plugins.png)

Manage and install plugins
{: .text-center}

**2.**  In the Plugins window, search for **MMQGIS**. Click the mmqgis and then Install Plugin. 

![MMQGIS plugin](../fig/Figure27-MMQGIS-plugin.png)

MMQGIS plugin
{: .text-center}

**3.**  After installation, check the box in front of **mmqgis**. 

![Check mmqgis plugin](../fig/Figure28-Check-mmqgis-plugin.png)

Check mmqgis plugin
{: .text-center}

**4.**  With successful installation, you should see the MMQGIS in the Menu bar. 

![Open MMQGIS in the Menu bar](../fig/Figure29-Open-MMQGIS-in-the-Menu-bar.png)

Check mmqgis plugin
{: .text-center}

{% include links.md %}

