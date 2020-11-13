# Fire Kite Analysis in Gaza strip area
Use of data mining methods for explore the phenomenon of Fire-Kites launched from Gaza

created by [**Etzion Harari**](https://github.com/EtzionR) and [**Asher Chazan**](https://github.com/ashercha)

![fire](https://github.com/EtzionR/fire-kite-analysis/blob/main/pictures/big_fire.png)

## Introduction
As of 2018, balloons and incendiary kites have been launched from the Gaza Strip towards Israeli territory. These measures have led to **hundreds of fires** in the Gaza surrounding areas. Since launching incendiary means towards Israel is a **large-scale effort** (Almost 2,000 documented events), we believe that the **weather** is a significant consideration in launching the means. This hypothesis is based on the fact that parameters such as wind direction and speed affect the trajectory of the balloons.

Therefore, we chose to use meteorological data on the **wind direction** documented in the Gaza Strip each day. With this data, we will try to pinpoint the source of the balloon launches from the Gaza Strip itself. In addition, we will also use additional data mining tools as well as additional Python packages that we have developed [(**see here**)](https://github.com/EtzionR?tab=repositories) before, for the research.

## Data
Landing points of fire kites in Israeli territory. Data includes coordinates in wgs84 geo dd, date and nickname for each landing location.

source: [landing points](https://www.google.com/maps/d/u/0/viewer?mid=1U3A57H6TCphdux7Sf7dl4z2-1F3vmecJ)

Meteorological records in the required date range, from the **Israel Meteorological Service** (IMS).

source : [IMS](https://ims.data.gov.il/ims/7)

## Descreption
The work flow is divided into three main stages. Full documentation of the work process can be found in the Python notebook: [**fire_kite_analysis.ipynb**](https://github.com/EtzionR/fire-kite-analysis/blob/main/fire_kite_analysis.ipynb)

### 1) Preliminary Processing:
Processing information and converting data so that it possible to work with it. We will also merged the data tables, so we can analyze them. Finally, we will present some statistics and basic information about the data. 

### 2) Data Processing:
We will use a number of tools from the field of data mining, in order to:
* point out the **Main Targets** of the Fire-Kites launchers in Israel area. 
* Identify the **Launched Areas** of the Fire-Kites from Gaza Strip.

In order to do this, we will use a number of codes developed by us:
* **Cumulative HeatMap Calculation:** Code that allows very fast calculation of **heatmap** from given points. We will use it to identify points in Israel area that have hit by large number of Fire-Kites. Full documentation can be seen here: [**cumulative-heatmap-calculation**](https://github.com/EtzionR/cumulative-heatmap-calculation)

* **Clustering by Silhouette:** Code that allows clustering according to the parameter that will return the optimal result (according to the **Silhouette Score**). We will use it to identify clusters of Fire-Kites crash points in Israel area. Full documentation can be seen here: [**Clustering-by-Silhouette**](https://github.com/EtzionR/Clustering-by-Silhouette)

* **create Sector-Shape polygons:** Code that allows calculation of sector-polygon, based on parameters of starting point, angle, standard deviation of the angle and distance. We will use it to calculate the estimated area from which each Fire-Kite was launched. Full documentation can be seen here: [**create-sector-shape-KML-file**](https://github.com/EtzionR/create-sector-shape-KML-file)

### 3) Summary, Conclusions & Export results:
Based on the results we obtained in the previous section, we will propose conclusions about the data studied. We will also export and save the results, so that we can perform exploration on them. You can find the outputs here [**outputs**](https://github.com/EtzionR/fire-kite-analysis/tree/main/outputs) and as Google-MyMaps page here: [**Fire Kite Map**](https://www.google.com/maps/d/u/0/viewer?mid=1msfnGWnLRlIY-xA4YnbLac8vKAJpjb-7&usp=sharing)

![heatmap](https://github.com/EtzionR/fire-kite-analysis/blob/main/plots/sectors_heatmap.png)

## libraries
The code uses the following libraries in Python:

* **matplotlib**

* **simplekml**

* **shapely**

* **pandas**

* **random**

* **numpy**

* **scipy**

* **utm**

In addition, the project includes the use of three packages built by us:

* [**cumulative-heatmap-calculation**](https://github.com/EtzionR/cumulative-heatmap-calculation)

* [**Clustering-by-Silhouette**](https://github.com/EtzionR/Clustering-by-Silhouette)

* [**create-sector-shape-KML-file**](https://github.com/EtzionR/create-sector-shape-KML-file)


## application
The entire research process can be found in the project's Python notebook:

[**fire_kite_analysis.ipynb**](https://github.com/EtzionR/fire-kite-analysis/blob/main/fire_kite_analysis.ipynb)

## License
MIT © [**Etzion Harari**](https://github.com/EtzionR) & [**Asher Chazan**](https://github.com/ashercha)



