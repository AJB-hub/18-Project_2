<h1> Project 2: Steve, Andrew, Drew, and Marc </h1>

<h2> Topic: Crime related to marijuana dispensaries in Los Angeles City  </h2>

<h3> Central Question: Does crime correlate with location of legal marijuana dispensaries? </h3>

**Data Sets** <br>
Crime Data Set: https://catalog.data.gov/dataset/crime-data-from-2010-to-2019 <br>
CSV file for Crime Data Set: https://catalog.data.gov/dataset/crime-data-from-2010-to-2019/resource/7019ef5a-a383-479c-8a28-8175ced9b7f5 <br>
Dispensary Data Set 1: https://cannabis.lacity.org/personal-activity/find-licensed-retailers <br>
Dispensary Data Set 2: https://search.cannabis.ca.gov <br>
Geographic Areas: https://geohub.lacity.org/datasets/lahub::lapd-divisions/about <br>

**ETL: Crime Data** <br>
• Narrowed down to violent crimes; final dataset contains **996,161** incidents of crime <br>
•	Imported as CSV from Los Angeles City <br>
•	Deleted rows missing location coordinates <br>
•	Deleted columns not needed for analysis <br>
•	Deleted rows with crimes clearly domestic in nature, employee theft, moving violations, or clearly non-violent <br>
•	Created new variable for year of occurrence <br>
•	Grouped weapon used, premise of crime, and crime type into smaller categories <br>
•	Exported data into GEOJSON file <br>

**ETL: Dispensary Data** <br>
•	Contains **420** dispensaries located in Los Angeles City <br>
•	Deleted _known_ non-commercial retail facilities (i.e., cultivation locations) <br>
•	Deleted businesses missing location coordinates <br>
•	Manually examined data for locations with matching addresses or coordinates <br>
•	Dispensary data correlates with Choropleth maps to exclude non-Los Angeles City locations <br>

**Geographic Area** <br>
•	Los Angeles Police Department (LAPD) 21 different "Community Police Station" areas <br>

**Challenges** <br>
•	Could not find a _solid single source_ for dispensary location data - all sources had some data, but no central "source of truth"  <br>
•	Contacted California Bureau of Cannabis Control who sent the website that we had already used  <br>

**Future Improvements/Plans** <br>
•	A vetted, 100% accurate source of retail dispensary locations <br>

**Programs/Libraries Used** <br>
•	Pandas <br>
•	Java Script <br>
•	Leaflet/Mapbox <br>
•	HTML/CSS <br>
•	Plotly <br>
•	GeoPandas <br>
•	GeoJSON <br>
•	Bootstrap <br>

**If Changes Need to Be Made (complicated due to CSV files being too big for Git Hub** <br>
•	Re-run "Project_2.ipynb" and "crime_list.ipynb" <br>
•	In the ETL folder: open and re-run "choropleth" <br>
