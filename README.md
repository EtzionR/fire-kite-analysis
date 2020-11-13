# Fire Kite Analysis in Gaza strip area
Use of data mining methods for explore the phenomenon of Fire-Kites launched from Gaza
created by [**Etzion Harari**](https://github.com/EtzionR) and [**Asher Chazan**](https://github.com/ashercha)

![fire](https://doc-14-a8-mymaps.googleusercontent.com/untrusted/hostedimage/ipoo8mp319b8e6mg6ncdrjunqg/s8vfnugmcub72seqcntcacs0cc/1603390863750/Df5aJXzzJ_VZsWx8RPJQ9JMPHivr6YGw/13576183864254850826/5AF2TALovrR4feukkEEa1Ltxo7KyCI3QrgigN7l771FkXDHBwBe3uahV_gX3fQFMHHuw7jvQVgKHypf9u6go7vEpEJ2s3gVyb_2xUwBVt4j38j_kunYxJVH82hsW9agPeYjXeFLZZvw1-Ihtc1kjYcHNQwDdcOGFM1sVz2r3wEBcthvQ-jlkzqrm25l-MkaF-QFypDEEfzJQ7E1UPe5LSdhFp8X-_9123xYbpqTJhlvy360bZ86W8KMPN6RUQLHghwonVK3uJNprkM_n1f8C-JQOHs5JIt9Aj_Q?session=0&fife=s16383)

## Introduction
As of 2018, balloons and incendiary kites have been launched from the Gaza Strip towards Israeli territory. These measures have led to **hundreds of fires** in the Gaza surrounding areas. Since launching incendiary means towards Israel is a **large-scale effort** (Almost 2,000 documented events), we believe that the **weather** is a significant consideration in launching the means. This hypothesis is based on the fact that parameters such as wind direction and speed affect the trajectory of the balloons.

Therefore, we chose to use meteorological data on the **wind direction** documented in the Gaza Strip each day. With this data, we will try to pinpoint the source of the balloon launches from the Gaza Strip itself. In addition, we will also use additional data mining tools as well as additional Python packages that we have developed [(**see here**)](https://github.com/EtzionData?tab=repositories) before, for the research.

## Data
Landing points of fire kites in Israeli territory. Data includes coordinates in wgs84 geo dd, date and nickname for each landing location.

source: [landing points](https://www.google.com/maps/d/u/0/viewer?mid=1U3A57H6TCphdux7Sf7dl4z2-1F3vmecJ)

Meteorological records in the required date range, from the **Israel Meteorological Service** (IMS).

source : [IMS](https://ims.data.gov.il/ims/7)


