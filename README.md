# surfs_up
Weather data analysis /Jupyter nb /SQLLite /Flask

## Project Overview
In order to be able to open a Surf and Shake shop serving surfboards and ice cream to locals, tourists in Oahu,Hawaii ,we run a SQLite analysis on Temperature trends .This project explores the power of Advanced Data Storage and Retrieval to efficently produce an analyis of temperature trends in Oahu, Hawaii.
### Purpose
Considering temperature data for the months of June and December in Oahu, we run our analysis in order to determine if the surf and ice cream shop business is sustainable year-round. In order to achieve this weather has to be in out favor for most number of days throughout the year.

![b5f3c2c56052b9e344b9b14fb886342f](https://user-images.githubusercontent.com/119648166/220239451-7597e418-ba4a-42f7-b7ef-6dc95e62fd6c.jpg)

## Results
The analysis focuses on the key differences in weather between June and December.



 - summary statistics for the June  and December temperatures

 
 ![summary stats](https://user-images.githubusercontent.com/119648166/220239750-55cf7833-c9b9-4444-af2f-ac3155b30fac.png)
  Fig : Summary Statistics of Temp
#### Comparison of the Temperatures for June and December

**1. Number of data**

-   There are less data points for December (1517 data points) than for June (1700 data points).

**2. Dispersion of the data**
-   Temperatures are more spread out in December (std = 3.7) than in June (std = 3.25).
-   June’s mean and median are 74.94 °F and 75.00 °F respectively.
-   December’s mean and median are 71.04 °F and 71.0 °F respectively.
-    The average recorded temperature in June is about 75 degrees F, 4 degrees higher than the average temp in December.
    This represents a -5% change in average temperature from June to December.

**3. Quartiles**

-   1st quartile: 25% of all data is below 69 °F in December and 73 °F in June.
-   3rd quartile 75% of all data is below 74 °F in December and 77 °F in June.

-   The December temperatures seem to be more variable than those in June given its larger range in recorded temperatures (comparing the max vs min temp of each month)
    -   However, when looking at the plotted distribution of Dec Temps, we can see that the median temperature in Dec is more inline with the average, and there are not many outliers skuing the average temperature higher or lower than the actual recorded frequency.
![image](https://user-images.githubusercontent.com/119648166/220240152-ea8a5b90-6070-474e-96c6-a6ae67b379f9.png)
 Fig : Temperature vs Frequency  recorded in June
![image](https://user-images.githubusercontent.com/119648166/220240185-b066e61d-9a0d-425e-b741-fd20a9265743.png)
  Fig : Temperature vs Frequency  recorded in December

-   The frequency of temperatures recorded in June tends to have a much more normal, tight bell curve distribution, cooroborated by the smaller std measure of June temps vs December temps.
### Comparison of the Rainfall for June and December.
![image](https://user-images.githubusercontent.com/119648166/220240596-1983e53d-3753-4fbc-a6ac-d04e01bd2723.png)
Fig : Rainfall Stats in June and December.

**1. Number of data**

-   There are less data for December (1405 data points) than for June (1574 data points).

**2. Dispersion of the data**

-   Rainfall quantity is more spread out in December (std = 0.5) than in June (std = 0.33).
-   June’s mean and median are 0.13 inches and 0.02 inches respectively.
-   December’s mean and median are 0.21 inches and 0.03 inches respectively.
-   Maximum rainfall in December is 6.42 inches and 4.43 inches in June.
-   Minimum rainfall in December is 0 inches and 0 inches in June.[Rainfall in June and December Stats](%22C:%5CUsers%5Csmita_emkucur%5CDesktop%5CBoot%20Camp%5CMod%209%20Python-sqllite-flask%5Csurfs_up%5Crainfall.png%22)

## Summary
### Temperatures for June and December

From the temperature report we can see that there is not much difference in the weather in June and December, indicating mild and steady temperatures year-round. .To find out protentional outliers and other trends  **the box and whiskers chart**  can tell us more about that.
![image](https://user-images.githubusercontent.com/119648166/220240686-6815619a-3f0e-4730-8938-10c357de463d.png)

From the graph we can see that there are just a few outliers. There are more outliers below the lower boundary in December, however the minimum temperature is 56 °F.

###  Rainfall for June and December

The first difference that we notice is the max rainfall in June and December (4.43 and 6.42 inches respectively) and in both cases, highly above the mean.
Also, standard deviation is high, mean and median or 2nd quartile are far apart, meaning that distribution of the data is highly spread out. That indicates the presence of extreme values in the dataset. The easiest way to determine outliers is to plot **box and whiskers chart**.
![image](https://user-images.githubusercontent.com/119648166/220240719-4d46be7b-ffbd-4939-8a18-483f3cbba9f1.png)

To get a better understanding of the average rainfall every year,I have plotted another graph .
![image](https://user-images.githubusercontent.com/119648166/220240741-45e615f8-7c99-4889-81d6-f20426a29ed9.png)

From the graph above ,we notice that  December 2010  had heavy rainfall.However,there is  significant drop in the following years. The rainfall became pretty steady in the following years without much variation in both months.

