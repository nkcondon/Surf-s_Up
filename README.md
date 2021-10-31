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
![image](https://user-images.githubusercontent.com/89953246/139587103-62907143-0d0c-42e3-a2bd-2ce1dfb0df2c.png)
