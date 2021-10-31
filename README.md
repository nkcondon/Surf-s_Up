# Surf"s_Up
W. Avy has requested a weather analysis on Oahu, Ha for the potential investment in a "Surf and Shake Shop.  Mr. Avy has provided weather data in a SQLite datatbase from January 2010 to August 2017 that includes dates, weather stations, temperature observations, and precipitation. Mr. Avry is requesting information about temperature trends for the months of June and December for Oahu in order to determine if the surf and ice cream business is sustainable year-round.

# Software
Software utilized for the analysis:  Jupyter Core 4.7.1 / Jupter Client 7.27 / Python 3.7.6.

# Overview of Analysis
The data provided by the client was in a SQLite database named "hawaii.sqlite".  To begin the analysis, additional tools were needed amd were "imported":

![image](https://user-images.githubusercontent.com/89953246/139586514-38f82522-4b7f-4d5f-ade5-704b8bc7c1d7.png)

SQLAlchemy was used to connect, create a new model(schema), create classes(reflect) and query the database to perform the analysis. The next requirement was to query the database under the "Measurement" and filter the "date" column for June temperatures. The "extract" function was used to help collect all June data for the 10 years of data.

![image](https://user-images.githubusercontent.com/89953246/139586644-0b34fe88-d6fc-4816-9288-99f84351f694.png)

The June temperatures were then saved as Pandas dataframe and using the "describe()" function to create statistics for June.

![image](https://user-images.githubusercontent.com/89953246/139586795-d4c1aedc-c76e-4a16-8d83-34327796bcb0.png)

The same code was refactored and used to capture December's temperature data and statistics.

![image](https://user-images.githubusercontent.com/89953246/139587259-dd9e8124-c78e-43f1-b1b7-5a3e63648c0a.png)

![image](https://user-images.githubusercontent.com/89953246/139587340-6203be3c-e212-4009-957c-21097ae575c2.png)

# Results
Upon review of the each month's statistics:

![image](https://user-images.githubusercontent.com/89953246/139587486-d69868d7-bafc-475c-aa85-5b9a0d953f8e.png)

Weather data supplied was ample for both months.  

  - For average temperature (Fahrenheit) for June was slightly warmer and Decemeber cooler for the daily lows (June = 74.9F / 64.0F, December = 71.04F / 56.0F).  
  - Within the 50 and 75 percentiles, the temperatures were within 3-4 degrees, with the maxium temperature 85.0F / 83.0 F respectively.
