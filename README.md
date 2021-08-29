# COVID-19-Tracker-on-Android
Tracking COVID-19 latest Global and Countries Stats on Android through API.

This App takes an API: https://corona.lmao.ninja/v2/all/ to obtain all the data related to COVID-19 stats.

**Volley** Library is implemented to fetch data from the API.

This App related website is also built by me using React JS: https://covid19bybikashro.netlify.app/
Github: https://github.com/BikashBIOS/COVID-19-Tracker-using-React-JS-and-Material-UI

**LIBRARIES USED:**
1) Card View - For Making Cardview of a separate components.
2) SimpleArcLoader - For the Loading animation for the time the data gets fetched from the API.
3) Glide - To portray the image of the Country flags.
4) Volley - For Getting the Requests from the API
5) Blackfizz EazeGraph - For building the PIE chart for the data fetched.


**PROCESS**

1) Country Model contains all the Constructor and the Getter Setters for the attributes i.e flag, country names, cases, deaths, today cases, recovered, active and critical.
2) MyCustomAdapter filters the Countries by taking list of the countrymodel.
3) Affected Countries contains the main fetchData function to get all the data from the API for a separate country.
4) It makes a String request from the API url and creates a JSON Array with the response.
5) With the help of Looping and JSONObject, we get all the attributes data for all the countries.
6) Pass the values to the Country Model using its class and objects.
7) Now pass the adapter to the MyCustomAdapter and set the adapter in the list view.
8) DetailActivity contains the data of a particular country of all its attributes with just the country position and get it from the functions.
9) In the Main Activity, fetchData and add the Cases, Recovered, Active and Deaths in a Pie Chart by their JSONObjects.


**NOTE: This Project was made by Me in my 2nd year of B. Tech**

Copyright Disclaimer Under Section 107 of the Copyright Act 1976, allowance is made for "fair use" for purposes such as criticism, comment, news reporting, teaching, scholarship, and research. Fair use is a use permitted by copyright statute that might otherwise be infringing. Non-profit, educational or personal use tips the balance in favor of fair use.
