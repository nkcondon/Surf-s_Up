# Surf"s_Up
W. Avy has requested a weather analysis on Oahu, Ha for the potential investment in a "Surf and Shake Shop.  Mr. Avy has provided weather data in a SQLite datatbase from January 2010 to August 2017 that includes dates, weather stations, temperature observations, and precipitation. Mr. Avry is requesting information about temperature trends for the months of June and December for Oahu in order to determine if the surf and ice cream business is sustainable year-round.

# Software
Software utilized for the analysis:  Jupyter Core 4.7.1 / Jupter Client 7.27 / Python 3.7.6.

# Overview of Analysis
The data provided by the client was in a SQLite database named "hawaii.sqlite".  To begin the analysis, additional tools were needed amd were "imported":

![image](https://user-images.githubusercontent.com/89953246/139585989-b6882caa-5e43-48aa-9e56-1fca348e050e.png)

SQLAlchemy was used to connect, create a new model(schema), create classes(reflect) and query the database to perform the analysis. The next requirement was to filter the database for June temperatures adding the "extract function".

