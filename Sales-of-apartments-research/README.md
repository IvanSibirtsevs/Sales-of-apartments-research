# Study of ads for the sale of apartments

***We have at our disposal the data of the Yandex.Realty service - an archive of ads for the sale of apartments in St. Petersburg and neighboring settlements for several years. You need to learn how to determine the market value of real estate. Our task is to set the parameters. This will make it possible to build an automated system: it will track anomalies and fraudulent activity.***

**Two types of data are available for each apartment for sale. The first ones are entered by the user, the second ones are obtained automatically on the basis of cartographic data. For example, the distance to the city center, airport, nearest park and body of water.**

- Studying the time of sale of the apartment.
- Exclusion of rare and outliers
- Factors most affecting the cost of an apartment?
- For apartments in St. Petersburg, which area is included in the center
- A segment of apartments in the center. Do the following parameters affect the price: area, price, number of rooms, ceiling height.


### Step 1. Open the data file and examine the general information.
- Empty values ​​in living_area, ceiling_height, living_area, is_apartment,balcony, cityCenters_nearest, parks_around3000, parks_nearest, ponds_around3000,ponds_nearest, days_exposition
- Wrong data type in almost all columns

### Step 2. Data preprocessing

### Step 3. Calculate and add to table

### Step 4. Conduct an exploratory data analysis and follow the instructions:

***The average area of ​​apartments is about 50 meters The most frequent apartments have 2-3 rooms The average ceiling height is a little more than 2.5 meters There is a very large spread in the histogram with the price (There are very cheap real estate and very expensive) ***

***There are very large outliers. more than 500 days, I think this is due to illiquid real estate or people constantly forget to remove ads from sites.
Most apartments are sold within 3 months.
It’s fast for a month, but for a long time it’s more than six months ***

***The average area of ​​apartments is from 30 to 70 meters (There are also quite large apartments up to 900 meters)***
200 is the number after which there are large outliers. I calculated it using the 75% quantile.

***The price depends on the size of the apartment. The larger the area, the higher the price***

***The most expensive apartments with 8 rooms and the price also strongly depends on the number of rooms***

***Remoteness from the center affects the price, but the farther away the price almost does not change***

*** The cheapest apartments are on the first floor, but on the top and the rest they cost about the same
(I think this is due to the bars on the windows and the noise).***

***The most expensive apartments are put up for sale on weekdays.***

***The cheapest apartments are exhibited from the end of spring and the beginning of summer. The rest of the months are pretty much the same***

***Conclusion:***
- The price depends on the size of the apartment. The number of rooms also greatly affects the price,
- But strange as it may seem, apartments in the very center and on the outskirts of the central part of the city cost about the same.
- The cheapest apartments are on the first floor, but on the top floor and the rest they cost about the same (I think this is due to the bars on the windows and noise).
- The most expensive apartments are put up for sale on weekdays.
- The cheapest apartments are exhibited from the end of spring and the beginning of summer.
- The year of publication does not affect the price
- Housing prices fell from 2014 to 2015 and started to recover slightly from 2018 to 2019

***The most expensive city to live in is St. Petersburg, but the cheapest is Vyborg***

***The central zone is located at a distance of 3-4 kilometers from the city center.***

***Histograms are similar, but flats in the center are slightly better in everything. Except price***


- Residents of the center sell cheaper properties on weekends
- Also, the cheapest apartments are sold not only at the end of spring, but also in the winter before the new year
- You can clearly see that the farther from the center the cheaper.

### Step 5. General conclusion
***Everything affects the price of an apartment. From the distance to the center, to the number of rooms.***
- The most important parameters are the number of rooms and the area of ​​the apartment.
- The cheapest apartments are on the first floor
- Apartments in the center are more expensive and smaller in area.
- The most expensive apartments in St. Petersburg, but the cheapest in Vyborg
