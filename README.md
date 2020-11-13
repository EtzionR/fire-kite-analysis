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
The work flow is divided into three main stages:
1) **Preliminary processing:** Processing information and converting data so that it is convenient to work with. We will also consolidate the data tables so that we can make convenient use of them. Finally, we will present some statistics and basic information about the data. 

